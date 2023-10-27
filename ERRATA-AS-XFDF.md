# Proposal for publishing resolved Issues as XFDF

## Concept

Provide end users (developers, software engineers, etc.) a far better experience of reliably understanding and identifying all resolved errata. This can be achieved by importing an FDF/XFDF file containing all resolved errata as PDF annotations and then which appear inline as various text markups onto their own licensed copy of ISO 32000-2:2020 that they
have acquired from ISO or their national body.

It is known that PDF specifications
are not read like books, but referenced randomly like a reference manual (_which is what it is!_).

# Background

Although the public PDF Association website https://pdf-issues.pdfa.org publishes
all resolved errata, it forms an independent source in a different format that
developers must remember to continually reference. It is also laborious and error prone for every single developer to constantly map between their ISO 32000-2:2020 PDF-based publication and the HTML+CSS errata website.

## Feedback from PDF meeting and experimentation

- keep errata text identical between https://pdf-issues.pdfa.org and XFDF/FDF at all times.

- visually style XFDF/FDF errata to match website (e.g. green text for new text, red for deletions).
   - viewer annotation highlighting is a viewer preference and not controllable via XFDF/FDF  

- for very long additions (such as https://pdf-issues.pdfa.org/32000-2-2020/clause14.html#H14.8.4.7.3),
 make these multiple smaller PDF annotations (e.g. 2 paragraphs per annotations).

- mentioning a pdf-issues Issue # is helpful, but making them clickable URLs is difficult and unreliable:
  - some annotations are specified to display `/Contents` (text string, no URL possible) while others use `/RC` (XFA rich text, which can have HTML tags).
  - support for clickable URLs in annotations also varies greatly between viewers  .

- different viewers choose to the many annotation fields differently.
  - For example: the annotation subject (`/S` key) is not shown in all PDF viewers.
  - however this can still be in the XFDF/FDF for those that do display it.

- the PDF TWG is against heavy use of pop-up annotations because they can be an annoying user experience, especially when a lot of edits (errata) are close-by.

- it is known that some national bodies (e.g. BSI, previously SA) add additional front pages as well
scaling and translating page content so a tool is required that can transform an
XFDF/FDF designed for a "master" ISO publication to suit whatever an national body might do.  
   - current ad-hoc experimentation shows that BSI adds 3 pages, scales content by 94% and requires 26 pt added to X values and 6pt subtracted from Y values (approx.!)

- iText have such a tool for XFDF (only, not FDF): https://github.com/itext/xfdf-merger

- there is no known FDF equivalent tool.

- thus the PDF TWG preferences XFDF over FDF going forward.

## Additional notes related to ISO Amendments

- ISO Amendment documents have to be _very_ short. As WG8 learned, if it is too long ISO has the right to not permit an Amendment.
   - _current expectation is less than 8-10 pages, including ISO front matter!_

- ISO Amendments require "location statements" prior to each fully reiterated errata. 
   - _this increases the length of an ISO Amendment_.

- ISO do not permit the pseudo "track changes" colored markup shown at https://pdf-issues.pdfa.org/ but insteasd require explicit location statements "_change X to Y_"
   - _this increases the length of an ISO Amendment_.

- ISO Amendments are **NOT** allowed to have a Table of Contents. This has been confirmed.
   - This is _unlike_ the original 1,000 page ISO 32000-2:2020 PDF and the utility ToCs published at the top of each HTML page for top level clauses to https://pdf-issues.pdfa.org (as well as a list of Tables that have been updated at https://pdf-issues.pdfa.org/32000-2-2020/) so navigating such a large number of errata will be extremely difficult!

- ISO Amendments are **not** free, unlike previous Technical Corrigenda.

- ISO Directives state can only do a maximum of 2 ISO Amendments per ISO publication.
