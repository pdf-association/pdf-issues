---
subset: PDF/A-4
isodoc: ISO 19005-4:2020
isotitle: 'Document management - Electronic document file format for long-term preservation - Part 4: Use of ISO 32000-2 (PDF/A-4)'
title: ISO 19005-4:2020 PDF/A-4
last_modified_date: 6 October 2023
nav_order: 14
has_toc: false
search_exclude: true
---

<h1>{{ page.isodoc }}: <i>{{ page.isotitle }}</i></h1>

<p><strong>IMPORTANT NOTE: a formal dated revision of PDF/A-4 is currently being prepared by ISO TC 171 SC 2 WG 5 that will adopt all resolutions published here as well as align wording with PDF/X-6 (ISO 15930-9:2020) and PDF 2.0 errata. This edition will eventually replace ISO 19005-4:2020.</strong></p> 

<p>
This document lists all industry-approved corrections to {{ page.subset }} as defined by "{{ page.isodoc }} <i>{{ page.isotitle }}</i>".
All issues related to {{ page.subset }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>
with the label '<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aissue+label%3APDF%2FA-4" target="_blank">{{ page.subset }}</a>'.
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

<p>The following tables have been corrected:</p>

<nav>
<ul>
<li><a href="clause06.html#Table2">Table 2 - PDF/A identification schema</a></li>
</ul>
</nav>
