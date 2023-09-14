---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: Annex E
title: (normative) Extending PDF
modified: 15 September 2023
---

<ul class="noprint">
    <li><a href="#HE.2">E.2 Classes of PDF names</a>
    </li>
</ul>
<hr>

<link rel="stylesheet" href="../assets/iso-style.css">
<div class="isostyle">
<div class="fixedpopup" id="issuelink">
    Issue #xxxx
</div>

<p class="fake-h1">{{ page.clause }}. {{ page.title }}</p>

<h2 id="HF.3">E.2 Classes of PDF names</h2>

<p>...</p>

<p class="location">Change the third bullet point for <i>Third class</i> as follows:</p>

<ul>
 <li>...</li>
 <li>
  <i>Third class.</i> Names that may be used only in PDF files that are part of an internal process between writer and processor in order to avoid conflicts with third-class names defined by others. 
  Third-class names shall all begin with a specific prefix
  <del onMouseEnter="mouseEnter(this)" data-issue="340">reserved for private extensions. This prefix, which is XX, shall be used as the first characters in the names of all private data added by the developer. It is not necessary to register third-class names in the PDF Names list.</del>
  <ins onMouseEnter="mouseEnter(this)" data-issue="340">, XX, which has been reserved for this purpose. Any keys that are added by a developer for the purpose of adding private data to a PDF, shall begin with this prefix. Third-class names cannot be registered in the PDF Names list.</ins>
 </li>
</ul>

</div>

<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
