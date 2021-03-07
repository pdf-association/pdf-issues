# Publication Process for resolved Issues

This is a short description of what happens after the PDF Association PDF TWG agrees that an issue resolution:

* Edits are applied to the Markdown files in docs/_clauses. The docs/index.md is the main page but shouldn't need changing too often.

* Edits are done manually with a lot of manual HTML formatting and fiddling to get the closest possible appearance to a "track changes" of ISO 32000-2:2020.

* Just like in ISO 32000-2:2020, keys are **bold** and values are _italic_. No attempt is to made to make the table columns retain their same width as in ISO 32000-2:2020.

* We fully respect ISO copyright so only small amounts of surrounding text are used. Typically just the paragraph in question so that the track change is clearly understandable with some context and is easily and clearly locatable within ISO 32000-2. Headings (clause titles) and Table numbers are always used.

* Ellipsis (...) with breaks <br\\> are used to visually indicate missing stuff from ISO 32000-2:2020. Otherwise the resolutions look like adjacent paragraphs when they're not!

* The track-changes styling is implemented via _includes/iso-style.html which is an inline set of styles that are %-included into each _clause/ MarkDown file.

* Edits are currently split on top level (H1) clauses in ISO 32000. The MD files have some Jekyll magic at the top which allows them to be enumerated into a ToC from index.md. At some point this arbitrary decision may need to change... and that may be some work!

* The heading <hX> tag in the docs/_clause Markdown matches the nearest heading level in ISO 32000-2 for all resolutions. If the heading title is something highly generic (e.g. X.Y.Z General) then also add the next highest heading (e.g. X.Y Topic) is added.

* The simulated "track changes" is achieved via inline span class="new-text" and class="deleted-text".

* The popup tooltips (which state the pdf-issues Issue number e.g. "Issue #123") is achieved via class="new-tooltiptext" and class="deleted-tooltiptext". Implement as an inline span within the surrounding span of the "track changes".

* The "Last Modified" date at the end of each clause MD file needs to be changed manually (as this needs to be the edit time of substantive changes, not just trying to work around GH-Pages issues)

* A local version of GH-Pages and Jekyll is used to check data entry and appearance before pushing to Github:

```bundle exec jekyll serve```

* Visually check the rendered HTML appearance via [127.0.0.1:4000](127.0.0.1:4000) (default local jekyll URL)

* "View Page source" from inside various browsers (Edge, Chrome, FF, Safari for Mac users) and check for 'red' tags indicating issues (such as typos, missing or mismatched HTML tags, etc).

* Each pdf-issue is then closed in GitHub, possibly with any additional comment if any unexpected issue or edit arose in implementing the PDF TWG recommendations.

* Once pushed to GitHub, wait for the "successfully deployed" message and then also check [https://pdfa.org/pdf-issues](https://pdfa.org/pdf-issues). If there are any issues when incorporated into the iframes used by pdfa.org, also check the direct GitHub Jekkll site at [https://pdf-association.github.io/pdf-issues/](https://pdf-association.github.io/pdf-issues/)

# Scripting GitHub pdf-issues

For tweeting or other purposes, here are some basic starting points for automated bulk data extraction:

```
curl -s -H "Accept: application/vnd.github.v3.html+json" https://api.github.com/repos/pdf-association/pdf-issues/issues | jq '.[] | { number, state, title }'
curl -s -H "Accept: application/vnd.github.v3.html+json" https://api.github.com/repos/pdf-association/pdf-issues/issues?state=open\&labels=proposed%20solution | jq '.[] | { number, state, title }'

```