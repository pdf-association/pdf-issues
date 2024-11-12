---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: Annex E
title: (normative) Extending PDF
modified: 7 June 2024
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

<p class="location">Change the first paragraph of the second bullet point for <i>Second class</i> as follows:</p>

<ul>
  <li>...</li>
  <li>
    <p><i>Second class</i>. Names that are applicable to a specific developer. All names that begin with 4 characters including or followed by a LOW LINE (5fh) or COLON (3Ah) in either the key or value of a dictionary entry are second-class names, except 
    <del onMouseEnter="mouseEnter(this)" data-issue="229" data-iso="approved">">keys added to a document information dictionary (see 14.3.3, "Document information dictionary") or a thread information dictionary (in the I entry of a thread dictionary; see 12.4.3, "Articles")</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="229" data-iso="approved">"> where otherwise stated in this specification</ins>
    . 
    Those four-byte prefixes are developer-specific name prefixes that are managed in a public list at <a href="https://github.com/adobe/pdf-names-list">https://github.com/adobe/pdf-names-list</a>, to which new prefixes can be added.
    </p>
    <p>...</p>
  </li>
</ul>

<p class="location">Change the third bullet point for <i>Third class</i> as follows:</p>

<ul>
 <li>
  <i>Third class.</i> Names that may be used only in PDF files that are part of an internal process between writer and processor in order to avoid conflicts with third-class names defined by others. 
  Third-class names shall all begin with a specific prefix
  <del onMouseEnter="mouseEnter(this)" data-issue="340" data-iso="approved">reserved for private extensions. This prefix, which is XX, shall be used as the first characters in the names of all private data added by the developer. It is not necessary to register third-class names in the PDF Names list.</del>
  <ins onMouseEnter="mouseEnter(this)" data-issue="340" data-iso="approved">, XX, which has been reserved for this purpose. Any keys that are added by a developer for the purpose of adding private data to a PDF, shall begin with this prefix. Third-class names cannot be registered in the PDF Names list.</ins>
 </li>
</ul>

</div>

<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
