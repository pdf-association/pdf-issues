---
subset: PDF/X-6
isodoc: ISO 15930-9:2020
isotitle: 'Graphic technology - Prepress digital data exchange using PDF - Part 9: Complete exchange of printing data (PDF/X-6) and partial exchange of printing data with external profile reference (PDF/X-6p and PDF/X-6n)'
title: PDF/X-6 Corrections
modified: 6 October 2023
---

<p><strong>IMPORTANT NOTE: a formal dated revision of PDF/X-6 is currently being prepared by ISO TC 130 WG 2 that will adopt all resolutions published here as well as align wording with PDF/A-4 (ISO 19005-4:2020) and PDF 2.0 errata. This edition will eventually replace ISO 15930-9:2020.</strong></p> 

<p>
This is a placeholder for all industry-approved corrections to {{ page.subset }} as defined by "{{ page.isodoc }} <i>{{ page.isotitle }}</i>".
All issues related to {{ page.subset }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>
with the label '<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aissue+label%3APDF%2FX-6" target="_blank">{{ page.subset }}</a>'.
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
