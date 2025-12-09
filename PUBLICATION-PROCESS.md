# Publication Process for resolved Issues

This is a short description of what happens after the PDF Association PDF TWG agrees that an issue resolution:

- `_config.yml` should not need changing.

- The `docs/index.md` is the main page but shouldn't need changing too often unless a new standard is being added.

- `docs/_data/data.yml` will also need updating if a new standard is added.

- Individual corrections are applied to the MD files below `docs/_clauses`.
   - Sub-folders are named after each ISO standard in the form `<iso-number>-<iso-part>-<year>`.
   - Each clause file in each sub-folder is named `clauseXXX.md`.

- Each ISO standard also has a specific landing page at `docs/_clauses/<iso-standard>/index.md`.
   - This should not need changing once created, as Liquid is used to generate the index to each top clause based on the file `docs/_data/data.yml`.
   - When creating a new standard, copy an existing file and just change the top matter. Data is pulled from `docs/_data/data.yml`.

- If a new `docs/_clauses/<iso-standard>/clauseXXX.md` MD file is added, then the `docs/_data/data.yml` will need updating to ensure the new clause occurs on the correct standard-specific language page, and in the correct order.

- All clause MD files have special Jekyll top matter which is required. The matter is used by Jekyll/Liquid to create indices, ToCs, set page title, page modification date, etc.

- Edits are done manually with a lot of manual HTML formatting and fiddling to get the closest possible appearance to a "track changes" of ISO 32000-2:2020.

- Just like in ISO 32000-2:2020, keys are **bold** and values are _italic_.
   - No attempt is to made to make the table columns retain their same width in the relevant standard.

- We fully respect ISO copyright so only small amounts of surrounding text are used. Typically just the paragraph in question so that the track change is clearly understandable with some context and is easily and clearly locatable within the relevant ISO standard. Headings (clause titles) and Table numbers are **always** used to aid location.

- Ellipsis (...) paragraphs `<p>...</p>` are used to visually indicate missing stuff from ISO standards. Otherwise the resolutions look like adjacent paragraphs when they're not!

- The track-changes styling is implemented via `assets/iso-style.css`.

- Edits are currently split into separate clause pages based on top level clauses in each ISO standard.

- The heading `<hX>` tag in the `docs/_clause/<iso-standard>/clauseXXX.md` matches the nearest heading level in the ISO standard for each resolutions. If the heading title is something highly generic (e.g. X.Y.Z General) then also add the next highest heading (e.g. X.Y Topic) is added. This means heading numbers are not contiguous (did someone say "document fragment"?)!!

- Anchor IDs are added to all headings (level 2 and greater) and all Table captions:
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

- URLs can then be used to jump to a specific heading or table in a clause file:
   ```
   .../32000-2-2020/clause12.html#H12.5.6.2
   .../32000-2-2020/clauseAnnexA.html#TableA.1
   ```

- The simulated "track changes" is achieved via HTML5 `del` and `ins` tags, styled by CSS in `assets/iso-style.css`.

- Editor notes use `class="editornote"` and can use `ins` or `del` tags as necessary to link to the edits for an issue.

- Descriptive location statements (where abouts in the relevant standard each specific edit is made) are needed for ISO Amendments. These use `<p class="location">...</p>` and tend to be of the form "Change Table XX as follows:", "Delete the third paragraph below ...", "Insert a new NOTE above ...", etc.

- Each `clauseXXX.md` file needs to start with the following structure: a local ToC for just this clause (if required); the ISO stylesheet, the hidden `div` used to display the popups, a fake H1 for the start of the clause:

```html
<ul>
	<li><a href="#Hx.y.z">x.y.z AAA BBB CCC</a></li>
</ul>
<hr>;

<div class="isostyle">
<div class="fixedpopup" id="issuelink">
	Issue #xxxx
</div>

<p class="fake-h1">{{ page.title }}</p>

<h2 id="H4.1">4.1 General</h2>
```

- The popup tooltips which state the pdf-issues Issue number and provide clickable URLs back to GitHub (e.g. "Issue #12") are achieved via `onMouseEnter` JavaScript that reads the custom attribute `data-issue` on the HTML5 `del` and `ins` tags. `del` tags occur first, then `ins` for changes on existing text. For changes with multiple Issues, comma separate the issue numbers (e.g. `issue="3,5,7"`). If the Errata is ISO approved, then set the custom attribute `data-iso` to the string `"approved"`. The JavaScript and CSS styling will then be merged by Jeykll.

   ```html
   <del onMouseEnter="mouseEnter(this)" data-issue="12">to be deleted</del> ... <ins onMouseEnter="mouseEnter(this)" data-issue="34">to be inserted</ins>
   <del onMouseEnter="mouseEnter(this)" data-issue="12" data-iso="approved">to be deleted</del> ... <ins onMouseEnter="mouseEnter(this)" data-issue="34" data-iso="approved">to be inserted</ins>
   ```

- It is *very strongly* recommended that each edit, demarcated by `<del ... </del>` and `<ins ... </ins>` are each on a single line by themselves. This simplifies greps, sed, etc.

- It is *required* that by `<del ... </del>` and `<ins ... </ins>` tags are entirely on the same line and not split across lines. This allows scripted updating of the ISO approval status.

- To check the ISO status of each errata, use the following `grep` - if `data-iso="approved"` is shown then it is ISO approved; if is not shown then it is not:

```bash
grep -o "data-[a-z]*\=\"[a-z0-9,]*\"" *.md
```
- To update the ISO status of errata, do a search and replace on `data-issue"123"` with `data-issue"123" data-iso="approved"` or `data-issue"12,34"` with `data-issue"12,34" data-iso="approved,approved"`. The custom attribute `data-iso` must be the same length as the `data-issue` custom attribute!

- The "Last Modified" in the top Liquid metadata of each MD file needs to be changed manually (as this needs to be the edit time of substantive changes)

- To create an interactive index to all modified Tables within a standard, use this Linux CLI:
   ```bash
   $ grep --color=auto "<caption" *.md | sed -e 's/\(.*\)\.md:.*id=\"\(.*\)\">\(Table .*\)<\/caption>/<li><a href=\"\1.html#\2">\3<\/a><\/li>/'
   ```

- Each clause MD file also has a local index to subclauses with corrections. This index occurs before `<div class="iso-style">` so it is sytled differently. This is done by running the following Linux CLI against each clause MD file followed by a bit of hand editing:
   ```bash
   grep --color=auto -H "<h[2-9]" clauseXX.md | sed -e 's/^\(.*\)\.md:<h\([2-9]\) id=\"\(.*\)\">\(.*\)<\/h.>/\2 <li><a href=\"\1#\3\">\4<\/a>/'
   ```

- A local version of GitHub-Pages and Jekyll is used to check data entry and appearance before pushing to Github. See [GitHub Docs](https://docs.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll). Current environment is Windows with Ruby 3.2.1, gem 3.4.8 and bundler 2.4.8 as well as the latest version of all gems:

   ```bash
   bundle exec jekyll serve
   
   # Or if things are going wrong...
   bundle exec jekyll serve --safe --trace --verbose
   ```

- Visually check the rendered HTML appearance via [127.0.0.1:4000](127.0.0.1:4000) (default local jekyll URL)

- "View Page source" from inside various browsers (Edge, Chrome, FireFox, Safari for Mac users) and check for 'red' tags indicating issues when viewing page source (such as typos, missing or mismatched HTML tags, etc).
   - Common mistakes are mistyped tags and missing closing tags, which means at the bottom of each page "\<div>" might be visible in the page content, or the local ToC has "\<ul>" or "\<li>" visible.

- Upload each of the local HTML files produced by jekyll (in `/docs/_site/clause`) to the [W3C HTML Validator](https://validator.w3.org/nu/#file).
   - Expected errors and warnings caused by Jekyll are:
       1. Errors (3): A link element must not appear as a descendant of a body element unless the link element has an itemprop attribute or has a rel attribute whose value contains dns-prefetch, modulepreload, pingback, preconnect, prefetch, preload, prerender, or stylesheet.
       2. Warning: Consider using the `h1` element as a top-level heading only (all `h1` elements are treated as top-level headings by many screen readers and other tools).

- Check for missing or mismatched HTML tag pairs. This is often shown as a `</div>` at the very bottom of a page, or other closing HTML tags appearing in content. Because of Jekyll the simplest way is to grep for HMTL open and closing tags and try to work out which tag is missing/incorrect... 

- Each pdf-issue is then closed in GitHub, possibly with any additional comment if any unexpected issue or edit arose in implementing the PDF TWG recommendations.

- Once pushed to GitHub, wait for the "successfully deployed" message in Slack and then also check [https://pdfa.org/pdf-issues](https://pdfa.org/pdf-issues).

- If there are any issues when incorporated into the iframes used by pdfa.org, also check the direct GitHub Jekkll site at [https://pdf-association.github.io/pdf-issues/](https://pdf-association.github.io/pdf-issues/)

- And don't forget to update the [Arlington PDF Model](https://github.com/pdf-association/arlington-pdf-model) for any required edits. This will be in the `tsv/latest` folder but also the XML and TSV file sets for earlier PDF versions.

# Making a subset of resolved errata for review by ISO

The goal is to create a subset of all closed Errata that are ready for ISO WG8 technical review ([using this query](https://github.com/pdf-association/pdf-issues/issues?q=is%3Aissue+is%3Aclosed+-label%3A%22ISO+approved%22+-label%3Awontfix)) that can be saved to PDF from a web browser using the equivalent of https://pdf-issues.pdfa.org. This relies on Jekyll and [iso-styles.css](assets/iso-style.css) `@media print` to produce something approximating an MSWord "track changes" document. Once the PDF is exported from a browser (_Chrome and FireFox are slightly different!_), then those same Errata need to be re-labelled `ISO submitted` ([this query](https://github.com/pdf-association/pdf-issues/issues?q=is%3Aissue+is%3Aclosed+label%3A%22ISO+submitted%22)) and the master MD files have `data-iso="submitted"` to the appropriate `<del` or `<ins` opening tag. 

```bash
# Make sure all errata have a data-iso="submitted" or data-iso="approved" attribute.
# Any later errata resolutions by the PDF Association PDF TWG will not have a data-iso attribute.
grep -o "data-issue=\"[0-9,]*\"[^>]*>" clauseXX.md
```

Once appproved by ISO with possible tweaks to wording, etc. then those Errata need to be re-labelled `ISO approved` in GitHub ([this query](https://github.com/pdf-association/pdf-issues/issues?q=is%3Aissue+is%3Aclosed+label%3A%22ISO+approved%22+)) and the master MD files have `data-iso="approved"` to the appropriate `<del` or `<ins` opening tag. 

All resolved Errata are in the closed state in GitHub. Errata that are labelled "Won't fix" or are already labelled "ISO approved" must also be ignored.

```bash
cd ./docs

# We don't care about index.md which is just convenience for web navigation
rm 32000-2-2020/index.md

# List the Errata numbers that will be include - confirm with GitHub browser query
curl -s -H "Accept: application/vnd.github+json" https://api.github.com/search/issues?q=is:closed+is:issue+-label:wontfix,\"ISO%20approved\"+repo:pdf-association/pdf-issues\&per_page=90 | jq ".items[] | .number"

# Find out the ISO 32000-2:2020 clauses - any clause NOT included can be deleted
curl -s -H "Accept: application/vnd.github+json" https://api.github.com/search/issues?q=is:closed+is:issue+-label:wontfix,\"ISO%20approved\"+repo:pdf-association/pdf-issues\&per_page=90 | jq ".items[] | .number" | sed -re "s/^([0-9]+)/grep --files-with-matches 'data-issue=\\\\\"[0-9,]\*\1' .\/32000-2-2020\/\*.md/" > clauses.sh
./clauses.sh | sort -u

# Manually delete clauses that are NOT relevant to errata for ISO review
ls 32000-2-2020/
rm 32000-2-2020/xxxx.md

# For each clause, work out which edits need to be kept and then manually delete ALL OTHER EDITS in each MD file.
# Repeat the following commands for each clause.
curl -s -H "Accept: application/vnd.github+json" https://api.github.com/search/issues?q=is:closed+is:issue+-label:wontfix,\"ISO%20approved\"+repo:pdf-association/pdf-issues\&per_page=90 | jq ".items[] | .number" | sed -re "s/^([0-9]+)/grep --with-filename --line-number 'data-issue=\\\\\"[0-9,]\*\1' .\/32000-2-2020\/clauseXX.md/" > clauseXX.sh
./clauseXX.sh

# From ./docs folder
bundle install
bundle exec jekyll serve
```


# Scripting GitHub pdf-issues

For tweeting or other purposes, here are some basic starting points for automated bulk data extraction:

```bash
curl -s -H "Accept: application/vnd.github.v3.html+json" https://api.github.com/repos/pdf-association/pdf-issues/issues | jq '.[] | { number, state, title }'
curl -s -H "Accept: application/vnd.github.v3.html+json" https://api.github.com/repos/pdf-association/pdf-issues/issues?state=open\&labels=proposed%20solution | jq '.[] | { number, state, title }'

```
