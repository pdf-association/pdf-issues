---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
isotitle: 'Document management - Portable document format - Part 2: PDF 2.0'
title: PDF 2.0 Corrections
modified: 10 August 2021
---

<p>
This is all industry-approved corrections to {{ page.subset }} as defined by "{{ page.isodoc }} <i>{{ page.isotitle }}</i>".
All issues related to {{ page.subset }} are recorded in the PDF Association's <a href="https://github.com/pdf-association/pdf-issues" target="_blank">GitHub pdf-issues</a>.
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

<p>The following tables have all had corrections applied:</p>
<ul>
<li><a href="clause07.html#Table5">Table 5 - Entries common to all stream dictionaries</a></li>
<li><a href="clause07.html#Table15">Table 15 - Entries in the file trailer dictionary</a></li>
<li><a href="clause07.html#Table27">Table 27 - Additional crypt filter dictionary entries for public-key security handlers</a></li>
<li><a href="clause07.html#Table31">Table 31 - Entries in a page object</a></li>
<li><a href="clause07.html#Table47">Table 47 - Entries in a collection subitem dictionary</a></li>
<li><a href="clause07.html#Table48">Table 48 - Entries in an extensions dictionary</a></li>
<li><a href="clause08.html#Table50">Table 50 - Operator categories</a></li>
<li><a href="clause08.html#Table59">Table 59 - Path-painting categories</a></li>
<li><a href="clause08.html#Table87">Table 87 - Additional entries specific to an image dictionary</a></li>
<li><a href="clause09.html#Table109">Table 109 - Entries in a Type 1 font dictionary</a></li>
<li><a href="clause09.html#Table111">Table 111 - Type 3 font operators</a></li>
<li><a href="clause09.html#Table120">Table 120 - Entries common to all font descriptors</a></li>
<li><a href="clause10.html#Table132">Table 132 - Entries in a Type 5 halftone dictionary</a></li>
<li><a href="clause12.html#Table147">Table 147 - Entries in a viewer preferences dictionary</a></li>
<li><a href="clause12.html#Table164">Table 164 - Entries in a transition dictionary</a></li>
<li><a href="clause12.html#Table166">Table 166 - Entries common to all annotation dictionaries</a></li>
<li><a href="clause12.html#Table176">Table 176 - Additional entries specific to a link annotation</a></li>
<li><a href="clause12.html#Table177">Table 177 - Additional entries specific to a free text annotation</a></li>
<li><a href="clause12.html#Table226">Table 226 - Entries common to all field dictionaries</a></li>
<li><a href="clause12.html#Table237">Table 237 - Entries in a signature field seed value dictionary</a></li>
<li><a href="clause12.html#Table255">Table 255 - Entries in a signature dictionary</a></li>
<li><a href="clause12.html#Table259">Table 259 - Entries in the FieldMDP transform parameters dictionary</a></li>
<li><a href="clause12.html#Table260">Table 260 - SubFilter value algorithm support</a></li>
<li><a href="clause13.html#Table311">Table 311 - Entries in a 3D stream dictionary</a></li>
<li><a href="clause13.html#Table315">Table 315 - Entries in a 3D view dictionary</a></li>
<li><a href="clause13.html#Table317">Table 317 - Entries in a 3D background dictionary</a></li>
<li><a href="clause13.html#Table322">Table 322 - Entries in a 3D cross section dictionary</a></li>
<li><a href="clause13.html#Table335">Table 335 - Entries in a RichMediaActivation dictionary</a></li>
<li><a href="clause13.html#Table343">Table 343 - Entries in a RichMediaInstance dictionary</a></li>
<li><a href="clause14.html#Table350">Table 350 - Entries in a page-piece dictionary</a></li>
<li><a href="clause14.html#Table355">Table 355 - Entries in a structure element dictionary</a></li>
<li><a href="clause14.html#Table368">Table 368 - General inline level structure types</a></li>
<li><a href="clause14.html#Table371">Table 371 - Table standard structure types</a></li>
<li><a href="clause14.html#Table372">Table 372 - Standard structure type Caption</a></li>
<li><a href="clauseAnnexA.html#TableA.1">Table A.1 - PDF content stream operators</a></li>
</ul>

<hr>
<link rel="stylesheet" href="../assets/iso-style.css">
<p class="footnote">Last modified: {{ page.modified }}</p>
