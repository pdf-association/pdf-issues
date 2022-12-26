---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 10
title: Rendering
modified: 14 August 2022
---

<ul class="noprint">
    <li>10.3 CIE-Based colour to device colour
     <ul>
      <li><a href="#H10.3.1">10.3.1 General</a>
      </li>
     </ul>
    </li>
    <li>10.6 Halftones
     <ul>
      <li>10.6.5 Halftone dictionaries
       <ul>
        <li><a href="#H10.6.5.6">10.6.5.6 Type 5 halftones</a>
        </li>
       </ul>
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

<h2 id="H10.3">10.3 CIE-Based colour to device colour</h2>

<h3 id="H10.3.1">10.3.1 General</h3>

<p>...</p>

<p class="location">Change the last paragraph as follows:</p>

<p>
Conversion from a CIE-based source colour to a CIE-based destination colour shall be performed based on <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">ISO 15076-1:2010 (ICC.1:2010)</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">the appropriate ICC specification (see "Table 66 - ICC profile versions supported by <b>ICCBased</b> colour spaces")</ins>.
</p>


<h2 id="H10.6">10.6 Halftones</h2>

<h3 id="H10.6.5">10.6.5 Halftone dictionaries</h3>

<h4 id="H10.6.5.6">10.6.5.6 Type 5 halftones</h4>

<p class="location">Change Table 132 as follows:</p>

<table>
  <caption id="Table132">Table 132 - Entries in a Type 5 halftone dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Default</b></td>
    <td>dictionary or<br/>stream</td>
    <td>
    (<i>Required</i>) A halftone that shall be used for any colourant or colour component that does not have an entry of its own.
    <del onMouseEnter="mouseEnter(this)" data-issue="12" data-iso="approved">The value shall not be 5.</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="12" data-iso="approved">The halftone shall not be a Type 5 halftone.</ins>
    If there are any nonprimary colourants, the default halftone shall have a transfer function.
    </td>
  </tr>
</table>


</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
