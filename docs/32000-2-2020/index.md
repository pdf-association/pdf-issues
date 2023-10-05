---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
isotitle: 'Document management - Portable document format - Part 2: PDF 2.0'
title: PDF 2.0 Corrections
modified: 6 October 2023
---

<p>
This document lists all industry-approved corrections to {{ page.subset }} as defined by "{{ page.isodoc }} <i>{{ page.isotitle }}</i>".
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

<p>The following tables have all been corrected:</p>
<ul>
<li><a href="clause07.html#Table5">Table 5 - Entries common to all stream dictionaries</a></li>
<li><a href="clause07.html#Table15">Table 15 - Entries in the file trailer dictionary</a></li>
<li><a href="clause07.html#Table19">Table 19 - Additional entries in a hybrid-reference file’s trailer dictionary</a></li>
<li><a href="clause07.html#Table25">Table 25 - Entries common to all crypt filter dictionaries</a></li>
<li><a href="clause07.html#Table27">Table 27 - Additional crypt filter dictionary entries for public-key security handlers</a></li>
<li><a href="clause07.html#Table29">Table 29 - Entries in the catalog dictionary</a></li>
<li><a href="clause07.html#Table31">Table 31 - Entries in a page object</a></li>
<li><a href="clause07.html#Table32">Table 32 - Entries in the name dictionary</a></li>
<li><a href="clause07.html#Table34">Table 34 - Entries in a resource dictionary</a></li>
<li><a href="clause07.html#Table36">Table 36 - Entries in a name tree node dictionary</a></li>
<li><a href="clause07.html#Table42">Table 42 - Operators in Type 4 functions</a></li>
<li><a href="clause07.html#Table43">Table 43 - Entries in a file specification dictionary</a></li>
<li><a href="clause07.html#Table44">Table 44 - Additional entries in an embedded file stream dictionary</a></li>
<li><a href="clause07.html#Table47">Table 47 - Entries in a collection subitem dictionary</a></li>
<li><a href="clause07.html#Table48">Table 48 - Entries in an extensions dictionary</a></li>
<li><a href="clause08.html#Table50">Table 50 - Operator categories</a></li>
<li><a href="clause08.html#Table52">Table 52 - Device-dependent graphics state parameters</a></li>
<li><a href="clause08.html#Table59">Table 59 - Path-painting categories</a></li>
<li><a href="clause08.html#Table66">Table 66 - <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">ICC Specification versions supported by ICC based colour spaces</del><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">ICC profile versions supported by <b>ICCBased</b> colour spaces</ins></a></li>
<li><a href="clause08.html#Table74">Table 74 - Additional entries specific to a Type 1 pattern <ins onMouseEnter="mouseEnter(this)" data-issue="294">stream</ins> dictionary</a></li>
<li><a href="clause08.html#Table87">Table 87 - Additional entries specific to an image dictionary</a></li>
<li><a href="clause08.html#Table91">Table 91 - Entries in an inline image object</a></li>
<li><a href="clause08.html#Table99">Table 99 - Entries in an optional content configuration dictionary</a></li>
<li><a href="clause09.html#Table109">Table 109 - Entries in a Type 1 font dictionary</a></li>
<li><a href="clause09.html#Table110">Table 110 - Entries in a Type 3 font dictionary</a></li>
<li><a href="clause09.html#Table111">Table 111 - Type 3 font operators</a></li>
<li><a href="clause09.html#Table115">Table 115 - Entries in a CIDFont dictionary</a></li>
<li><a href="clause09.html#Table119">Table 119 - Entries in a Type 0 font dictionary</a></li>
<li><a href="clause09.html#Table120">Table 120 - Entries common to all font descriptors</a></li>
<li><a href="clause10.html#Table132">Table 132 - Entries in a Type 5 halftone dictionary</a></li>
<li><a href="clause11.html#Table145">Table 145 - Additional entries specific to a transparency group attributes dictionary</a></li>
<li><a href="clause12.html#Table147">Table 147 - Entries in a viewer preferences dictionary</a></li>
<li><a href="clause12.html#Table151">Table 151 - Entries in an outline item dictionary</a></li>
<li><a href="clause12.html#Table164">Table 164 - Entries in a transition dictionary</a></li>
<li><a href="clause12.html#Table166">Table 166 - Entries common to all annotation dictionaries</a></li>
<li><a href="clause12.html#Table176">Table 176 - Additional entries specific to a link annotation</a></li>
<li><a href="clause12.html#Table177">Table 177 - Additional entries specific to a free text annotation</a></li>
<li><a href="clause12.html#Table202">Table 202 - Additional entries specific to a go-to action</a></li>
<li><a href="clause12.html#Table220">Table 220 - Additional entries specific to a go-to-3D-view action</a></li>
<li><a href="clause12.html#Table224">Table 224 - Entries in the interactive form dictionary</a></li>
<li><a href="clause12.html#Table226">Table 226 - Entries common to all field dictionaries</a></li>
<li><a href="clause12.html#Table228">Table 228 - Additional entries common to all fields containing variable text</a></li>
<li><a href="clause12.html#Table232">Table 232 - Additional entry specific to a text field</a></li>
<li><a href="clause12.html#Table236">Table 236 - Entries in a signature field lock dictionary</a></li>
<li><a href="clause12.html#Table237">Table 237 - Entries in a signature field seed value dictionary</a></li>
<li><a href="clause12.html#Table239">Table 239 - Additional entries specific to a submit-form action</a></li>
<li><a href="clause12.html#Table242">Table 242 - Flag for reset-form actions</a></li>
<li><a href="clause12.html#Table255">Table 255 - Entries in a signature dictionary</a></li>
<li><a href="clause12.html#Table256">Table 256 - Entries in a signature reference dictionary</a></li>
<li><a href="clause12.html#Table257">Table 257 - Entries in the DocMDP transform parameters dictionary</a></li>
<li><a href="clause12.html#Table259">Table 259 - Entries in the FieldMDP transform parameters dictionary</a></li>
<li><a href="clause12.html#Table260">Table 260 - SubFilter value algorithm support</a></li>
<li><a href="clause12.html#Table263">Table 263 - Entries in a permissions dictionary</a></li>
<li><a href="clause12.html#Table273">Table 273 - Entries common to all requirement dictionaries</a></li>
<li><a href="clause12.html#Table274">Table 274 - <del onMouseEnter="mouseEnter(this)" data-issue="187" data-iso="submitted">Entries</del><ins onMouseEnter="mouseEnter(this)" data-issue="187" data-iso="submitted">Additional entries</ins> for specific types of requirements</a></li>
<li><a href="clause12.html#Table275">Table 275 - Requirement types</a></li>
<li><a href="clause13.html#Table277">Table 277 - Entries common to all rendition dictionaries</a></li>
<li><a href="clause13.html#Table285">Table 285 - Additional entries in a media clip data dictionary</a></li>
<li><a href="clause13.html#Table311">Table 311 - Entries in a 3D stream dictionary</a></li>
<li><a href="clause13.html#Table315">Table 315 - Entries in a 3D view dictionary</a></li>
<li><a href="clause13.html#Table317">Table 317 - Entries in a 3D background dictionary</a></li>
<li><a href="clause13.html#Table322">Table 322 - Entries in a 3D cross section dictionary</a></li>
<li><a href="clause13.html#Table323">Table 323 - Entries in a 3D node dictionary</a></li>
<li><ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="submitted"><a href="clause13.html#Table323a">Table 323a - Interpretation of 3D Node Subtype entry</a></ins></li>
<li><a href="clause13.html#Table331">Table 331 - Additional entries in a 3D measurement/markup dictionary for a 3D comment note</a></li>
<li><a href="clause13.html#Table333">Table 333 - Additional entries specific to a RichMedia annotation</a></li>
<li><a href="clause13.html#Table335">Table 335 - Entries in a RichMediaActivation dictionary</a></li>
<li><a href="clause13.html#Table341">Table 341 - Entries in a RichMediaContent dictionary</a></li>
<li><a href="clause13.html#Table343">Table 343 - Entries in a RichMediaInstance dictionary</a></li>
<li><a href="clause14.html#Table350">Table 350 - Entries in a page-piece dictionary</a></li>
<li><a href="clause14.html#Table352">Table 352 - Marked content operators</a></li>
<li><a href="clause14.html#Table355">Table 355 - Entries in a structure element dictionary</a></li>
<li><a href="clause14.html#Table358">Table 358 - Entries in an object reference dictionary</a></li>
<li><a href="clause14.html#Table365">Table 365 - Grouping level structure types</a></li>
<li><a href="clause14.html#Table368">Table 368 - General inline level structure types</a></li>
<li><a href="clause14.html#Table371">Table 371 - Table standard structure types</a></li>
<li><a href="clause14.html#Table372">Table 372 - Standard structure type Caption</a></li>
<li><a href="clause14.html#Table377">Table 377 - Standard layout attributes</a></li>
<li><a href="clause14.html#Table378">Table 378 - Standard layout attributes common to all standard structure types</a></li>
<li><a href="clause14.html#Table380">Table 380 - Standard layout attributes specific to inline-level structure elements</a></li>
<li><a href="clause14.html#Table393">Table 393 - Entries in a Web Capture command dictionary</a></li>
<li><a href="clauseAnnexA.html#TableA.1">Table A.1 - PDF content stream operators</a></li>
<li><a href="clauseAnnexD.html#TableD.3">Table D.3 - PDFDocEncoding character set</a></li>
<li><a href="clauseAnnexF.html#TableF.1">Table F.1 - Entries in the linearization parameter dictionary</a></li>
</ul>

<hr>
<link rel="stylesheet" href="https://pdf-issues.pdfa.org/assets/iso-style.css">
<p class="footnote">Last modified: {{ page.modified }}</p>
