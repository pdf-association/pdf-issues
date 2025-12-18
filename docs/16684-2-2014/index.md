---
subset: XMP RELAX NG schemas
isodoc: ISO 16684-2:2014
isotitle: 'Graphic technology — Extensible metadata platform (XMP)Part 2: Description of XMP schemas using RELAX NG'
title: ISO 16684-2:2014 XMP RELAX NG schema
last_modified_date: 11 November 2025
nav_order: 13
has_toc: false
search_exclude: true
---

<h1>{{ page.isodoc }}: <i>{{ page.isotitle }}</i></h1>

<p>
This is all industry-approved corrections to {{ page.subset }} as defined by "{{ page.isodoc }} <i>{{ page.isotitle }}</i>".
All issues related to {{ page.subset }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>.
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
