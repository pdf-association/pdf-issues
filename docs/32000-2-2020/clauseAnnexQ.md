---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: Annex Q
title: (normative) Method for determining transparency on a page
modified: 14 February 2022
---

<ul class="noprint">
   <li><a href="#HQ.2">Q.2. Page content</a>
   </li>
</ul>
<hr>

<link rel="stylesheet" href="../assets/iso-style.css">
<div class="isostyle">
<div class="fixedpopup" id="issuelink">
    Issue #xxxx
</div>

<p class="fake-h1">{{ page.clause }}. {{ page.title }}</p>

<h2 id="HQ.2">Q.2. Page content</h2>

<p class="location">Change the last paragraph as follows:</p>

<p>
Since Annotations require an appearance stream which is drawn by a PDF processor on top of the page content, it is possible
that their presence may cause a page without any transparency to acquire some transparency. Therefore, all annotations object's
in the page dictionary's <b>Annots</b> array shall have their appearance streams processed as a form XObject, according to Q.3, "Form XObjects".
<ins onMouseEnter="mouseEnter(this)" data-issue="51">Any annotation that has a <b>BM</b> key (<i>PDF 2.0</i>) in the Annotation dictionary with a value other than <i>Normal</i>
shall be considered to contain transparency (see "Table 166 - Entries common to all annotation dictionaries").</ins>
</p>

</div>

<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
