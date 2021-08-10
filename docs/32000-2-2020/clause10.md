---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 10
title: Rendering
modified: 16 February 2021
---

<ul>
</ul>
<hr>

<link rel="stylesheet" href="../assets/iso-style.css">
<div class="isostyle">
<div class="fixedpopup" id="issuelink">
	Issue #xxxx
</div>

<p class="fake-h1">{{ page.clause }}. {{ page.title }}</p>

<h4 id="H10.6.5.6">10.6.5.6 Type 5 halftones</h4>


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
    <del onMouseEnter="mouseEnter(this)" data-issue="12">The value shall not be 5.</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="12">The halftone shall not be a Type 5 halftone.</ins>
    If there are any nonprimary colourants, the default halftone shall have a transfer function.
    </td>
  </tr>
</table>


</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
