---
subset: ECMAScript for PDF 2.0
isodoc: ISO 21757-1:2020
clause: 12
title: Object overview
modified: 8 May 2024
---

<ul>
   <li>12.19 Mesh
    <ul> 
     <li><a href="#H12.19.2">12.19.2 Mesh properties</a>
     </li>
    </ul>
   </li>
   <li>12.35 StateEvent
    <ul>
     <li><a href="#H12.35.1">12.35.1 General</a>
     </li>
    </ul>
   </li>
   <li>12.40 ToolEvent
    <ul>
     <li><a href="#H12.40.2">12.40.2 ToolEventHandler <del onMouseEnter="mouseEnter(this)" data-issue="267">methods</del><ins onMouseEnter="mouseEnter(this)" data-issue="267">properties</ins></a>
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

<h2 id="H12.19">12.19 Mesh</h2>

<h3 id="H12.19.2">12.19.2 Mesh properties</h3>

<p class="location">Change Table 113 as follows:</p>

<table>
  <caption id="Table113">Table 113 - Mesh properties</caption>
  <tr>
    <th>Property</th>
    <th>Type</th>
    <th>Access</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>material</td>
    <td>material</td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="388">R</ins></td>
    <td>...</td>
  </tr>
  <tr>
    <td>renderMode</td>
    <td>string</td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="388">R/W</ins></td>
    <td>...</td>
  </tr>
</table>


<h2 id="H12.35">12.35 StateEvent</h2>

<h3 id="H12.35.1">12.35.1 General</h3>

<p class="location">Add a new NOTE after the first and only paragraph as follows:</p>

<p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="210">
NOTE The state data could be stored or retrieved from the <b>Data</b> entry of the View Params dictionary as described in Table 345 of the ISO 32000-2 specification.
</ins></p>

<h2 id="H12.40">12.40 ToolEvent</h2>

<p class="location">Change the title of subclause 12.40.2 as follows:</p>

<h3 id="H12.40.2">12.40.2 ToolEventHandler
<del onMouseEnter="mouseEnter(this)" data-issue="267">methods</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="267">properties</ins></h3>

</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
