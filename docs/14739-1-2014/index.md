---
isodoc: ISO 14739-1:2014
isotitle: 'Document management - 3D use of Product Representation Compact (PRC) formatPart 1: PRC 10001'
title: 'PRC Corrections'
modified: 29 May 2024
---

<p>
This is a placeholder for all industry-approved corrections to <a href="https://pdfa.org/resource/3d-formats/" target="_blank">"{{ page.isodoc }} <i>{{ page.isotitle }}</i>"</a>.
All issues related to {{ page.isodoc }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>
with the label '<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aissue+label%3APRC" target="_blank">PRC</a>'.
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
