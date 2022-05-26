# XFDF Creation Process and Validation

The process for creating XFDF files is to use https://pdf-issues.pdfa.org/ as the master reference and manually apply each fix that has the ISO logo as a review comment annotation to a special reference copy of the master ISO PDF file of ISO 32000-2:2020 using a specific PDF application. When all editing is completed, some manual edits of the XFDF XML are the needed (via a text editor).

## Summary

* XFDF files are standardized according to [ISO 19444-1](https://www.pdfa.org/resource/iso-19444-xfdf/).

* the final XFDF file can be safely renamed as it does not have any significance.

* the way that content is organized in the XFDF is such that the viewing experience across multiple PDF viewers on various platforms from different vendors is generally OK. Things are not done specifically for one vendor.  

* for deleted text, the body of the annotation is always empty. Red is used as the strikethrough color.

* for replaced text, the body of the annotation contains the new text with appropriate character formatting (bold, italic).

* for new text, the body of the annotation contains the new text with appropriate character formatting (bold, italic).

* for bulk inserted text, "Sticky Note" annotations are used.

* sometimes an EDITOR NOTE, explanation or some specific additional instruction is also required - this is added to the body of the annotation.

* there are limitations in what character formatting can be used in the annotation - it is assumed that end users will understand this limitation.

* all ISO approved annotations are checked as "Completed".

```bash
grep -o "state=\"[^\"]*" errata.xfdf | sort | uniq
```

* all annotations are "Locked".

```bash
 grep -o "flags=\"[^\"]*" errata.xfdf | sort | uniq
 ```

* The annotation `Subject` and `Title` are both set to be the same: the pdf-issues Issue number with the prefix "Issue #". If there are 2 issues, then the format is "Issue #xx and #yy" so that a grep for `#` can easily locate issue numbers:

```bash
grep -o "subject=\"Issue #[^\"]*" errata.xfdf | sort | uniq
grep -o "title=\"Issue #[^\"]*" errata.xfdf | sort | uniq
```

* there are no URLs in the XFDF as they do not work reliably or consistently in PDF viewers. End users can manually add an Issue number of interest to this URL https://github.com/pdf-association/pdf-issues/issues if they wish to research the reported issue.
    - e.g. https://github.com/pdf-association/pdf-issues/issues/12

* a single pdf-issue Issue may result in multiple annotations, which will all have the same Issue #.

## Manual Edits

* the XFDF XML must **NOT** be beautified, pretty-printed, or line-endings changed or it will fail with various PDF viewers! But if you want to understand it better try this:

```bash
xmllint --pretty 1 errata.xfdf
```

* all `creationdate` and `date` tags are set to be the same (final date of publication of the XFDF)

* any user names are replaced with "PDF Association"

* the XFDF XML tags to the specific PDF used to edit/create the XFDF are manually removed after all edits.
    - This is normally the 3rd-last and 2nd-last lines of the XFDF file (`f` and `ids` tags).

* the final XFDF (after manual editting) is tested by:
    - checking consistency of the XML using the `grep` commands above
    - opening in various PDF applications and checking random pages with edits
    - using the iText XFDF Merging application: https://github.com/itext/xfdf-merger
