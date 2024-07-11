---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: Annex L
title: (normative) Parent-child relationships between the standard structure elements in the standard structure namespace for PDF 2.0
modified: 11 July 2022
---

<ul class="noprint">
</ul>
<hr>

<link rel="stylesheet" href="../assets/iso-style.css">
<div class="isostyle">
<div class="fixedpopup" id="issuelink">
    Issue #xxxx
</div>


<p class="fake-h1">{{ page.clause }}. {{ page.title }}</p>

<p class="location">Change the third paragraph as follows:</p>

<p>
An informative matrix representation of Table L.2 is attached to the PDF of this document as "ISO32000-2_AnnexL_matrix-version2020.pdf" and
in machine-readable form, as <ins onMouseEnter="mouseEnter(this)" data-issue="64" data-iso="approved">
<a href="https://www.pdfa.org/norm-refs/ISO32000-2_AnnexL_matrix-version2020-amd1.xlsx">"ISO32000-2_AnnexL_matrix-version2020-amd1.xlsx</a></ins>."
</p>

<p class="location">Correct Table Annex L.2 and associated attachments as follows:</p>

<p class="editornote">EDITOR NOTE: as a result of <a href="https://github.com/pdf-association/pdf-issues/issues/83">Errata #83</a> modify Table Annex L.2 so that <b>Table</b> is now indicated as a valid child of <b>P</b> with a
<ins onMouseEnter="mouseEnter(this)" data-issue="83" data-iso="approved">"0..<i>n</i>"</ins> 
relationship and, in the <b>Table</b> section, <b>P</b> is listed as a valid parent also with a 
<ins onMouseEnter="mouseEnter(this)" data-issue="83" data-iso="approved">"0..<i>n</i>"</ins> relationship. 
The embedded PDF and spreadsheet data are also corrected.
</p>

<p class="editornote">EDITOR NOTE: as a result of <a href="https://github.com/pdf-association/pdf-issues/issues/440">Errata #440</a> modify Table Annex L.2 such that where Structure Type is <b>WP</b> and Child is <b>Figure</b> and where Structure Type is <b>Figure</b> and Parent is <b>WP</b> the undefined cell value <del onMouseEnter="mouseEnter(this)" data-issue="440">"c"</del> 
is corrected to be a <ins onMouseEnter="mouseEnter(this)" data-issue="440">"0..<i>n</i>"</ins> relationship. 
The embedded PDF and spreadsheet data are also corrected.
</p>

<p class="location">Add a footnote to the first data row in Table Annex L.2 as follows:</p>

<table>
  <caption id="TableAnnexL.2">Table Annex L.2 -Parent-child relationships between the standard structure elements in the standard structure namespace for PDF 2.0</caption>
  <thead>
    <tr>
      <th>Structure Type</th>
      <th>Children<br>Occ.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Structure Type</th>
      <th>Parents<br>Occ.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Structure Type</th>
    </tr>
  </thead>
  <tbody>
    <tr>
     <td>StructTreeRoot <ins onMouseEnter="mouseEnter(this)" data-issue="349"><sup>1</sup></ins></td>
     <td>1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Document</td>
     <td></td>
    </tr>
    <tr>
     <td>...</td>
     <td>...</td>
     <td>...</td>
    </tr>
  </tbody>
</table>

<p><ins onMouseEnter="mouseEnter(this)" data-issue="349">
<sup>1</sup> StructTreeRoot refers to the structure tree root dictionary (see "Table 354 — Entries in the structure tree root") and is not the name of a structure element.
</ins></p>

</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
