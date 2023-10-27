---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: Annex F
title: (normative) Linearized PDF
modified: 15 September 2023
---

<ul class="noprint">
    <li>F.3 Linearized PDF document structure
     <ul>
      <li><a href="#HF.3.2">F.3.2 Header (Part 1)</a>
      </li>
      <li><a href="#HF.3.3">F.3.3 Linearization parameter dictionary (Part 2)</a>
      </li>
     </ul>
    </li>
</ul>
<hr>

<link rel="stylesheet" href="../assets/iso-style.css">
<div class="isostyle">
<div class="fixedpopup" id="issuelink">
    Issue #xxxx
</div>

<p class="fake-h1">{{ page.clause }}. {{ page.title }}</p>

<h2 id="HF.3">F.3 Linearized PDF document structure</h2>

<p class="location">Change the first paragraph as follows:</p>

<p>
The Linearized PDF file shall begin with the standard header line (see 7.5.2, "File header"). Linearization is independent of PDF version number and may be applied to any PDF file of version 
<del onMouseEnter="mouseEnter(this)" data-issue="331">1.1</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="331">1.2</ins> 
or greater.
</p>

<p>...</p>


<h3 id="HF.3.2">F.3.2 Header (Part 1)</h3>

<h3 id="HF.3.3">F.3.3 Linearization parameter dictionary (Part 2)</h3>

<p class="location">Change Table F.1 as follows:</p>

<table>
  <caption id="TableA.1">Table F.1 - Entries in the linearization parameter dictionary</caption>
  <tr>
    <th>Parameter</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Linearized</b></td>
    <td>number</td>
    <td>
      <p>(<i>Required</i>) A version identification for the linearized format.
      <ins onMouseEnter="mouseEnter(this)" data-issue="153" data-iso="approved">As usual, a change in the integer part
      indicates an incompatible change in the linearized format. A change in the fractional part
      indicates an upward-compatible change. The current version is 1.0.</ins>
      </p>
    </td>
  </tr>
</table>

</div>

<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
