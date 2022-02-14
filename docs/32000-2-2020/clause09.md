---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 9
title: Text
modified: 14 February 2022
---

<ul class="noprint">
 <li>9.6 Simple fonts
  <ul>
   <li>9.6.2 Type 1 fonts
    <ul>
     <li><a href="#H9.6.2.1">9.6.2.1 General</a>
     </li>
     <li><a href="#H9.6.2.2">9.6.2.2 Standard Type 1 fonts (standard 14 fonts) (PDF 1.0-1.7)</a>
     </li>
    </ul>
   </li>
   <li><a href="#H9.6.4">9.6.4 Type 3 fonts</a>
   </li>
  </ul>
 </li>
 <li>9.8 Font descriptors
  <ul>
   <li><a href="#H9.8.1">9.8.1 General</a>
   </li>
   <li>9.8.3 Font descriptors for CIDFonts
    <ul>
     <li><a href="#H9.8.3.3">9.8.3.3 FD</a>
     </li>
    </ul>
   </li>
  </ul>
 </li>
 <li>9.10 Extraction of text content
  <ul>
   <li><a href="#H9.10.3">9.10.3 ToUnicode CMaps</a>
   </li>
  </ul>
 </li>
</ul>
<hr>

<link rel="stylesheet" href="../assets/iso-style.css">
<div class="isostyle">
<div class="fixedpopup" id="issuelink">
    Issue #xxxx
</div>

<p class="fake-h1">{{ page.clause }}. {{ page.title }}</p>

<h3 id="H9.6.2">9.6.2 Type 1 fonts</h3>

<h4 id="H9.6.2.1">9.6.2.1 General</h4>

<p class="location">Change Table 109 as follows:</p>

<table>
  <caption id="Table109">Table 109 - Entries in a Type 1 font dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>FontDescriptor</b></td>
    <td>dictionary</td>
    <td>
    <p>(<i>Required; optional in PDF 1.0-1.7 for the standard 14 fonts; shall be an indirect reference</i>) A font descriptor describing the
    font's metrics other than its glyph widths (see 9.8, "Font descriptors").</p>
    <p>
    <del onMouseEnter="mouseEnter(this)" data-issue="47,48">For the standard 14 fonts, the entries <b>FirstChar</b>, <b>LastChar</b>, <b>Widths</b>, and <b>FontDescriptor</b> shall either all be present or all be absent. Ordinarily, these dictionary keys may be absent; specifying them enables a standard font to be overridden; see</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="47,48">See also</ins>
    9.6.2.2, "Standard Type 1 fonts (standard 14 fonts) (PDF 1.0-1.7)".
    </p>
    </td>
  </tr>
</table>

<p class="location">Change the paragraph below Table 109 as follows:</p>

<p>
<del onMouseEnter="mouseEnter(this)" data-issue="47,48">PDF versions 1.0 to 1.7 did not require Type 1 font dictionaries to include <b>FirstChar</b>, <b>LastChar</b>, <b>Widths</b> and <b>FontDescriptor</b> entries as described in 9.6.2.2, "Standard Type 1 fonts (standard 14 fonts) (PDF 1.0-1.7)". For compatibility reasons PDF processors shall provide glyph widths and font descriptor data for those standard fonts for use in processing PDF files when the entries are absent.</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="47,48">See also 9.6.2.2, "Standard Type 1 fonts (standard 14 fonts) (PDF 1.0-1.7)".</ins>
</p>


<p>...</p>

<h4 id="H9.6.2.2">9.6.2.2 Standard Type 1 fonts (standard 14 fonts) (PDF 1.0-1.7)</h4>

<p class="location">Change the second paragraph to a NOTE and modify as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="47,48">NOTE: </ins>
In PDF 1.0 to PDF 1.7, the <b>FirstChar</b>, <b>LastChar</b>, <b>Widths</b> and <b>FontDescriptor</b> (see "Table 109 - Entries in a Type 1 font dictionary") were
optional in Type 1 font dictionaries for the standard 14 fonts. PDF processors supporting PDF 1.0 to PDF 1.7 files
<del onMouseEnter="mouseEnter(this)" data-issue="47,48">shall</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="47,48">are required to</ins>
have these fonts, or their font metrics and suitable substitution fonts available.</p>

<p class="location">Delete the last paragraph as follows:</p>

<p>
<del onMouseEnter="mouseEnter(this)" data-issue="47,48">These fonts, or their font metrics and suitable substitution fonts, shall be available to the PDF processor.</del>
</p>


<h3 id="H9.6.4">9.6.4 Type 3 fonts</h3>

<p class="location">Change the first paragraph as follows:</p>

<p>
Type 3 fonts differ from the other fonts supported by PDF. Font dictionaries for other fonts simply contain information about the font and refer to a separate font program for the actual glyph descriptions; a Type 3 font dictionary contains the glyph descriptions. In Type 3 fonts, glyphs shall be defined by streams of PDF graphics <del onMouseEnter="mouseEnter(this)" data-issue="111">operators</del><ins onMouseEnter="mouseEnter(this)" data-issue="111">objects</ins>. These streams shall be associated with glyph names. A separate encoding entry shall map character codes to the appropriate glyph names for the glyphs.
</p>

<p class="hangingindent">
NOTE 1 Type 3 fonts are more flexible than Type 1 fonts because the glyph descriptions can contain arbitrary PDF graphics operators. However, Type 3 fonts have no hinting mechanism for improving output at small sizes or low resolutions.
</p>

<p class="location">Insert a new NOTE 2 and a new paragraph below NOTE 1 as follows:</p>

<p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="111">NOTE 2 Type 3 glyphs can use any PDF operator from any operator category (see "Table 50 - Operator categories" and "Figure 9 - Graphics objects") subject to additional restrictions described in this clause. </ins></p>

<p><ins onMouseEnter="mouseEnter(this)" data-issue="111">Implementations also need to avoid potential infinite recursion if a Type 3 glyph description refers to itself directly or indirectly. The result in all such cases is implementation-dependent.</ins></p>

<p class="editornote">EDITOR NOTE: remaining NOTEs in this clause will be renumbered appropriately.</p>

<p>...</p>

<p class="location">Change Table 111 as follows:</p>

<table>
  <caption id="Table111">Table 111 - Type 3 font operators</caption>
  <tr>
    <th>Operands</th>
    <th>Operator</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><i>w<sub>x</sub> w<sub>y</sub></i></td>
    <td><b>d0</b></td>
    <td>
    <p>...</p>
    <p>
    <ins onMouseEnter="mouseEnter(this)" data-issue="43">The number</ins> <i>w<sub>x</sub></i> denotes the horizontal displacement in the glyph coordinate system; it shall be consistent with the corresponding width in the font's
    <b>Widths</b> array. <ins onMouseEnter="mouseEnter(this)" data-issue="43">The number </ins><i>w<sub>y</sub></i> shall be 0 (see 9.2.4, "Glyph positioning and metrics").
    </p>
    <p>...</p>
    </td>
  </tr>
  <tr>
    <td><i>w<sub>x</sub> w<sub>y</sub> ll<sub>x</sub> ll<sub>y</sub> ur<sub>x</sub> ur<sub>y</sub></i></td>
    <td><b>d1</b></td>
    <td>
    <p>...</p>
    <p>
    <ins onMouseEnter="mouseEnter(this)" data-issue="43">The number</ins> <i>w<sub>x</sub></i> denotes the horizontal displacement in the glyph coordinate system; it shall be consistent with the corresponding width in the font's
    <b>Widths</b> array. <ins onMouseEnter="mouseEnter(this)" data-issue="43">The number</ins> <i>w<sub>y</sub></i> shall be 0 (see 9.2.4, "Glyph positioning and metrics").
    </p>
    <p>
    <ins onMouseEnter="mouseEnter(this)" data-issue="43">The numbers</ins> <i>ll<sub>x</sub></i> and <i>ll<sub>y</sub></i> denote the coordinates of the lower-left corner,
    and <ins onMouseEnter="mouseEnter(this)" data-issue="43">The numbers</ins> <i>ur<sub>x</sub></i> and <i>ur<sub>y</sub></i> denote the upper-right corner, of the glyph bounding box. ...
    </p>
    <p>...</p>
    </td>
  </tr>
</table>

<p class="location">Change the EXAMPLE below Table 111 as follows:</p>

<p>EXAMPLE
This example shows the definition of a Type 3 font with only two glyphs - a filled square and a filled triangle
<del onMouseEnter="mouseEnter(this)" data-issue="44">, selected by the character codes a and b</del>.
<ins onMouseEnter="mouseEnter(this)" data-issue="44">at positions 97 and 98 of the font's <b>Encoding</b> (corresponding to 'a' and 'b' in PDFDocEncoding) in the <b>Tj</b> string operand</ins>.
"Figure 62 - Output from the example" shows the result of showing the string ( ababab ) using this font.
</p>

<code>
  ...
  <del onMouseEnter="mouseEnter(this)" data-issue="44">%Type 3 font definition encoding two glyphs, 'a' and 'b'</del>
  <ins onMouseEnter="mouseEnter(this)" data-issue="44">%Type 3 font definition encoding the two glyphs square and triangle</ins>
  4 0 obj
     &lt;&lt;
        /Type /Font
        /Subtype /Type3
        /FontBBox [-36 -36 786 786]
        /FontMatrix [0.001 0 0 0.001 0 0]
        /CharProcs 10 0 R
        /Encoding 9 0 R
        /FirstChar 97
        /LastChar <del onMouseEnter="mouseEnter(this)" data-issue="144">144</del><ins onMouseEnter="mouseEnter(this)" data-issue="144">98</ins>
        /Widths [1000 1000]
     &gt;&gt;
  endobj
  ...
</code>


<h2 id="H9.8">9.8 Font descriptors</h2>


<h3 id="H9.8.1">9.8.1 General</h3>

<p class="location">Change Table 120 as follows:</p>

<table>
  <caption id="Table120">Table 120 - Entries common to all font descriptors</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>FontName</b></td>
    <td>name</td>
    <td>
    (<i>Required <ins onMouseEnter="mouseEnter(this)" data-issue="11">for non-Type 3 fonts</ins></i>)
    The PostScript name of the font. <del onMouseEnter="mouseEnter(this)" data-issue="11">This name shall be the same as the value of <b>BaseFont</b>
    in the font or CIDFont dictionary that refers to this font descriptor.</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="11">For Type 3 fonts that include a <b>Name</b> entry in the Type 3 font dictionary, this name shall match the value of that key. For all fonts other than Type 3 this name shall be the same as the value of <b>BaseFont</b> in the font or CIDFont dictionary that refers to this font descriptor.</ins>
    </td>
  </tr>
</table>


<h4 id="H9.8.3.3">9.8.3.3 FD</h4>

<p class="location">Change the second paragraph below EXAMPLE 1 as follows:</p>

<p>
The key for each entry in an <b>FD</b> dictionary shall be the name of a class of glyphs - that is, a particular subset of the CIDFont's
character collection. The entry's value shall be a font descriptor whose contents shall
<ins onMouseEnter="mouseEnter(this)" data-issue="5">be a subset of the keys defined in "Table 120 - Entries common to all font descriptors" that</ins>
override the font-wide attributes for that class only. This font descriptor
<del onMouseEnter="mouseEnter(this)" data-issue="5">shall contain</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="5">contains</ins>
entries for metric information only; it shall not include <b>FontFile</b>, <b>FontFile2</b>,
<b>FontFile3</b>, or any of the entries listed in
<del onMouseEnter="mouseEnter(this)" data-issue="5">"Table 120 - Entries common to all font descriptors"</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="5">"Table 122 - Additional font descriptor entries for CIDFonts"</ins>.
</p>

<h3 id="H9.10.3">9.10.3 ToUnicode CMaps</h3>

<p class="location">Change the last paragraph in EXAMPLE 2 as follows:</p>

<p>EXAMPLE 2</p>
<p style="margin-left: 40px;">...</p>
<p style="margin-left: 40px;">Finally, the character code &lt;3A 51&gt; is mapped to the Unicode value
<del onMouseEnter="mouseEnter(this)" data-issue="87">UNICODE HAN CHARACTER 'U+2003E'</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="87">CJK UNIFIED IDEOGRAPH-2003E</ins>
(U+2003E), which is expressed by the byte sequence &lt;D840DC3E&gt; in UTF-16BE encoding.
</p>


</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
