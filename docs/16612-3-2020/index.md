---
subset: PDF/VT-3
isodoc: ISO 16612-3:2020
isotitle: 'Graphic technology - Variable data exchange - Part 3: Using PDF/X-6 (PDF/VT-3)'
title: PDF/VT-3 Corrections
modified: 10 August 2021
---

<p>
This is a placeholder for all industry-approved corrections to {{ page.subset }} as defined by "{{ page.isodoc }} <i>{{ page.isotitle }}</i>".
All issues related to {{ page.subset }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>
with the label '<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aissue+label%3APDF%2FVT-3" target="_blank">{{ page.subset }}</a>'.
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

<hr>
<link rel="stylesheet" href="../assets/iso-style.css">
<p class="footnote">Last modified: {{ page.modified }}</p>
