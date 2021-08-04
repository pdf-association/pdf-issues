---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: Annex H
title: (informative) Example PDF files
modified: 30 July 2021
---

<link rel="stylesheet" href="../assets/iso-style.css">
<div class="isostyle">

<h1>{{ page.clause }}. {{ page.title }}</h1>


<h2 id="HH.8.2">H.8.2 Table of Contents</h2>

<p>
The structure element's structure type entry (<b>S</b>) may have values that establish hierarchical relationships between entries in a table of contents.
The <b>TOCI</b> value specifies an individual member of a table of contents. The <b>TOC</b> value specifies a list made up of other table of contents items that
are individual members of the table of contents and/or lists of table of contents items. (The trailing character in <b>TOCI</b> is an upper case "i".)
</p>

<p><span class="new-text">NOTE the following example uses <b>Reference</b>, <b>TOC</b> and <b>TOCI</b> structure elements which are part of the <i>standard structure
namespace for PDF 1.7</i> and are entirely valid for use in PDF 2.0 under the <i>default standard structure namespace</i> (see 14.8.6, "Standard structure namespaces").
<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/62" target="_blank">Issue #62</a></span></span></p>

<p>...</p>

</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
