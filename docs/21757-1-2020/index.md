---
subset: ECMAScript for PDF 2.0
isodoc: ISO 21757-1:2020
isotitle: 'Document management - ECMAScript for PDF - Part 1: Use of ISO 32000-2 (PDF 2.0)'
title: 'PDF 2.0 ECMAscript  Corrections'
modified: 8 May 2024
---

<p>
This document lists all industry-approved corrections to {{ page.subset }} as defined by "{{ page.isodoc }} <i>{{ page.isotitle }}</i>".
All issues related to {{ page.subset }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>
with the label '<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aopen+is%3Aissue+label%3A%22ISO+21757-1%3A2020%22" target="_blank">{{ page.isodoc }}</a>'.
</p>

<p>Corrections are organized by the top level clauses in {{ page.isodoc }}:</p>

<ul>
    {% for std in site.data.data.toc %}
         {% if std.standard == page.isodoc %}
            {% for pg in std.subfolderitems %}
            <li><a href="{{ pg.url }}">{{ pg.ref }}</a></li>
           {% endfor %}
        {% endif %}
    {% endfor %}
</ul>

<p>The following tables have been corrected:</p>
<ul>
<li><a href="clause10.html#Table1">Table 1 - Annotation types and their properties</a></li>
<li><a href="clause10.html#Table3">Table 3 - AnnotRichMedia object properties</a></li>
<li><a href="clause10.html#Table89">Table 89 - oRequest <del onMouseEnter="mouseEnter(this)" data-issue="268">parameters</del><ins onMouseEnter="mouseEnter(this)" data-issue="268">properties</ins></a></li>
<li><a href="clause12.html#Table113">Table 113 - Mesh properties</a></li>
</ul>

<hr>
<link rel="stylesheet" href="../assets/iso-style.css">
<p class="footnote">Last modified: {{ page.modified }}</p>
