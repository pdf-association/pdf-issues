---
isodoc: PDF Declarations
isotitle: A use of ISO 32000
title: PDF Declarations
last_modified_date: 29 May 2024
nav_order: 21
has_toc: false
search_exclude: true
---

<h1>{{ page.isodoc }}: <i>{{ page.isotitle }}</i></h1>

<p>
This document lists all industry-approved corrections to <a href="https://www.pdfa.org/resource/iso-ts-32001/" target="_blank">"{{ page.isodoc }}: <i>{{ page.isotitle }}</i>"</a>.
All issues related to {{ page.isodoc }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>
with the label '<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aissue+label%3A%22PDF+Declarations%22" target="_blank">PDF Declarations</a>'.
</p>

<p>Corrections are organized by the top level clauses in {{ page.isodoc }}:</p>

<nav>
<ul>
    {% for std in site.data.data.toc %}
         {% if std.standard == page.isodoc %}
            {% for pg in std.subfolderitems %}
            <li><a href="{{ pg.url }}">{{ pg.ref }}</a></li>
           {% endfor %}
        {% endif %}
    {% endfor %}
</ul>
</nav>

<p>The following tables have all been corrected:</p>

<nav>
<ul>
<li><a href="clause08.html#Table2">Table 2 - PDF Declaration fields.</a></li>
</ul>
</nav>
