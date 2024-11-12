---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 3
title: Terms and definitions
modified: 19 April 2024
---

<ul class="noprint">
 <li><a href="#H3.31">3.31 ICC profile</a>
 </li>
 <li><a href="#H3.32">3.32 ICC specification</a>
 </li>
</ul>
<hr>

<link rel="stylesheet" href="../assets/iso-style.css">
<div class="isostyle">
<div class="fixedpopup" id="issuelink">
    Issue #xxxx
</div>

<p class="fake-h1">{{ page.clause }}. {{ page.title }}</p>

<p class="editornote">EDITOR NOTE: ISO requires that Terms and Definitions are sorted alphabetically, which may result in updated numbering.
</p>

<p class="location">Change term 3.31 ICC profile as follows:</p>

<h2 id="H3.31">3.31<br/>ICC profile</h2>
<p>
ISO 15076-1<del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">:2010</del> or <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">any of the ICC.1 specifications</del><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">"Specification ICC.1:2001-04 - File Format for Color Profiles [REVISION of ICC.1:1998-09]"</ins>
</p>

<p class="location">Change term 3.32 ICC specification as follows:</p>

<h2 id="H3.32">3.32<br/>ICC specification</h2>
<p>
cross-platform profile format for the creation and interpretation of colour data and means of reference to ISO 15076-1<del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">:2010</del> or <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">any of the ICC.1 specifications</del><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">"Specification ICC.1:2001-04 - File Format for Color Profiles [REVISION of ICC.1:1998-09]"</ins>
</p>

<p class="location">Add the following new Terms and Definitions (<i>subclause numbering is not shown</i>):</p>

<h2><ins onMouseEnter="mouseEnter(this)" data-issue="149" data-iso="approved"><i>x.y</i><br/>cross-reference table</ins></h2>
<p>
<ins onMouseEnter="mouseEnter(this)" data-issue="149" data-iso="approved">data derived from all cross-reference sections and cross-reference streams in a PDF file that contains information that permits random access to all indirect objects within the PDF file (see 7.5.4 "Cross-reference table").</ins>
</p>
<p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="149" data-iso="approved">NOTE TO ENTRY: common colloquial usage of "cross-reference table" is often incorrectly used to describe a cross-reference section.</ins></p>

<h2><ins onMouseEnter="mouseEnter(this)" data-issue="149" data-iso="approved"><i>x.y</i><br/>cross-reference section</ins></h2>
<p>
<ins onMouseEnter="mouseEnter(this)" data-issue="149" data-iso="approved">begins with a line containing the keyword <b>xref</b> followed by one or more cross-reference subsections (see 7.5.4 "Cross-reference table").</ins>
</p>
<p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="149" data-iso="approved">NOTE TO ENTRY: common colloquial usage of "cross-reference table" is often incorrectly used to describe a cross-reference section.</ins></p>

<h2><ins onMouseEnter="mouseEnter(this)" data-issue="149" data-iso="approved"><i>x.y</i><br/>cross-reference sub-section</ins></h2>
<p>
<ins onMouseEnter="mouseEnter(this)" data-issue="149" data-iso="approved">exist within cross-reference sections and start with a line containing a pair of integers followed by lines containing entries for a contiguous range of object numbers (see 7.5.4 "Cross-reference table").</ins>
</p>

<p>...</p>

</div>


<hr>
<p class="footnote">Last modified: {{ page.modified }}</p>
