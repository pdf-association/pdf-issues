---
isodoc: PDF Declarations
isotitle: 'PDF Declarations: A use of ISO 32000'
title: 'PDF Declarations Corrections'
modified: 29 May 2024
---

<p>
This document lists all industry-approved corrections to <a href="https://www.pdfa.org/resource/iso-ts-32001/" target="_blank">"{{ page.isodoc }} <i>{{ page.isotitle }}</i>"</a>.
All issues related to {{ page.isodoc }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>
with the label '<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aissue+label%3A%22PDF+Declarations%22" target="_blank">PDF Declarations</a>'.
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

<p>The following tables have all been corrected:</p>
<ul>
<li><a href="clause08.html#Table2">Table 2 - PDF Declaration fields.</a></li>
</ul>

<hr>
<link rel="stylesheet" href="../assets/iso-style.css">
<p class="footnote">Last modified: {{ page.modified }}</p>
