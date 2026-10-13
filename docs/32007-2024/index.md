---
isodoc: ISO TS 32007:2024
isotitle: 'Document management - Portable Document Format - RichMedia annotations conforming to glTF assets'
title: 'ISO TS 32007: RichMedia glTF assets'
last_modified_date: 13 October 2026
nav_order: 6
has_toc: false
search_exclude: true
---

<h1>{{ page.isodoc }}: <i>{{ page.isotitle }}</i></h1>

<p>
This document lists all industry-approved corrections to <a href="https://pdfa.org/resource/iso-32007/" target="_blank">"{{ page.isodoc }} <i>{{ page.isotitle }}</i>"</a>.
All issues related to {{ page.isodoc }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>
with the label '<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aissue+label%3A%22ISO%2FTS+32007%22" target="_blank">ISO/TS 32007</a>'.
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
</ul>
</nav>
