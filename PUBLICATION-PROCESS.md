# Publication Process for resolved Issues

This is a short description of what happens after the PDF Association PDF TWG agrees that an issue resolution:

* `_config.yml` should not need changing.

* The `docs/index.md` is the main page but shouldn't need changing too often unless a new standard is being added.

* `docs/_data/data.yml` will also need updating if a new standard is added.

* Individual corrections are applied to the MD files below `docs/_clauses`.
   - Sub-folders are named after each ISO standard in the form `<iso-number>-<iso-part>-<year>`.
   - Each clause file in each sub-folder is named `clauseXXX.md`.

* Each ISO standard also has a specific landing page at `docs/_clauses/<iso-standard>/index.md`.
   - This should not need changing once created, as Liquid is used to generate the index to each top clause based on the file `docs/_data/data.yml`.
   - When creating a new standard, copy an existing file and just change the top matter. Data is pulled from `docs/_data/data.yml`.

* If a new `docs/_clauses/<iso-standard>/clauseXXX.md` Markdown file is added, then the `docs/_data/data.yml` will need updating to ensure the new clause occurs on the correct standard-specific language page, and in the correct order.

* All clause MD files have special Jekyll top matter which is required. The matter is used by Jekyll/Liquid to create indices, ToCs, set page title and meta tags, etc.

* Edits are done manually with a lot of manual HTML formatting and fiddling to get the closest possible appearance to a "track changes" of ISO 32000-2:2020.

* Just like in ISO 32000-2:2020, keys are **bold** and values are _italic_.
   - No attempt is to made to make the table columns retain their same width in the relevant standard.

* We fully respect ISO copyright so only small amounts of surrounding text are used. Typically just the paragraph in question so that the track change is clearly understandable with some context and is easily and clearly locatable within the relevant ISO standard. Headings (clause titles) and Table numbers are always used to aid location.

* Ellipsis (...) paragraphs are used to visually indicate missing stuff from ISO standards. Otherwise the resolutions look like adjacent paragraphs when they're not!

* The track-changes styling is implemented via `_includes/iso-style.html` which is an inline set of styles that are `%-included` into each `docs/_clause/<iso-standard>/clauseXXX.md` MarkDown file. We cannot use a proper CSS since the current Jekyll theme won't reliably get altered.

* Edits are currently split into separate clause pages based on top level (`H1`) clauses in each ISO standard.

* The heading `<hX>` tag in the `docs/_clause/<iso-standard>/clauseXXX.md` matches the nearest heading level in the ISO standard for each resolutions. If the heading title is something highly generic (e.g. X.Y.Z General) then also add the next highest heading (e.g. X.Y Topic) is added. This means heading numbers are not contiguous!!

* Anchor IDs are added to all headings (level 2 and greater) and all Table captions:
   - Heading IDs start with "H" and then have the precise heading numbering (or lettering for annexes)
     ```html
     <h4 id="H12.5.6.2">12.5.6.2 Markup annotations</h4>
     <h2 id="HH.8.2">H.8.2 Table of Contents</h2>
     ```
   - Table IDs are "Table" followed by the table number from the PDF specification (incl. letters for tables in annexes)
     ```html
     <caption id="Table50">Table 50 - Operator categories</caption>
     <caption id="TableA.1">Table A.1 - PDF content stream operators</caption>
     ```

* URLs can then be used to jump to a specific heading or table in a clause file:
   ```
   .../32000-2-2020/clause12.html#H12.5.6.2
   .../32000-2-2020/clauseAnnexA.html#TableA.1
   ```

* The simulated "track changes" is achieved via inline `span class="new-text"` and `span class="deleted-text"`.

* The coloured popup tooltips (which state the pdf-issues Issue number and provide a clickable link back to GitHub e.g. "Issue #123") is achieved via `span class="new-tooltiptext"` and `span class="deleted-tooltiptext"`. Implement as an inline span within the surrounding span of the "track changes".

   ```html
   <span class="deleted-text">to-be-deleted<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/xx" target="_blank">Issue #xx</a></span></span>
   ```

* The "Last Modified" date at the end of each MD file needs to be changed manually (as this needs to be the edit time of substantive changes, not just when GH-Pages publishes everything)

* To create an interactive index to all modified Tables within a standard, use this Linux CLI:
   ```bash
   $ grep --color=auto "<caption" *.md | sed -e 's/\(.*\.md\):.*id=\"\(.*\)\">\(Table .*\)<\/caption>/<li><a href=\"\1#\2">\3<\/a><\/li>/'
   ```

* A local version of GH-Pages and Jekyll is used to check data entry and appearance before pushing to Github. See [GitHub Docs](https://docs.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll):

   ```
   bundle exec jekyll serve
   ```

* Visually check the rendered HTML appearance via [127.0.0.1:4000](127.0.0.1:4000) (default local jekyll URL)

* Currently in order to work correctly in the WordPress iframe on pdfa.org, `a` tags need to specific a `target=` attribute. Use `"github"` for the iframe on pdfa.org (for intra-site navigation links), `"_parent"` for links to other pdfa.org pages, or `"_blank"` for external links (e.g. to ISO)

* "View Page source" from inside various browsers (Edge, Chrome, FF, Safari for Mac users) and check for 'red' tags indicating issues (such as typos, missing or mismatched HTML tags, etc).

* Upload each of the local HTML files produced by jekyll (in `/docs/_site/clause`) to the [W3C HTML Validator](https://validator.w3.org/nu/#file).
   - Expect to see warnings regarding the use of heading levels since we are tring to mirror fragments of ISO standards.
   - There is also a warning regarding `element style not allowed as child of element section` caused by inclusion of the our `iso-style.html`. This is because using CSS won't override the Jekyll theme being used, but things work anyway so it can be ignored.

* Each pdf-issue is then closed in GitHub, possibly with any additional comment if any unexpected issue or edit arose in implementing the PDF TWG recommendations.

* Once pushed to GitHub, wait for the "successfully deployed" message and then also check [https://pdfa.org/pdf-issues](https://pdfa.org/pdf-issues).

* If there are any issues when incorporated into the iframes used by pdfa.org, also check the direct GitHub Jekkll site at [https://pdf-association.github.io/pdf-issues/](https://pdf-association.github.io/pdf-issues/)

# Scripting GitHub pdf-issues

For tweeting or other purposes, here are some basic starting points for automated bulk data extraction:

```bash
curl -s -H "Accept: application/vnd.github.v3.html+json" https://api.github.com/repos/pdf-association/pdf-issues/issues | jq '.[] | { number, state, title }'
curl -s -H "Accept: application/vnd.github.v3.html+json" https://api.github.com/repos/pdf-association/pdf-issues/issues?state=open\&labels=proposed%20solution | jq '.[] | { number, state, title }'

```