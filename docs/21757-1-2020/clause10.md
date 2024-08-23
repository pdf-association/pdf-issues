---
subset: ECMAScript for PDF 2.0
isodoc: ISO 21757-1:2020
clause: 10
title: ECMAScript API
modified: 14 February 2022
---

<ul>
    <li><a href="#H10.1">10.1 General</a>
    </li>
    <li>10.2 Annotation
      <ul>
        <li><a href="#H10.2.2">10.2.2 Annotation types</a>
        </li>
      </ul>
    </li>
    <li>10.3 AnnotRichMedia
      <ul>
        <li><a href="#H10.3.2">10.3.2 AnnotRichMedia properties</a>
        </li>
      </ul>
    </li>
    <li>10.32 SOAP
      <ul>
        <li>10.32.3 SOAP methods
          <ul>
            <li>10.32.3.5 request(...)
              <ul>
                <li><a href="#H10.32.3.5.1">10.32.3.5.1 oRequest Parameter Details</a>
                </li>
              </ul>
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

<h2 id="H10.1">10.1 General</h2>

<p class="location">Delete the last paragraph as follows:</p>

<p>
<del onMouseEnter="mouseEnter(this)" data-issue="70" data-iso="approved">More information regarding the ECMAScript core can be found in ISO/IEC 22537.</del>
</p>

<h2 id="H10.2">10.2 Annotation</h2>

<p>...</p>

<h3 id="H10.2.2">10.2.2 Annotation types</h3>

<p class="location">Change the list as follows:</p>

<table style="border: none;">
<tr style="border: none;">
    <td style="border: none;"><ins onMouseEnter="mouseEnter(this)" data-issue="82" data-iso="approved">Sound</ins></td>
    <td style="border: none;"><ins onMouseEnter="mouseEnter(this)" data-issue="82" data-iso="approved">Deprecated in ISO 32000-2</ins></td>
</tr>
<tr style="border: none;">
    <td style="border: none;"><del onMouseEnter="mouseEnter(this)" data-issue="82" data-iso="approved">PrinterMark</del></td>
    <td style="border: none;"><del onMouseEnter="mouseEnter(this)" data-issue="82" data-iso="approved">Deprecated in ISO 32000-2</del></td>
</tr>
<tr style="border: none;">
    <td style="border: none;"><del onMouseEnter="mouseEnter(this)" data-issue="82" data-iso="approved">Screen</del></td>
    <td style="border: none;"><del onMouseEnter="mouseEnter(this)" data-issue="82" data-iso="approved">Deprecated in ISO 32000-2 (replaced by the <b>AnnotRichMedia</b> annotation)</del></td>
</tr>
</table>

<p class="location">Change Table 1 as follows:</p>

<table>
  <caption id="Table1">Table 1 - Annotation types and their properties</caption>
  <tr>
    <th>Annotation type</th>
    <th>Properties</th>
  </tr>
  <tr>
    <td>Sound <ins onMouseEnter="mouseEnter(this)" data-issue="82" data-iso="approved"><i>(deprecated in PDF 2.0)</i></ins></td>
    <td style="font-family: monospace; font-size: smaller;">author, borderEffectIntensity, borderEffectStyle, contents, creationDate, delay, hidden, inReplyTo, intent, lock, modDate, name, noView, opacity, page, point, print, readOnly, rect, refType, richContents, rotate, seqNum, soundIcon, strokeColor, style, subject, toggleNoView, type, width</td>
  </tr>
</table>

<h2 id="H10.3">10.3 AnnotRichMedia</h2>

<h3 id="H10.3.2">10.3.2 AnnotRichMedia</h3>

<p class="location">Change Table 3 as follows:</p>

<table>
  <caption id="Table3">Table 3 - AnnotRichMedia object properties</caption>
  <tr>
    <th>Property</th>
    <th>Type</th>
    <th>Access</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>
      <del onMouseEnter="mouseEnter(this)" data-issue="266" data-iso="submitted">rec:</del>
      <ins onMouseEnter="mouseEnter(this)" data-issue="266" data-iso="submitted">rect</ins>
    </td>
    <td>Array</td>
    <td>R/W</td>
    <td>...</td>
  </tr>
</table>

<h2 id="H10.32">10.32 SOAP</h2>

<h3 id="H10.32.3">10.32.3 SOAP methods</h3>

<h4 id="H10.32.3.5">10.32.3.5 request(...)</h4>

<h5 id="H10.32.3.5.1">10.32.3.5.1 oRequest Parameter Details</h5>

<p class="location">Change Table 89 as follows:</p>

<table>
  <caption id="Table89">Table 89 - oRequest <del onMouseEnter="mouseEnter(this)" data-issue="268" data-iso="submitted">parameters</del><ins onMouseEnter="mouseEnter(this)" data-issue="268">properties</ins></caption>
  <tr>
    <th>
    <del onMouseEnter="mouseEnter(this)" data-issue="268" data-iso="submitted">Parameter</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="268" data-iso="submitted">Property</ins>
    </th>
    <th>Type</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>...</td>
    <td>...</td>
    <td>...</td>
  </tr>
</table>

</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
