---
isodoc: ISO TS 32005:2023
isotitle: 'Document management - Portable Document Format - PDF 1.7 and 2.0 structure namespace inclusion in ISO 32000-2'
title: 'ISO TS 32005: PDF 1.7 and 2.0 inclusion rules in PDF 2.0'
last_modified_date: 6 October 2023
nav_order: 6
has_toc: false
search_exclude: true
---

<h1>{{ page.isodoc }}: <i>{{ page.isotitle }}</i></h1>

<p>
This document lists all industry-approved corrections to <a href="https://pdfa.org/resource/iso-32005/" target="_blank">"{{ page.isodoc }} <i>{{ page.isotitle }}</i>"</a>.
All issues related to {{ page.isodoc }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>
with the label '<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aissue+label%3A%22ISO%2FTS+32005%22" target="_blank">ISO/TS 32005</a>'.
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
<li><a href="clause07.html#Table5">Table 5 - Parent-child relationships between the PDF 1.7 elements and PDF 2.0 elements</a></li>
</ul>
