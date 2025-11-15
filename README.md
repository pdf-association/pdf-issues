# PDF Specification Issues

![PDF support](https://img.shields.io/badge/PDF-1.x%2C2.0-blue)
&nbsp;&nbsp;&nbsp;
![PDF subsets](https://img.shields.io/badge/PDF%20subsets-PDF%2FA%2CPDF%2FUA%2CPDF%2FX%2CPDF%2FVT%2CPDF%2FR-blue)
&nbsp;&nbsp;&nbsp;
![LinkedIn](https://img.shields.io/static/v1?style=social&label=LinkedIn&logo=linkedin&message=PDF-Association)
&nbsp;&nbsp;&nbsp;
![Twitter Follow](https://img.shields.io/twitter/follow/PDFAssociation?style=social)
&nbsp;&nbsp;&nbsp;
![YouTube Channel Subscribers](https://img.shields.io/youtube/channel/subscribers/UCJL_M0VH2lm65gvGVarUTKQ?style=social)

Get your [sponsored copy of ISO 32000-2 or PDF/UA-2 now](https://pdfa.org/sponsored-standards/)! Includes industry and ISO-approved errata and various ISO PDF 2.0 extensions.

## Stats

![Open Errata](https://img.shields.io/github/issues/pdf-association/pdf-issues)
&nbsp;&nbsp;&nbsp;
![Closed Errata](https://img.shields.io/github/issues-closed-raw/pdf-association/pdf-issues)
&nbsp;&nbsp;&nbsp;
![ISO 32000-2 Amd1](https://img.shields.io/github/issues-closed-raw/pdf-association/pdf-issues/ISO%2032000-2%20Amd1)
&nbsp;&nbsp;&nbsp;
![ISO Approved Errata](https://img.shields.io/github/issues-closed-raw/pdf-association/pdf-issues/ISO%20approved)
&nbsp;&nbsp;&nbsp;
![ISO Submitted Errata](https://img.shields.io/github/issues-closed-raw/pdf-association/pdf-issues/ISO%20submitted)

## About

This public GitHub repository is hosted by the [PDF Association](https://www.pdfa.org) and
provides every stakeholder a means of openly reporting errata against any PDF specification, including ISO publications and certain PDF Association industry specifications. Errata are resolved via consensus in PDF Association [Technical Working Groups](https://pdfa.org/community/) (*open to members*) and published at [https://pdf-issues.pdfa.org/](https://pdf-issues.pdfa.org/). For ISO publications, these industry resolutions are passed to the [relevant ISO working group](https://www.pdfa.org/iso-status/) for later ratification.

All issues in PDF specifications are important, from minor typos and formatting issues, to
larger ambiguous, unclear or apparently contradictory statements. By reaching consensus on resolutions as an industry,
PDF interoperability and implementation reliability can be improved.

The current set of resolved errata are presented as
<span style="background-color:lightyellow;color:green;text-decoration-style:double;text-decoration-color:green;">additions</span>,
<span style="background-color:seashell;color:darkred;text-decoration:line-through;text-decoration-color:red;">deletions</span> or
<span style="font-weight:bold;color:purple;background-color:snow;text-decoration initial">Editor Notes</span>
to the published wording in the relevant ISO standard organized by clause number.
GitHub Issue numbers will appear as popup tooltips when hovering over changes and refer back to
<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aclosed+label=%22proposed+solution%22" target="_blank">
closed GitHub pdf-issues</a>.

* If a small blue ISO logo is also shown ![ISO approved logo](docs/assets/Logo-ISO-small.png), then that errata has been approved by both the PDF Association's appropriate TWG and the appropriate [ISO working groups responsible for PDF](https://www.pdfa.org/iso-status/).

* If a small gray ISO logo is also shown ![ISO submitted logo](docs/assets/Logo-ISO-submitted-small.png), then that errata has been approved by the PDF Association's appropriate TWG and submitted to the appropriate ISO working group and is waiting for approval.

* If no ISO logo is shown then the errata has been resolved by a PDF Association [Technical Working Group](https://www.pdfa.org/community/) but has not yet been submitted to ISO for ratification.

Due to ISO copyright, only minimal surrounding text from the relevant ISO publication is provided that is sufficient to understand where the resolution is being applied.

Errata in the following PDF specifications are supported:

### Core PDF technologies

  <ul>
   <li>PDF 2.0 (<a href="https://www.pdfa.org/resource/iso-32000-pdf/" target="_blank">ISO 32000-2:2020</a>) - <a href="https://pdf-issues.pdfa.org/32000-2-2020/index.html"><i>Resolved errata</i></a>
   <ul>
     <li>
     ISO/TS 32001 <a href="https://www.pdfa.org/resource/iso-ts-32001/">Extensions to Hash Algorithm Support in PDF 2.0</a> - <a href="https://pdf-issues.pdfa.org/32001-2022/"><i>Resolved errata</i></a>
     </li>
     <li>ISO/TS 32002 <a href="https://www.pdfa.org/resource/iso-ts-32002">Extensions to Digital Signatures in PDF 2.0</a> - <a href="https://pdf-issues.pdfa.org/32002-2022/"><i>Resolved errata</i></a>
     </li>
     <li>ISO/TS 24064 <a href="https://pdfa.org/resource/iso-ts-24064/">RichMedia annotations with STEP AP 242 3D for PDF 2.0</a>
     </li>
     <li>ISO/TS 32003 <a href="https://pdfa.org/resource/iso-ts-32003-aes-gcm/">Adding support of AES-GCM in PDF 2.0</a>
     </li>
     <li>ISO/TS 32004 <a href="https://pdfa.org/resource/iso-ts-32004-integrity-protection/">Integrity protection in encrypted documents in PDF 2.0</a>
     </li>
     <li>ISO/TS 32005 <a href="https://pdfa.org/resource/iso-32005/">PDF 1.7 and 2.0 structure namespace inclusion in PDF 2.0</a> - <a href="https://pdf-issues.pdfa.org/32005-2023/"><i>Resolved errata</i></a>
     </li>
   </ul>
   </li>
   <li>ECMAScript for PDF 2.0 (<a href="https://www.pdfa.org/resource/iso-21757-ecmascript/" target="_blank">ISO 21757-1:2020</a>) - <a href="https://pdf-issues.pdfa.org/21757-1-2020/index.html"><i>Resolved errata</i></a></li>
   <li>XFDF 3.0 (<a href="https://www.pdfa.org/resource/iso-19444-xfdf/" target="_blank">ISO 19444-1:2019</a>)</li>
   <li>"<a href="https://pdfa.org/wtpdf/">Well-Tagged PDF v1.0</a>" - <i><a href="https://pdf-issues.pdfa.org/wtpdf-1/">Resolved errata</a></i></li>
   <li>"<a href="https://pdfa.org/declarations/">PDF Declarations</a>" - <i><a href="https://pdf-issues.pdfa.org/pdf-declarations/">Resolved errata</a></i></li>
  </ul>

### <a href="https://www.pdfa.org/resource/iso-19005-pdfa/" target="_blank">PDF/A (ISO 19005) - PDF for long-term preservation</a>

* PDF/A-4 (ISO 19005-4:2020) - <a href="https://pdf-issues.pdfa.org/19005-4-2020/index.html">*Resolved errata*</a>
* PDF/A-3 (ISO 19005-3:2012) - see <a href="https://www.pdfa.org/resource/technote-0010-clarifications-of-iso-19005-parts-1-3-for-developers-of-pdfa-creators-and-validators/" target="_blank">TechNote 0010</a>
* PDF/A-2 (ISO 19005-2:2011) - see <a href="https://www.pdfa.org/resource/technote-0010-clarifications-of-iso-19005-parts-1-3-for-developers-of-pdfa-creators-and-validators/" target="_blank">TechNote 0010</a>

* PDF/A-1 (ISO 19005-1:2005) - see <a href="https://www.pdfa.org/resource/pdfa-1-technical-notes/" target="_blank">PDF/A-1 Technical Notes</a> and <a href="https://www.pdfa.org/resource/technote-0010-clarifications-of-iso-19005-parts-1-3-for-developers-of-pdfa-creators-and-validators/" target="_blank">TechNote 0010</a>

### <a href="https://www.pdfa.org/resource/iso-15930-pdfx/" target="_blank">PDF/X (ISO 15930) - PDF for prepress digital data exchange</a>

* PDF/X-6 (ISO 15930-9:2020) - <a href="https://pdf-issues.pdfa.org/15930-9-2020/index.html">*Resolved errata*</a>
* PDF/X-5 (ISO 15930-8:2010)
* PDF/X-4 (ISO 15930-7:2010)
* PDF/X-3 (ISO 15930-6:2003)

### <a href="https://www.pdfa.org/resource/iso-16612-pdfvt/" target="_blank">PDF/VT (ISO 16612) - PDF for variable data &amp; transactional printing</a>

* PDF/VT-3 (ISO 16612-3:2020) - <a href="https://pdf-issues.pdfa.org/16612-3-2020/index.html">*Resolved Errata*</a>
* PDF/VT-2 (ISO 16612-2:2010)

### <a href="https://www.pdfa.org/resource/iso-14289-pdfua/" target="_blank">PDF/UA (ISO 14289) - PDF for universal accessibility</a>

* PDF/UA-1 (ISO 14289-1:2014)
* PDF/UA-2 (ISO 14289-2:2024)

### Other ISO PDF publications

* <a href="https://www.pdfa.org/resource/iso-23504-pdfr/" target="_blank">PDF/R-1 (ISO 23504-1:2020)- PDF for raster image transport and storage</a>

Errata on PDF 1.7 (ISO 32000-1:2008) and withdrawn ISO publications are **not** supported - refer to ISO 32000-2 instead.
The PDF Association maintains a [full list of all PDF-related ISO publications](https://www.pdfa.org/index-of-pdf-related-iso-publications/).

Not all resolutions proposed here are officially authorized by the [ISO working groups responsible for PDF](https://www.pdfa.org/iso-status/) and may get changed when reviewed by the ISO working group.

## A Simple Process

1. Open a new GitHub Issue. Clearly explain the mistake you have found in a PDF specification, or the feature you would like to see in a future version.
2. The community can discuss and contribute to open issues here in GitHub, and work towards a proposed resolution.
3. The PDF Association's [PDF Technical Working Group](https://www.pdfa.org/community/pdf-technical-working-group/) (TWG) will consider all input and reach a consensus for each proposed resolution. Issues related to PDF subset standards or specific technical topics may get delegated to other TWGs.
4. Each issue will be updated with the agreed resolution and then Closed by moderators once the resolution is published at [https://pdf-issues.pdfa.org/](https://pdf-issues.pdfa.org/).
5. At some later time, errata will be passed to the appropriate ISO working group for formal ratification.

A full list of all ISO and industry-agreed issue resolutions (as pseudo-markup) is actively maintained at [https://pdf-issues.pdfa.org/](https://pdf-issues.pdfa.org/).

## Directly referencing resolutions

Errata can always be referred by the appropriate GitHub issue numbers(s). Resolutions are published to a set of static URLs at [https://pdf-issues.pdfa.org/](https://pdf-issues.pdfa.org/) of the form `<standard-number>/clause<clause-number>.html`. Each of these resolution pages also includes anchor points for all Headings (`#Hx.y.z` anchors to heading X.Y.Z in the appropriate ISO standard) and Tables (`#TableXXX` anchors to Table XXX in the appropriate ISO standard). This allows very precise linkages to final resolution outcomes, without scrolling through long technical GitHub discussions.

For example:

* [https://pdf-issues.pdfa.org/21757-1-2020/](https://pdf-issues.pdfa.org/21757-1-2020/) links directly to every resolution in ISO 21757-1:2020 ECMAscript for PDF 2.0.
* [https://pdf-issues.pdfa.org/32000-2-2020/clauseAnnexQ.html](https://pdf-issues.pdfa.org/32000-2-2020/clauseAnnexQ.html) links directly to all resolutions in Annex Q *(normative) Method for determining transparency on a page* of ISO 32000-2:2020 (PDF 2.0).
* [https://pdf-issues.pdfa.org/32000-2-2020/clause12.html#H12.5.6.5](https://pdf-issues.pdfa.org/32000-2-2020/clause12.html#H12.5.6.5) links directly to all resolutions in ISO 32000-2:2020 (PDF 2.0) clause 12.5.6.5 *Link annotations*.
* [https://pdf-issues.pdfa.org/32000-2-2020/clause08.html#Table87](https://pdf-issues.pdfa.org/32000-2-2020/clause08.html#Table87) links directly to all resolutions in ISO 32000-2:2020 (PDF 2.0) Table 87 - *Additional entries specific to an image dictionary*.

## Legal

In contributing to this GitHub repository, you acknowledge that all content you share may be reproduced in whole or in part in future PDF Association publications, ISO standards or other deliverables. It is your responsibility in submitting such content to ensure that the agreement of any copyright holder has been obtained. More information about [ISO contribution processes can be found here](https://www.iso.org/publication/PUB100037.html).
