---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: Annex F
title: (normative) Linearized PDF
modified: 7 June 2024
---

<ul class="noprint">
    <li>F.3 Linearized PDF document structure
     <ul>
      <li><a href="#HF.3.2">F.3.2 Header (Part 1)</a>
      </li>
      <li><a href="#HF.3.3">F.3.3 Linearization parameter dictionary (Part 2)</a>
      </li>
      <li><a href="#HF.3.6">F.3.6 Hint streams (Parts 5 and 10)</a>
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

<h3 id="HF.3.2">F.3.2 Header (Part 1)</h3>

<p class="location">Change the first paragraph as follows:</p>

<p>
The Linearized PDF file shall begin with the standard header line (see 7.5.2, "File header"). Linearization is independent of PDF version number and may be applied to any PDF file of version 
<del onMouseEnter="mouseEnter(this)" data-issue="331" data-iso="approved">1.1</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="331" data-iso="approved">1.2</ins> 
or greater.
</p>

<p>...</p>

<h3 id="HF.3.3">F.3.3 Linearization parameter dictionary (Part 2)</h3>

<p class="location">Add a new informative NOTE below the first paragraph as follows:</p>

<p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="403" data-iso="approved">
NOTE: due to the above requirement for direct objects, Metadata streams (see 14.3.2, "Metadata streams") and Associated Files (see 14.13, "Associated Files") cannot be included in a Linearization parameter dictionary.
</ins></p> 


<p class="location">Change Table F.1 as follows:</p>

<table>
  <caption id="TableF.1">Table F.1 - Entries in the linearization parameter dictionary</caption>
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
  <tr>
    <td><b>P</b></td>
    <td>integer</td>
    <td>
      <p>(<i>Optional</i>) The page number of the first page; see 
      <del onMouseEnter="mouseEnter(this)" data-issue="389" data-iso="approved">F.3.4, "First-page cross-reference table and trailer (Part 3)"</del>
      <ins onMouseEnter="mouseEnter(this)" data-issue="389" data-iso="approved">F.3.7, "First-page section (Part 6)"</ins>. Default value: <i>0</i>.
      </p>
    </td>
  </tr>
</table>


<h3 id="HF.3.6">F.3.6 Hint streams (Parts 5 and 10)</h3>

<p class="location">Add a new informative NOTE 2 below the paragraph below the existing NOTE as follows:</p>

<p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="403" data-iso="approved">
NOTE 2: due to the above requirement for direct objects, Metadata streams (see 14.3.2, "Metadata streams") and Associated Files (see 14.13, "Associated Files") cannot be included in hint stream dictionaries.
</ins></p> 
</div>

<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
