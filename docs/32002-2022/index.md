---
isodoc: ISO TS 32002:2022
isotitle: 'Document management — Portable Document Format — Extensions to Digital Signatures in ISO 32000-2 (PDF 2.0)'
title: 'ISO TS 32002: PDF 2.0 Digital Signature extensions'
last_modified_date: 11 Sept 2024
nav_order: 3
has_toc: false
search_exclude: true
---

<h1>{{ page.isodoc }}: <i>{{ page.isotitle }}</i></h1>

<p>
This document lists all industry-approved corrections to <a href="https://www.pdfa.org/resource/iso-ts-32002/" target="_blank">"{{ page.isodoc }} <i>{{ page.isotitle }}</i>"</a>.
All issues related to {{ page.isodoc }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>
with the label '<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aissue+label%3A%22ISO%2FTS+32002%22" target="_blank">ISO/TS 32002</a>'.
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
<li><a href="clause05.html#Table2">Table 2 - Additional permitted SubFilter values for ISO 32000-2:2020, Table 260</a></li>
<li><a href="clause05.html#Table4">Table 4 - Supported EdDSA elliptic curves</a></li>
</ul>
