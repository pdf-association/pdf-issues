---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: Annex Q
title: (normative) Method for determining transparency on a page
---

{% include iso-style.html %}
<div class="isostyle">

<h1>{{ page.clause }}. {{ page.title }}</h1>

<h2>Q.2. Page content</h2>

<p>...</p>

<p>
Since Annotations require an appearance stream which is drawn by a PDF processor on top of the page content, it is possible
that their presence may cause a page without any transparency to acquire some transparency. Therefore, all annotations object's
in the page dictionary's <b>Annots</b> array shall have their appearance streams processed as a form XObject, according to Q.3, "Form XObjects".
<span class="new-text">Any annotation that has a <b>BM</b> key (<i>PDF 2.0</i>) in the Annotation dictionary with a value other than <i>Normal</i>
shall be considered to contain transparency (see "Table 166 - Entries common to all annotation dictionaries").<span class="new-tooltiptext">Issue #51</span></span>
</p>

</div>


<hr>
<p class="footnote">Last modified: 16 April 2021</p>