---
subset: PDF/A-4
isodoc: ISO 19005-4:2020
isotitle: 'Document management - Electronic document file format for long-term preservation - Part 4: Use of ISO 32000-2 (PDF/A-4)'
title: PDF/A-4 Corrections
modified: 15 January 2022
---

<p>
This document lists all industry-approved corrections to {{ page.subset }} as defined by "{{ page.isodoc }} <i>{{ page.isotitle }}</i>".
All issues related to {{ page.subset }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>
with the label '<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aissue+label%3APDF%2FA-4" target="_blank">{{ page.subset }}</a>'.
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
<li><a href="clause06.html#Table2">Table 2 - PDF/A identification schema</a></li>
</ul>

<hr>
<link rel="stylesheet" href="../assets/iso-style.css">
<p class="footnote">Last modified: {{ page.modified }}</p>
