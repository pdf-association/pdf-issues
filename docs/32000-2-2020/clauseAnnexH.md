---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: Annex H
title: (informative) Example PDF files
modified: 14 February 2022
---

<ul class="noprint">
  <li>H.8 Structure elements examples
    <ul>
      <li><a href="clauseAnnexH#HH.8.2">H.8.2 Table of Contents</a>
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

<h2 id="HH.8">H.8 Structure elements examples</h2>

<h3 id="HH.8.2">H.8.2 Table of Contents</h3>

<p class="location">Insert a new NOTE after the first paragraph as follows:</p>

<p>
The structure element's structure type entry (<b>S</b>) may have values that establish hierarchical relationships between entries in a table of contents.
The <b>TOCI</b> value specifies an individual member of a table of contents. The <b>TOC</b> value specifies a list made up of other table of contents items that
are individual members of the table of contents and/or lists of table of contents items. (The trailing character in <b>TOCI</b> is an upper case "i".)
</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="62">NOTE the following example uses <b>Reference</b>, <b>TOC</b> and <b>TOCI</b> structure elements which are
part of the <i>standard structure namespace for PDF 1.7</i> and are entirely valid for use in PDF 2.0 under the <i>default standard structure namespace</i>
(see 14.8.6, "Standard structure namespaces").</ins>
</p>

<p>...</p>

</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
