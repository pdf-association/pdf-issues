---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 11
title: Transparency
modified: 20 March 2022
---

<ul class="noprint">
    <li>11.6 Specifying transparency in PDF
     <ul>
      <li><a href="#H11.6.6">11.6.6 Transparency group XObjects</a>
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

<h2 id="H11.6">11.6 Specifying transparency in PDF</h2>

<h3 id="H11.6.6">11.6.6 Transparency group XObjects</h3>

<p class="location">Change Table 145 as follows:</p>

<table>
  <caption id="Table145">Table 145 -Additional entries specific to a transparency group attributes dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>CS</b></td>
    <td>name or array</td>
    <td>
    <p>...</p>
    <p>
    The group colour space shall be any device or CIE-based colour space that treats its components as independent
    additive or subtractive values in the range 0.0 to 1.0, subject to the restrictions described in 11.3.4,
    "Blending colour space". These restrictions exclude Lab and lightness-chromaticity <b>ICCBased</b> colour
    spaces, as well as the special colour spaces <b>Pattern</b>, <b>Indexed</b>, <b>Separation</b>, and <b>DeviceN</b>.
    Device colour spaces shall be subject to remapping according to the <b>DefaultGray</b>, <b>DefaultRGB</b>, and
    <b>DefaultCMYK</b> entries in the <b>ColorSpace</b> subdictionary of the current resource dictionary
    <ins onMouseEnter="mouseEnter(this)" data-issue="134">of the group XObject</ins>
    (see 8.6.5.6, "Default colour spaces").
    </p>
    <p>...</p>
    </td>
  </tr>
</table>
</div>


<hr>
<p class="footnote">Last modified: {{ page.modified }}</p>