# PDF 2.0 Issues

![PDF support](https://img.shields.io/badge/PDF-1.7%2C2.0-blue)
&nbsp;&nbsp;&nbsp;
![PDF subsets](https://img.shields.io/badge/PDF%20subsets-PDF%2FA%2CPDF%2FX%2CPDF%2FVT%2CPDF%2FR-blue)
&nbsp;&nbsp;&nbsp;
![LinkedIn](https://img.shields.io/static/v1?style=social&label=LinkedIn&logo=linkedin&message=PDF-Association)
&nbsp;&nbsp;&nbsp;
![Twitter Follow](https://img.shields.io/twitter/follow/PDFAssociation?style=social)
&nbsp;&nbsp;&nbsp;
![YouTube Channel Subscribers](https://img.shields.io/youtube/channel/subscribers/UCJL_M0VH2lm65gvGVarUTKQ?style=social)

## Stats

![Open Errata](https://img.shields.io/github/issues/pdf-association/pdf-issues)
&nbsp;&nbsp;&nbsp;
![Closed Errata](https://img.shields.io/github/issues-closed-raw/pdf-association/pdf-issues)
&nbsp;&nbsp;&nbsp;
![ISO Approved Errata](https://img.shields.io/github/issues-closed-raw/pdf-association/pdf-issues/ISO%20approved)
&nbsp;&nbsp;&nbsp;
![ISO Submitted Errata](https://img.shields.io/github/issues-closed-raw/pdf-association/pdf-issues/ISO%20submitted)

## About

This public GitHub repository "pdf-issues" is hosted by the <a href="https://www.pdfa.org">PDF Association</a> and
provides all developers a means of openly reporting errata against ISO PDF related standards for review and resolution by industry and ISO experts.
All issues in ISO PDF related standards are important, from minor typos and formatting issues, to
larger ambiguous, unclear or apparently contradictory statements. By reaching consensus on resolutions as an industry,
PDF interoperability and implementation reliability will be improved.

The current set of resolved errata are presented as
<span style="background-color:lightyellow;color:green;text-decoration-style:double;text-decoration-color:green;">additions</span>,
<span style="background-color:seashell;color:darkred;text-decoration:line-through;text-decoration-color:red;">deletions</span> or
<span style="font-weight:bold;color:purple;background-color:snow;text-decoration initial">editor notes</span>
to the published wording in the relevant ISO standard organized by clause number.
GitHub Issue numbers will appear as popup tooltips when hovering over changes and refer back to
<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aclosed+label%3A%22proposed+solution%22" target="_blank">
closed GitHub pdf-issues</a>. 

* If a small blue ISO logo is also shown ![ISO approved logo](docs/assets/Logo-ISO-small.png), then that errata has been approved by both the PDF Association's appropriate TWG and the appropriate [ISO working groups responsible for PDF](https://www.pdfa.org/iso-status/). 
    - For ISO 32000-2:2020 (PDF 2.0), this means the resolution will be included in the forthcoming [Amendment 1](https://www.iso.org/standard/85145.html).


* If a small gray ISO logo is also shown ![ISO submitted logo](docs/assets/Logo-ISO-submitted-small.png), then that errata has been approved by the PDF Association's appropriate TWG and submitted to the appropriate ISO working group and is waiting for approval. 
    - For ISO 32000-2:2020 (PDF 2.0), these errata have been technically approved by ISO TC 171 SC 2 WG 8, but do not yet have an identified ISO document.


* If no ISO logo is shown then the errata has been resolved by the PDF Association's [PDF Technical Working Group](https://www.pdfa.org/community/pdf-technical-working-group/) but has not yet been submitted to ISO for ratification.


Due to ISO copyright, only minimal surrounding text from the relevant ISO standard is provided that is sufficient to understand how the resolution is being applied.

Errata in the following published ISO publications are supported:

### Core PDF technologies
  <ul>
   <li>PDF 2.0 (<a href="https://www.pdfa.org/resource/iso-32000-pdf/" target="_blank">ISO 32000-2:2020</a>) - <a href="https://pdf-issues.pdfa.org/32000-2-2020/index.html"><i>Resolved errata</i></a></li>
   <li>ECMAScript for PDF 2.0 (<a href="https://www.pdfa.org/resource/iso-21757-ecmascript/" target="_blank">ISO 21757-1:2020</a>) - <a href="https://pdf-issues.pdfa.org/21757-1-2020/index.html"><i>Resolved errata</i></a></li>
   <li>XFDF 3.0 (<a href="https://www.pdfa.org/resource/iso-19444-xfdf/" target="_blank">ISO 19444-1:2019</a>)</li>
  </ul>

### <a href="https://www.pdfa.org/resource/iso-19005-pdfa/" target="_blank">PDF/A (ISO 19005) - PDF for long-term preservation</a>
  <ul>
   <li>PDF/A-4 (ISO 19005-4:2020) - <a href="https://pdf-issues.pdfa.org/19005-4-2020/index.html"><i>Resolved errata</i></a></li>
   <li>PDF/A-3 (ISO 19005-3:2012) - see <a href="https://www.pdfa.org/resource/technote-0010-clarifications-of-iso-19005-parts-1-3-for-developers-of-pdfa-creators-and-validators/" target="_blank">TechNote 0010</a></li>
   <li>PDF/A-2 (ISO 19005-2:2011) - see <a href="https://www.pdfa.org/resource/technote-0010-clarifications-of-iso-19005-parts-1-3-for-developers-of-pdfa-creators-and-validators/" target="_blank">TechNote 0010</a></li>
   <li>PDF/A-1 (ISO 19005-1:2005) - see <a href="https://www.pdfa.org/resource/pdfa-1-technical-notes/" target="_blank">PDF/A-1 Technical Notes</a> and <a href="https://www.pdfa.org/resource/technote-0010-clarifications-of-iso-19005-parts-1-3-for-developers-of-pdfa-creators-and-validators/" target="_blank">TechNote 0010</a></li>
  </ul>

### <a href="https://www.pdfa.org/resource/iso-15930-pdfx/" target="_blank">PDF/X (ISO 15930) - PDF for prepress digital data exchange</a>
   <ul>
    <li>PDF/X-6 (ISO 15930-9:2020) - <a href="https://pdf-issues.pdfa.org/15930-9-2020/index.html"><i>Resolved errata</i></a></li>
    <li>PDF/X-5 (ISO 15930-8:2010)</li>
    <li>PDF/X-4 (ISO 15930-7:2010)</li>
    <li>PDF/X-3 (ISO 15930-6:2003)</li>
   </ul>

### <a href="https://www.pdfa.org/resource/iso-16612-pdfvt/" target="_blank">PDF/VT (ISO 16612) - PDF for variable data &amp; transactional printing</a>
   <ul>
    <li>PDF/VT-3 (ISO 16612-3:2020) - <a href="https://pdf-issues.pdfa.org/16612-3-2020/index.html"><i>Resolved Errata</i></a></li>
    <li>PDF/VT-2 (ISO 16612-2:2010)</li>
   </ul>

### <a href="https://www.pdfa.org/resource/iso-14289-pdfua/" target="_blank">PDF/UA (ISO 14289) - PDF for universal accessibility</a>
   <ul>
    <li>PDF/UA-1 (ISO 14289-1:2014)</li>
   </ul>

### Other ISO PDF publications
  <ul>
   <li><a href="https://www.pdfa.org/resource/iso-23504-pdfr/" target="_blank">PDF/R-1 (ISO 23504-1:2020)- PDF for raster image transport and storage</a></li>
  </ul>

<p>Errata on PDF 1.7 (ISO 32000-1:2008) and withdrawn ISO publications are <b>not</b> supported - refer to ISO 32000-2 instead.
The PDF Association maintains a <a href="https://www.pdfa.org/index-of-pdf-related-iso-publications/">full list of all PDF-related ISO publications</a>.</p>

Not all resolutions proposed here are officially authorized by the [ISO working groups responsible for PDF](https://www.pdfa.org/iso-status/) and may get changed when reviewed by the ISO working group.

## A Simple Process
1. Open a new GitHub Issue. Clearly explain the mistake you have found in a published ISO PDF 2.0-based standard, or the feature you would like to see in a future version.
2. The community can discuss and contribute to open issues here in GitHub, and work towards a proposed resolution.
3. The PDF Association's [PDF Technical Working Group](https://www.pdfa.org/community/pdf-technical-working-group/) (TWG) will consider all input and reach a consensus for each proposed resolution. Issues related to PDF subset standards may also get passed on to other TWGs.
4. Each issue will be updated with the agreed resolution and then Closed by moderators once the resolution is published at [https://pdf-issues.pdfa.org/](https://pdf-issues.pdfa.org/).
5. At some later time, some errata may be passed to the appropriate ISO working group for formal ratification.

A full list of all ISO and industry-agreed issue resolutions (as pseudo-markup) is actively maintained at [https://pdf-issues.pdfa.org/](https://pdf-issues.pdfa.org/).

## Directly referencing resolutions

Errata can always be referred by the appropriate GitHub issue numbers(s). Resolutions are published to a set of static URLs at [https://pdf-issues.pdfa.org/](https://pdf-issues.pdfa.org/) of the form `<standard-number>/clause<clause-number>.html`. Each of these resolution pages also includes anchor points for all Headings (`#Hx.y.z` anchors to heading X.Y.Z in the appropriate ISO standard) and Tables (`#TableXXX` anchors to Table XXX in the appropriate ISO standard). This allows very precise linkages to final resolution outcomes, without scrolling through long technical GitHub discussions.

For example:

- [https://pdf-issues.pdfa.org/21757-1-2020/](https://pdf-issues.pdfa.org/21757-1-2020/) links directly to every resolution in ISO 21757-1:2020 ECMAscript for PDF 2.0.
- [https://pdf-issues.pdfa.org/32000-2-2020/clauseAnnexQ.html](https://pdf-issues.pdfa.org/32000-2-2020/clauseAnnexQ.html) links directly to all resolutions in Annex Q *(normative) Method for determining transparency on a page* of ISO 32000-2:2020 (PDF 2.0).
- [https://pdf-issues.pdfa.org/32000-2-2020/clause12.html#H12.5.6.5](https://pdf-issues.pdfa.org/32000-2-2020/clause12.html#H12.5.6.5) links directly to all resolutions in ISO 32000-2:2020 (PDF 2.0) clause 12.5.6.5 *Link annotations*.
- [https://pdf-issues.pdfa.org/32000-2-2020/clause08.html#Table87](https://pdf-issues.pdfa.org/32000-2-2020/clause08.html#Table87) links directly to all resolutions in ISO 32000-2:2020 (PDF 2.0) Table 87 - *Additional entries specific to an image dictionary*.

## Legal
In contributing to this GitHub repository, you acknowledge that all content you share may be reproduced in whole or in part in future PDF Association publications, ISO standards or other deliverables. It is your responsibility in submitting such content to ensure that the agreement of any copyright holder has been obtained. More information about ISO contribution processes can be found [here](https://www.iso.org/publication/PUB100037.html).
