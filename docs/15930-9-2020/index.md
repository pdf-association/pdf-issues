---
subset: PDF/X-6
isodoc: ISO 15930-9:2020
isotitle: 'Graphic technology - Prepress digital data exchange using PDF — Part 9: Complete exchange of printing data (PDF/X-6) and partial exchange of printing data with external profile reference (PDF/X-6p and PDF/X-6n)'
title: Corrections
---

<h1>{{ page.isodoc }} {{ page.subset }} {{ page.title }}</h1>

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
<p class="footnote">Last modified: 19 June 2021</p>
