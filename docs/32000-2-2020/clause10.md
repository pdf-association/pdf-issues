---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 10
title: Rendering
modified: 18 February 2024
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
  <li>10.7 Scan conversion details
   <ul>
    <li><a href="#H10.7.2">10.7.2 Flatness tolerance</a>
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
Conversion from a CIE-based source colour to a CIE-based destination colour shall be performed based on <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">ISO 15076-1:2010 (ICC.1:2010)</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">the appropriate ICC specification (see "Table 66 - ICC profile versions supported by <b>ICCBased</b> colour spaces")</ins>.
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

<p>...</p>

<p class="location">Delete the paragraph below the bulleted list (above EXAMPLE) as follows:</p>

<p><del onMouseEnter="mouseEnter(this)" data-issue="311">
When a halftone dictionary of some other Type appears as the value of an entry in a Type 5 halftone dictionary, it shall apply only to the single colourant or colour component named by that entry’s key. This is in contrast to such a dictionary’s being used as the current halftone parameter in the graphics state, which shall apply to all colour components. If nonprimary colourants are requested when the current halftone is defined by any means other than a Type 5 halftone dictionary, the gray halftone screen and transfer function shall be used for all such colourants.
</del></p>

<h2 id="H10.7">10.7 Scan conversion details</h2>

<h3 id="H10.7.2">10.7.2 Flatness tolerance</h3>

<p class="location">Change the first paragraph as follows:</p>

<p>
The <i>flatness tolerance</i> controls the maximum permitted distance in device pixels between the mathematically correct path and an approximation constructed from straight line segments, as shown in "Figure 69 — Flatness tolerance". Flatness may be specified as the operand of the <b>i</b> operator (see "Table 56 — Graphics state operators") or as the value of the <b>FL</b> entry in a graphics state parameter dictionary (see "Table 57 — Entries in a graphics state parameter dictionary"). 
<del onMouseEnter="mouseEnter(this)" data-issue="371">It shall be a positive number.</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="371">It shall be a number in the range 0 to 100 inclusive, where a value of 0 shall specify the output device’s default flatness tolerance. The value indicates the maximum error tolerance measured in output device pixels.</ins>
</p>

</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
