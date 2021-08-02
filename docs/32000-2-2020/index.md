---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
isotitle: 'Document management - Portable document format - Part 2: PDF 2.0'
title: PDF 2.0 Corrections
---

<h1>{{ page.isodoc }} {{ page.title }}</h1>

<p>
This is a placeholder for all industry-approved corrections to {{ page.subset }} as defined by "{{ page.isodoc }} <i>{{ page.isotitle }}</i>".
All issues related to {{ page.subset }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>.
</p>

<p>Corrections are organized by the top level clauses in {{ page.isodoc }}:</p>

<ul>
    {% for std in site.data.data.toc %}
         {% if std.standard == page.isodoc %}
            {% for pg in std.subfolderitems %}
            <li><a href="{{ pg.url }}" target="github">{{ pg.ref }}</a></li>
           {% endfor %}
        {% endif %}
    {% endfor %}
</ul>

<hr>
<p class="footnote">Last modified: 19 June 2021</p>
