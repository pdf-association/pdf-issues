---
subset: PDF/UA-1
isodoc: ISO 14289-1:2014
isotitle: 'Document management applications - Electronic document file format enhancement for accessibility - Part 1: Use of ISO 32000-1 (PDF/UA-1) '
title: ISO 14289-1:2014 PDF/UA-1
last_modified_date: 17 April 2026
nav_order: 9
has_toc: false
search_exclude: true
---

<h1>{{ page.isodoc }}: <i>{{ page.isotitle }}</i></h1>

<p>
This is a placeholder for all industry-approved corrections to <a href="https://pdfa.org/resource/iso-14289-pdfua/" target="_blank">"{{ page.isodoc }} <i>{{ page.isotitle }}</i>"</a>.
All issues related to {{ page.isodoc }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>
with the label '<a href="https://github.com/pdf-association/pdf-issues/issues?q=label%3A%22PDF%2FUA-1%22" target="_blank">PDF/UA-1</a>'.
</p>

<!-- p>Corrections are organized by the top level clauses in {{ page.isodoc }}:</p -->

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
