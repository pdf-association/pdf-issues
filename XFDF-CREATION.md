# XFDF Creation Process and Validation

The process for creating XFDF files is to use https://pdf-issues.pdfa.org/ as the master reference and manually apply each fix that has the ISO logo as a review comment annotation to a special reference copy of the master ISO PDF file of ISO 32000-2:2020 using a specific PDF application. When all editing is completed, some manual edits of the XFDF XML are the needed (via a text editor).

## Summary

* XFDF files are standardized according to [ISO 19444-1](https://www.pdfa.org/resource/iso-19444-xfdf/).

* the final XFDF file can be safely renamed as it does not have any significance.

* the way that content is organized in the XFDF is such that the viewing experience across multiple PDF viewers on various platforms from different vendors (and in either light or dark mode) is generally OK. Things are not done specifically for one vendor.  

* for deleted text, the body of the annotation is always empty. Red(ish) ([RGB = e52237](https://www.color-hex.com/color/e52237)) is used as the strikethrough color.

* for replaced text, the body of the annotation contains the new text with appropriate character formatting (bold, italic). Blue ([RGB = 0000FF](https://www.color-hex.com/color/0000FF)) is used for the strikethrough color.

* for new text, the body of the annotation contains the new text with appropriate character formatting (bold, italic).

* for bulk inserted text or Editor Notes, "Sticky Note" annotations are used. A yellow/gold is used ([RGB = FFD100](https://www.color-hex.com/color/ffd100)).

* sometimes an EDITOR NOTE, explanation or some specific additional instruction is also required - this is added to the body of the annotation. Text color is not changed to purple to match https://pdf-issues.pdfa.org as this does not adequately work across light/dark mode and different vendors.

* file attachments are also used, using the paperclip icon.

* there are limitations in what character formatting can be used in the annotation - it is assumed that end users will understand this limitation.

* all ISO approved annotations are checked as "Completed".

```bash
grep -o "state=\"[^\"]*\"" errata.xfdf | sort | uniq
```

* all annotations are "Locked".

```bash
 grep -o "flags=\"[^\"]*\"" errata.xfdf | sort | uniq
 ```

* The annotation `Subject` and `Title` are both set to be the same: the pdf-issues Issue number with the prefix "Issue #". If there are 2 issues, then the format is "Issue #xx and #yy" so that a grep for `#` can easily locate issue numbers:

```bash
grep -o "subject=\"[^\"]*\"" errata.xfdf | sort | uniq
grep -o "title=\"[^\"]*\"" errata.xfdf | sort | uniq
grep -o --color=none "title=\"[^\"]*\"" errata.xfdf | sort | uniq | grep --color=none -Po "(?<=\#)[0-9]*" | sort -n
```

* there are no URLs back to the GitHub pdf-issues repository as they do not work consistently across PDF viewers. End users can manually add an Issue number of interest to this URL https://github.com/pdf-association/pdf-issues/issues if they wish to research the reported issue.
    - e.g. https://github.com/pdf-association/pdf-issues/issues/12

* a single pdf-issue Issue may result in multiple annotations, which will all have the same Issue #.

## Manual Edits

* the XFDF XML must **NOT** be beautified, pretty-printed, or line-endings changed or it will fail with various PDF viewers! But if you want to understand it better try this:

```bash
xmllint --pretty 1 errata.xfdf
```

* ensure all `font-size:` is set to `11pt` - this seems to work best across PDF viewers and platforms

```bash
grep "font-size:[^;\"]*" errata.xfdf | sort | uniq
```

* matching Issue numbers with the MarkDown

```bash
grep -o --color=none "title=\"[^\"]*\"" errata.xfdf | sort | uniq | grep --color=none -Po "(?<=\#)[0-9]*" | sort -n
grep -ho --color=none "data-iss[a-z]*\=\"[a-z0-9,]*\"" 32000-2-2020/*.md | sort | uniq | grep -o --color=none "[0-9,]*"
```

* ensure that all colors are consistent (as per above - there should only be 3 colors used)

```bash
grep -o "color=\"#......\"" errata.xfdf | sort | uniq
```

* all `creationdate` and `date` tags are set to be the same (final date of publication of the XFDF)

* all user names are replaced with "PDF Association"

* the XFDF XML tags to the specific PDF used to edit/create the XFDF are manually removed after all edits.
    - This is normally the 3rd-last and 2nd-last lines of the XFDF file (`f` and `ids` tags).

* the final XFDF (after manual editing) is tested by:
    - checking consistency of the XML using the `grep` commands above
    - opening in various PDF applications and checking random pages with edits
    - using the iText XFDF Merging application: https://github.com/itext/xfdf-merger
