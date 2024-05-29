---
isodoc: PDF Declarations
clause: 8
title: PDF Declaration requirements
modified: 29 May 2024
---

<ul>
 <li>8.2 PDF Declarations Property Value Types
   <ul>
     <li><a href="#H8.2.1">8.2.1 Declaration</a>
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

<h2 id="H8.2">8.2 PDF Declarations Property Value Types</h2>

<h3 id="H8.2.1">8.2.1 Declaration</h3>

<p class="location">Change Table 2 as follows:</p>

<table>
  <caption id="Table2">Table 2 - PDF Declaration fields.</caption>
  <tr>
    <th>Name</th>
    <th>Type</th>
    <th>Property content</th>
  </tr>
  <tr>
    <td><b>pdfd:conformsTo</b></td>
	<td>URI</td>
	<td>
	  <p>(Required) A property containing a URI specifying the standard or profile referred to by the PDF Declaration. This property is intended to mirror the Dublin Core property <b>dc:conformsTo</b>.</p>
	  <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="395">
	  NOTE: The convention used by PDF Declarations is to use <code>#</code> as the only separator between the URI path and fragment components as shown in the example in 7.2
	  </ins></p>
	</td>
  </tr>
</table>

</div>

<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
