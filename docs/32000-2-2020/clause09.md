---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 9
title: Text
modified: 15 August 2025
---

<ul class="noprint">
 <li>9.3 Text state parameters and operators
  <ul>
   <li><a href="#H9.3.4">9.3.4 Horizontal scaling</a>
   </li>
   <li><a href="#H9.3.6">9.3.6 Text rendering mode</a>
   </li>
  </ul>
 </li>
 <li>9.4 Text objects
  <ul>
   <li><a href="#H9.4.1">9.4.1 General</a>
   </li>
   <li><a href="#H9.4.2">9.4.2 Text-positioning operators</a>
   </li>
   <li><a href="#H9.4.3">9.4.3 Text-showing operators</a>
   </li>
   <li><a href="#H9.4.4">9.4.4 Text space details</a>
   </li>
  </ul>
 </li>
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
   <li><a href="#H9.6.3">9.6.3 TrueType fonts</a>
   </li>
   <li><a href="#H9.6.4">9.6.4 Type 3 fonts</a>
   </li>
  </ul>
 </li>
 <li>9.7 Composite fonts
  <ul>
   <li><a href="#H9.7.3">9.7.3. CIDSystemInfo dictionaries</a>
   </li>
   <li>9.7.4 CIDFonts
    <ul>
     <li><a href="#H9.7.4.1">9.7.4.1 General</a>
     </li>
    </ul>
   </li>
   <li>9.7.5 CMaps
    <ul>
     <li><a href="#H9.7.5.2">9.7.5.2 Predefined CMaps</a>
     </li>
    </ul>
   </li>
   <li>9.7.6 Type 0 font dictionaries
    <ul>
     <li><a href="#H9.7.6.1">9.7.6.1 General</a>
     </li>
    </ul>
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

<h2>9.3 Text state parameters and operators</h2>

<h3 id="H9.3.4">9.3.4 Horizontal scaling</h3>

<p class="location">Change the first paragraph as follows:</p>

<p>
The horizontal scaling parameter, 𝑇<sub>h</sub>, adjusts the width of glyphs by stretching or compressing them in the horizontal direction. Its value 
<ins onMouseEnter="mouseEnter(this)" data-issue="376" data-iso="approved">is the normalized value of the operand to the <b>Tz</b> operator which</ins> 
shall be specified as a percentage of the normal width of the glyphs, with 100 being the normal width 
<ins onMouseEnter="mouseEnter(this)" data-issue="376" data-iso="approved">of 100%, representing a scaling value of 1.0 for 𝑇<sub>h</sub></ins>. 
The scaling shall apply to the horizontal coordinate in text space, independently of the writing mode. It shall affect both the glyph’s shape and its horizontal displacement (that is, its displacement vector). If the writing mode is horizontal, it shall also affect the spacing parameters 𝑇<sub>c</sub> and 𝑇<sub>w</sub>, as well as any positioning adjustments performed by the <b>TJ</b> operator. "Figure 58 — Horizontal scaling" shows the effect of horizontal scaling.
</p>

<p class="location">Update Figure 58 as follows:</p>

<figure>
    <table style="width:fit-content;">
    <tr>
      <td style="vertical-align:middle;">
        <p><ins onMouseEnter="mouseEnter(this)" data-issue="376" data-iso="approved">100 <b>Tz</b></ins></p>
        <p>𝑇<sub>h</sub> = <del onMouseEnter="mouseEnter(this)" data-issue="376" data-iso="approved">100</del> <ins onMouseEnter="mouseEnter(this)" data-issue="376" data-iso="approved">1.0</ins> (default)</p>
      </td>
      <td style="vertical-align:middle;">
        <p style="font-size:360%; transform:translate(68px,0); -webkit-transform:translate(68px,0); display:inline-block;">Word</p>
      </td>
    </tr>
    <tr>
      <td style="vertical-align:middle;">
        <p><ins onMouseEnter="mouseEnter(this)" data-issue="376" data-iso="approved">50 <b>Tz</b></ins></p>
        <p>𝑇<sub>h</sub> = <del onMouseEnter="mouseEnter(this)" data-issue="376" data-iso="approved">50</del> <ins onMouseEnter="mouseEnter(this)" data-issue="376" data-iso="approved">0.5</ins></p>
      </td>
      <td style="vertical-align:middle;">
        <p style="font-size:360%; transform:scale(0.5,1); -webkit-transform:scale(0.5,1); display:inline-block;">WordWord</p>
      </td>
    </tr>
    </table>
  <figcaption>Figure 58 — Horizontal scaling</figcaption>
</figure>


<h3 id="H9.3.6">9.3.6 Text rendering mode</h3>

<p class="location">Change NOTE 3 as follows:</p>

<p class="hangingindent">
NOTE 3 Certain degenerate glyph sub-paths that are not visible when filled can become apparent when stroking, e.g., a zero<ins onMouseEnter="mouseEnter(this)" data-issue="372" data-iso="approved">-length</ins> line with round end caps will paint a circle according to the current stroke width.
</p>

<p class="location">Change the paragraph below NOTE 3 as follows:</p>

<p>
The <i>e</i> and <i>f</i> components of <del onMouseEnter="mouseEnter(this)" data-issue="372" data-iso="approved"><b>Tm</b></del><ins onMouseEnter="mouseEnter(this)" data-issue="372" data-iso="approved"><i>𝑇<sub>m</sub></i></ins> shall be updated for each glyph drawn when using text rendering mode 3 or 7 in exactly the same way as would be done for other text rendering modes.
</p>

<h2 id="H9.4">9.4 Text objects</h2>

<h3 id="H9.4.1">9.4.1 General</h3>

<p class="location">Append the following paragraph to this sub-clause as follows:</p>

<p><ins onMouseEnter="mouseEnter(this)" data-issue="368" data-iso="approved">
Within a text object, the graphics state stack operators <b>q</b> and <b>Q</b> (see 8.4.2, "Graphics state stack") shall additionally push and pop 𝑇<sub>m</sub> and 𝑇<sub>lm</sub> as part of the graphics state stack.
</ins></p>


<h3 id="H9.4.2">9.4.2 Text-positioning operators</h3>

<p class="location">Change Table 106 as follows:</p>

<table>
  <caption id="Table106">Table 106 - Text-positioning operators</caption>
  <tr>
    <th>Operands</th>
    <th>Operator</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><b>&#8212;</b></td>
    <td><b>T*</b></td>
    <td>
    <p>Move to the start of the next line. This operator has the same effect as the code</p>
    <p>
      0 <i>-𝑇<sub>l</sub></i> <del onMouseEnter="mouseEnter(this)" data-issue="373" data-iso="approved"><b>TD</b></del><ins onMouseEnter="mouseEnter(this)" data-issue="373" data-iso="approved"><b>Td</b></ins>  
    </p>
    <p>where <i>𝑇<sub>l</sub></i> denotes the current leading parameter in the text state. The negative of <i>𝑇<sub>l</sub></i> is used here because <i>𝑇<sub>l</sub></i> is the text leading expressed as a positive number. Going to the next line entails decreasing the y coordinate.</p>
    </td>
  </tr>
</table>

<h3 id="H9.4.3">9.4.3 Text-showing operators</h3>

<p class="location">Change 4th paragraph below Figure 61 as follows:</p>

<p>
The strings shall conform to the syntax for string objects
<ins onMouseEnter="mouseEnter(this)" data-issue="165" data-iso="approved">(see 7.3.4.2, "Literal strings")</ins>.
<del onMouseEnter="mouseEnter(this)" data-issue="550">When a string is written by enclosing the data in parentheses, bytes whose values are equal to
those of the ASCII characters
<ins onMouseEnter="mouseEnter(this)" data-issue="165" data-iso="approved">CARRIAGE RETURN (0Dh),</ins>
LEFT PARENTHESIS (28h), RIGHT PARENTHESIS (29h),
and REVERSE SOLIDUS (5Ch) (backslash) shall be preceded by a REVERSE SOLIDUS)
character. All other byte values between 0 and 255 may be used in a string object.
These</del> 
<ins onMouseEnter="mouseEnter(this)" data-issue="550">All literal string </ins> rules apply 
<del onMouseEnter="mouseEnter(this)" data-issue="550">to each individual byte in a string object, whether the string</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="550">before the string</ins>
is interpreted by the text-showing operators 
<del onMouseEnter="mouseEnter(this)" data-issue="550">as single-byte or multiple-byte character codes</del>.
</p>

<p>...</p>


<h3 id="H9.4.4">9.4.4 Text space details</h3>

<p class="location">Change NOTE 2 into normative text as follows:</p>

<p><del onMouseEnter="mouseEnter(this)" data-issue="376" data-iso="approved">NOTE 2</del> Conceptually, the entire transformation from text space to device space can be represented by a text rendering matrix, 𝑇<sub>𝑟𝑚</sub>:
</p>
<p style="text-align:center">
<math xmlns="https://www.w3.org/1998/Math/MathML">
 <msub>
  <mrow>
   <mi>T</mi>
  </mrow>
  <mrow>
   <mi>rm</mi>
  </mrow>
 </msub>
 <mo>=</mo>
 <mrow>
   <mo fence="true" stretchy="true">[</mo>
   <mtable>
    <mtr>
     <mtd>
      <msub>
       <mrow>
        <mi>T</mi>
       </mrow>
       <mrow>
        <mi>fs</mi>
       </mrow>
      </msub>
      <mo>×</mo>
      <msub>
       <mrow>
        <mi>T</mi>
       </mrow>
       <mrow>
        <mi>h</mi>
       </mrow>
      </msub>
     </mtd>
     <mtd>
      <mn>0</mn>
     </mtd>
     <mtd>
      <mn>0</mn>
     </mtd>
    </mtr>
    <mtr>
     <mtd>
      <mn>0</mn>
     </mtd>
     <mtd>
      <msub>
       <mrow>
        <mi>T</mi>
       </mrow>
       <mrow>
        <mi>fs</mi>
       </mrow>
      </msub>
     </mtd>
     <mtd>
      <mn>0</mn>
     </mtd>
    </mtr>
    <mtr>
     <mtd>
      <mn>0</mn>
     </mtd>
     <mtd>
      <msub>
       <mrow>
        <mi>T</mi>
       </mrow>
       <mrow>
        <mi>rise</mi>
       </mrow>
      </msub>
     </mtd>
     <mtd>
      <mn>1</mn>
     </mtd>
    </mtr>
   </mtable>
   <mo fence="true" stretchy="true">]</mo>
 </mrow>
 <mo>×</mo>
  <msub>
   <mrow>
    <mi>T</mi>
   </mrow>
   <mrow>
    <mi>m</mi>
   </mrow>
  </msub>
 <mo>×</mo>
 <mi>CTM</mi>
</math>
</p>
<p>
𝑇<sub>𝑟𝑚</sub> is a temporary matrix; conceptually, it is recomputed before each glyph is painted during a text-showing operation.
</p>


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
    <p>(<i>Required; optional in PDF 1.0-1.7 for the standard 14 fonts<del onMouseEnter="mouseEnter(this)" data-issue="106" data-iso="approved">; shall be an indirect reference</del></i>)
    A font descriptor describing the font's metrics other than its glyph widths (see 9.8, "Font descriptors").</p>
    <p>
    <del onMouseEnter="mouseEnter(this)" data-issue="47,48" data-iso="approved,approved">For the standard 14 fonts, the entries <b>FirstChar</b>, <b>LastChar</b>, <b>Widths</b>, and <b>FontDescriptor</b> shall either all be present or all be absent. Ordinarily, these dictionary keys may be absent; specifying them enables a standard font to be overridden; see</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="47,48" data-iso="approved,approved">See also</ins>
    9.6.2.2, "Standard Type 1 fonts (standard 14 fonts) (PDF 1.0-1.7)".
    </p>
    </td>
  </tr>
</table>

<p class="location">Change the paragraph below Table 109 as follows:</p>

<p>
<del onMouseEnter="mouseEnter(this)" data-issue="47,48" data-iso="approved,approved">PDF versions 1.0 to 1.7 did not require Type 1 font dictionaries to include <b>FirstChar</b>, <b>LastChar</b>, <b>Widths</b> and <b>FontDescriptor</b> entries as described in 9.6.2.2, "Standard Type 1 fonts (standard 14 fonts) (PDF 1.0-1.7)". For compatibility reasons PDF processors shall provide glyph widths and font descriptor data for those standard fonts for use in processing PDF files when the entries are absent.</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="47,48" data-iso="approved,approved">See also 9.6.2.2, "Standard Type 1 fonts (standard 14 fonts) (PDF 1.0-1.7)".</ins>
</p>

<p>...</p>

<h4 id="H9.6.2.2">9.6.2.2 Standard Type 1 fonts (standard 14 fonts) (PDF 1.0-1.7)</h4>

<p class="location">Convert the comma list of fonts in the first paragraph to a bulleted list as follows:</p>

<p>
The PostScript language names of 14 Type 1 fonts, known as the standard 14 fonts, are as follows: 
<del onMouseEnter="mouseEnter(this)" data-issue="384" data-iso="approved">Times-Roman, Helvetica, Courier, Symbol, Times-Bold, Helvetica-Bold, Courier-Bold, ZapfDingbats, Times-Italic, Helvetica-Oblique, Courier-Oblique, Times-BoldItalic, Helvetica-BoldOblique, Courier-BoldOblique.</del>
</p>

<ins onMouseEnter="mouseEnter(this)" data-issue="384" data-iso="approved">
<ul>
  <li>Courier</li>
  <li>Courier-Bold</li>
  <li>Courier-BoldOblique</li>
  <li>Courier-Oblique</li>
  <li>Helvetica</li>
  <li>Helvetica-Bold</li>
  <li>Helvetica-BoldOblique</li>
  <li>Helvetica-Oblique</li>
  <li>Symbol</li>
  <li>Times-Bold</li>
  <li>Times-BoldItalic</li>
  <li>Times-Italic</li>
  <li>Times-Roman</li>
  <li>ZapfDingbats</li>
</ul>
</ins>

<p class="location">Change the second paragraph to a NOTE and modify as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="47,48" data-iso="approved,approved">NOTE: </ins>
In PDF 1.0 to PDF 1.7, the <b>FirstChar</b>, <b>LastChar</b>, <b>Widths</b> and <b>FontDescriptor</b> (see "Table 109 - Entries in a Type 1 font dictionary") were
optional in Type 1 font dictionaries for the standard 14 fonts. PDF processors supporting PDF 1.0 to PDF 1.7 files
<del onMouseEnter="mouseEnter(this)" data-issue="47,48" data-iso="approved,approved">shall</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="47,48" data-iso="approved,approved">are required to</ins>
have these fonts, or their font metrics and suitable substitution fonts available.</p>

<p class="location">Delete the last paragraph as follows:</p>

<p>
<del onMouseEnter="mouseEnter(this)" data-issue="47,48" data-iso="approved,approved">These fonts, or their font metrics and suitable substitution fonts, shall be available to the PDF processor.</del>
</p>


<h3 id="H9.6.3">9.6.3 TrueType fonts</h3>

<p>...</p>>

<p class="location">Append additional text to the end of the last bullet as follows:</p>

<ol>
  <li>...</li>
  <li>In the absence of a PostScript language name in the "name" table, a PostScript language name should be derived from the name by which the font is known in the host operating system. <ins  onMouseEnter="mouseEnter(this)" data-issue="553">An Adobe technical note provides a specification for Postscript name generation that can be used for instance fonts derived from variable fonts. See Adobe Technical Note #5902: "<i>PostScript Name Generation for Variation Fonts</i>".</ins>
  </li>
</ol>

<p>...</p>>

<h3 id="H9.6.4">9.6.4 Type 3 fonts</h3>

<p class="location">Change the first paragraph as follows:</p>

<p>
Type 3 fonts differ from the other fonts supported by PDF. Font dictionaries for other fonts simply contain information about the font and refer to a separate font program for the actual glyph descriptions; a Type 3 font dictionary contains the glyph descriptions. In Type 3 fonts, glyphs shall be defined by streams of PDF graphics <del onMouseEnter="mouseEnter(this)" data-issue="111" data-iso="approved">operators</del><ins onMouseEnter="mouseEnter(this)" data-issue="111" data-iso="approved">objects</ins>. These streams shall be associated with glyph names. A separate encoding entry shall map character codes to the appropriate glyph names for the glyphs.
</p>

<p class="hangingindent">
NOTE 1 Type 3 fonts are more flexible than Type 1 fonts because the glyph descriptions can contain arbitrary PDF graphics operators. However, Type 3 fonts have no hinting mechanism for improving output at small sizes or low resolutions.
</p>

<p class="location">Insert a new NOTE 2 and a new paragraph below NOTE 1 as follows:</p>

<p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="111" data-iso="approved">NOTE 2 Type 3 glyphs can use any PDF operator from any operator category (see "Table 50 - Operator categories" and "Figure 9 - Graphics objects") subject to additional restrictions described in this clause. </ins></p>

<p><ins onMouseEnter="mouseEnter(this)" data-issue="111" data-iso="approved">Implementations also need to avoid potential infinite recursion if a Type 3 glyph description refers to itself directly or indirectly. The result in all such cases is implementation-dependent.</ins></p>

<p class="editornote">EDITOR NOTE: remaining NOTEs in this clause will be renumbered appropriately.</p>

<p>...</p>

<p class="location">Change Table 110 as follows:</p>

<table>
  <caption id="Table110">Table 110 - Entries in a Type 3 font dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>FontDescriptor</b></td>
    <td>dictionary</td>
    <td>
    <p>(<i>Required in Tagged PDF documents<del onMouseEnter="mouseEnter(this)" data-issue="106" data-iso="approved">; shall be an indirect reference</del></i>) ...
    </p>
    </td>
  </tr>
  <tr>
    <td><b>Resources</b></td>
    <td>dictionary</td>
    <td>
    <p><del onMouseEnter="mouseEnter(this)" data-issue="128" data-iso="approved">(<i>Optional but should be used; PDF 1.2</i>) A list of the named resources, such as fonts and images, required by the glyph descriptions in this font (see 7.8.3, "Resource dictionaries"). 
    If any glyph descriptions refer to named resources but this dictionary is absent, the names shall be looked up in the resource dictionary of the page on which the font is used.</del><br/>
    <ins onMouseEnter="mouseEnter(this)" data-issue="128" data-iso="approved">(<i>Optional; PDF 1.2</i>) Named resources, such as fonts and images, directly required by the glyph description content streams of this Type 3 font (see 7.8.3, "Resource dictionaries").</ins>
    </p>
    </td>
  </tr>
</table>

<p class="location">Change bullet (d) in the list below Table 110 as follows:</p>

<ol type="a" start="4">
 <li><del onMouseEnter="mouseEnter(this)" data-issue="128" data-iso="approved">If any glyph descriptions refer to named resources they shall be looked up in the <b>Resources</b> entry of the Type 3 font dictionary. If any glyph descriptions refer to named resources but this dictionary is absent, the names shall be looked up in the resource dictionary of the page on which the font is used.</del><br/>
 <ins onMouseEnter="mouseEnter(this)" data-issue="128" data-iso="approved">If a glyph description content stream refers to named resources they shall be looked up in the designated resource dictionary as described in subclause 7.8.3 "Resource dictionaries".</ins>
 </li>
</ol>

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
    <ins onMouseEnter="mouseEnter(this)" data-issue="43" data-iso="approved">The number</ins> <i>w<sub>x</sub></i> denotes the horizontal displacement in the glyph coordinate system; it shall be consistent with the corresponding width in the font's
    <b>Widths</b> array. <ins onMouseEnter="mouseEnter(this)" data-issue="43" data-iso="approved">The number </ins><i>w<sub>y</sub></i> shall be 0 (see 9.2.4, "Glyph positioning and metrics").
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
    <ins onMouseEnter="mouseEnter(this)" data-issue="43" data-iso="approved">The number</ins> <i>w<sub>x</sub></i> denotes the horizontal displacement in the glyph coordinate system; it shall be consistent with the corresponding width in the font's
    <b>Widths</b> array. <ins onMouseEnter="mouseEnter(this)" data-issue="43" data-iso="approved">The number</ins> <i>w<sub>y</sub></i> shall be 0 (see 9.2.4, "Glyph positioning and metrics").
    </p>
    <p>
    <ins onMouseEnter="mouseEnter(this)" data-issue="43" data-iso="approved">The numbers</ins> <i>ll<sub>x</sub></i> and <i>ll<sub>y</sub></i> denote the coordinates of the lower-left corner,
    and <ins onMouseEnter="mouseEnter(this)" data-issue="43" data-iso="approved">The numbers</ins> <i>ur<sub>x</sub></i> and <i>ur<sub>y</sub></i> denote the upper-right corner, of the glyph bounding box. ...
    </p>
    <p>...</p>
    </td>
  </tr>
</table>

<p class="location">Change the EXAMPLE below Table 111 as follows:</p>

<p>EXAMPLE
This example shows the definition of a Type 3 font with only two glyphs - a filled square and a filled triangle
<del onMouseEnter="mouseEnter(this)" data-issue="44" data-iso="approved">, selected by the character codes a and b</del>.
<ins onMouseEnter="mouseEnter(this)" data-issue="44" data-iso="approved">at positions 97 and 98 of the font's <b>Encoding</b> (corresponding to 'a' and 'b' in PDFDocEncoding) in the <b>Tj</b> string operand</ins>.
"Figure 62 - Output from the example" shows the result of showing the string ( ababab ) using this font.
</p>

<code>
  ...
  <del onMouseEnter="mouseEnter(this)" data-issue="44" data-iso="approved">%Type 3 font definition encoding two glyphs, 'a' and 'b'</del>
  <ins onMouseEnter="mouseEnter(this)" data-issue="44" data-iso="approved">%Type 3 font definition encoding the two glyphs square and triangle</ins>
  4 0 obj
     &lt;&lt;
        /Type /Font
        /Subtype /Type3
        /FontBBox [-36 -36 786 786]
        /FontMatrix [0.001 0 0 0.001 0 0]
        /CharProcs 10 0 R
        /Encoding 9 0 R
        /FirstChar 97
        /LastChar <del onMouseEnter="mouseEnter(this)" data-issue="144" data-iso="approved">144</del><ins onMouseEnter="mouseEnter(this)" data-issue="144" data-iso="approved">98</ins>
        /Widths [1000 1000]
     &gt;&gt;
  endobj
  ...
</code>


<h2 id="H9.7">9.7 Composite fonts</h2>

<h3 id="H9.7.3">9.7.3 CIDSystemInfo dictionaries</h3>

<p class="location">Change the second paragraph as follows:</p>

<p>
The <b>CIDSystemInfo</b> entry in a CIDFont is a dictionary that shall specify the CIDFont’s character collection. 
The CIDFont need not contain glyph descriptions for all the CIDs in a collection; it may contain a subset. 
The <b>CIDSystemInfo</b> entry in a CMap file shall be 
<del onMouseEnter="mouseEnter(this)" data-issue="518" data-iso="approved">either</del> a single dictionary
<del onMouseEnter="mouseEnter(this)" data-issue="518" data-iso="approved">or an array of dictionaries, depending on whether it associates codes with a single character collection or with multiple character collections</del>; see 9.7.5, "CMaps".
</p>


<h3 id="H9.7.4">9.7.4 CIDFonts</h3>

<h4 id="H9.7.4.1">9.7.4.1 General</h4>

<p class="location">Change Table 115 as follows:</p>

<table>
  <caption id="Table115">Table 115 - Entries in a CIDFont dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>FontDescriptor</b></td>
    <td>dictionary</td>
    <td>
    <p>(<i>Required<del onMouseEnter="mouseEnter(this)" data-issue="106" data-iso="approved">; shall be an indirect reference</del></i>) ...
    </p>
    </td>
  </tr>
</table>

<h3 id="H9.7.5">9.7.5 CMaps</h3>

<h4 id="H9.7.5.2">9.7.5.2 Predefined CMaps</h4>

<p class="location">Change the paragraph after Table 117 as follows:</p>

<p>
A PDF processor shall support Adobe-CNS1-7, Adobe-GB1-5, Adobe-Japan1-7 and Adobe-KR-9 character collections.
<del onMouseEnter="mouseEnter(this)" data-issue="278" data-iso="approved">".</del> 
Adobe-Japan2-0 and Adobe-Korea1-2 are deprecated in this document (2020). As noted in 9.7.3, "CIDSystemInfo dictionaries", a character collection is identified
by registry, ordering, and supplement number, and supplements are cumulative; that is, a higher-numbered supplement includes the CIDs contained in
lower-numbered supplements, as well as some additional CIDs. Consequently, text encoded according to the predefined CMaps for a given PDF version shall be 
valid when interpreted by a PDF processor supporting the same or a later PDF version. When interpreted by a PDF processor supporting an earlier PDF version,
such text causes an error if a CMap is encountered that is not predefined for that PDF version. If character codes are encountered that were added in
a higher-numbered supplement than the one corresponding to the supported PDF version, no characters are displayed for those codes; see 9.7.6.3, 
"Handling undefined characters".
</p>


<h3 id="H9.7.6">9.7.6 Type 0 font dictionaries</h3>

<h4 id="H9.7.6.1">9.7.6.1 General</h4>

<p class="location">Change Table 119 as follows:</p>

<table>
  <caption id="Table119">Table 119 - Entries in a Type 0 font dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>ToUnicode</b></td>
    <td>stream</td>
    <td>
    <i>(Optional)</i> A stream containing a CMap file that maps character codes to Unicode values (see 
    <del onMouseEnter="mouseEnter(this)" data-issue="324" data-iso="approved">9.9.2, "Font subsets"</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="324" data-iso="approved">9.10, "Extraction of Text Content"</ins>
    ).
    </td>
  </tr>
</table>

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
    (<i>Required <ins onMouseEnter="mouseEnter(this)" data-issue="11" data-iso="approved">for non-Type 3 fonts</ins></i>)
    The PostScript name of the font. <del onMouseEnter="mouseEnter(this)" data-issue="11" data-iso="approved">This name shall be the same as the value of <b>BaseFont</b>
    in the font or CIDFont dictionary that refers to this font descriptor.</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="11" data-iso="approved">For Type 3 fonts that include a <b>Name</b> entry in the Type 3 font dictionary, this name shall match the value of that key. For all fonts other than Type 3 this name shall be the same as the value of <b>BaseFont</b> in the font or CIDFont dictionary that refers to this font descriptor.</ins>
    </td>
  </tr>
  <tr>
    <td><b>FontWeight</b></td>
    <td><del onMouseEnter="mouseEnter(this)" data-issue="152" data-iso="approved">number</del> <ins onMouseEnter="mouseEnter(this)" data-issue="152" data-iso="approved">integer</ins></td>
    <td>
      <p>(<i>Optional; PDF 1.5</i>) The weight (thickness) component of the fully-qualified font name or font specifier. If present, 
      the value shall 
      <ins onMouseEnter="mouseEnter(this)" data-issue="474" data-iso="approved">be between 1 and 1000 inclusive, and should</ins>
      be one of 100, 200, 300, 400, 500, 600, 700, 800, or 900, where each number indicates a weight that is at least as dark as its predecessor.
      A value of 400 shall indicate a normal weight; 700 shall indicate bold.
      The specific interpretation of these values varies from font to font.
      </p>
      <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="178" data-iso="approved">NOTE The definition of <b>FontWeight</b>
      in PDF matches the CSS <code>font-weight</code> property.</ins>
      </p>
      <p class="hangingindent">
      EXAMPLE 3 300 in one font might appear most similar to 500 in another.
      </p>
    </td>
  </tr>
  <tr>
    <td><b>Descent</b></td>
    <td>number</td>
    <td>
    <p>(<i>Required, except for Type 3 fonts</i>) The maximum depth below the baseline reached by glyphs in this font.
    The value shall be a <del onMouseEnter="mouseEnter(this)" data-issue="190" data-iso="approved">negative</del> number <ins onMouseEnter="mouseEnter(this)" data-issue="190" data-iso="approved">less than or equal to zero</ins>.
    </p>
    <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="190" data-iso="approved">NOTE While different font programs may define descender metrics using either positive or negative numbers (e.g. <a href="https://docs.microsoft.com/en-us/typography/opentype/spec/os2#uswindescent">OpenType usWinDescent</a>), PDF always expects negative values.   
    </ins></p>
    </td>
  </tr>
  <tr>
    <td><b>MissingWidth</b></td>
    <td>number</td>
    <td>
      (<i>Optional</i>) The width to use for character codes whose widths are not specified in a font dictionary’s <b>Widths</b> array. 
      <del onMouseEnter="mouseEnter(this)" data-issue="453" data-iso="approved">This shall have a predictable effect only if all such codes map to glyphs whose actual widths are the same as the value of the <b>MissingWidth</b> entry.</del>
      <ins onMouseEnter="mouseEnter(this)" data-issue="453" data-iso="approved">To ensure predictable results, all such codes must map to glyphs whose actual widths are the same as the value of the <b>MissingWidth</b> entry - otherwise results are implementation dependent.</ins> 
      Default value: <i>0</i>.
    </td>
  </tr>
</table>

<p>...</p>

<p class="location">Add a new NOTE to the very end of clause 9.8.1 as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="337" data-iso="approved">NOTE: if the font descriptor is for an embedded font, then all fields of the descriptor are for that specific embedded (full or subset) font program. If it is for a referenced (non-embedded) font, then it applies to the source material found by the PDF Writer at the time of PDF creation.</ins>
</p>


<h4 id="H9.8.3.3">9.8.3.3 FD</h4>

<p class="location">Change the second paragraph below EXAMPLE 1 as follows:</p>

<p>
The key for each entry in an <b>FD</b> dictionary shall be the name of a class of glyphs - that is, a particular subset of the CIDFont's
character collection. The entry's value shall be a font descriptor whose contents shall
<ins onMouseEnter="mouseEnter(this)" data-issue="5" data-iso="approved">be a subset of the keys defined in "Table 120 - Entries common to all font descriptors" that</ins>
override the font-wide attributes for that class only. This font descriptor
<del onMouseEnter="mouseEnter(this)" data-issue="5" data-iso="approved">shall contain</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="5" data-iso="approved">contains</ins>
entries for metric information only; it shall not include <b>FontFile</b>, <b>FontFile2</b>,
<b>FontFile3</b>, or any of the entries listed in
<del onMouseEnter="mouseEnter(this)" data-issue="5" data-iso="approved">"Table 120 - Entries common to all font descriptors"</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="5" data-iso="approved">"Table 122 - Additional font descriptor entries for CIDFonts"</ins>.
</p>

<h3 id="H9.10.3">9.10.3 ToUnicode CMaps</h3>

<p class="location">Change the first paragraph and bullet list as follows:</p>

<p>
The CMap defined in the <b>ToUnicode</b> entry of the font dictionary shall follow the syntax for CMaps introduced in 9.7.5, "CMaps" and fully documented in Adobe Technical Note #5014, <i>Adobe CMap and CIDFont Files Specification</i>. 
<ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">The <b>ToUnicode</b> stream dictionary contains the entries list in "Table 125a - Additional entries in a ToUnicode CMap stream dictionary".</ins>
This CMap differs from an ordinary one in these ways:
</p>

<ul>
  <li>
    <del onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">The only pertinent entry in the CMap stream dictionary (see "Table 118 — Additional entries in a CMap stream dictionary") is</del>
    <b>UseCMap</b><del onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">, which</del> may be used if the CMap is based on another <b>ToUnicode</b> CMap.</li>
  <li>...</li>
  <li>...</li>
</ul>

<p class="location">Insert a new table (Table 125a) after the bulleted list as follows:</p>


<table>
  <caption id="Table125a"><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">Table 125a - Additional entries in a ToUnicode CMap stream dictionary</ins></caption>
  <tr>
    <th><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">Key</ins></th>
    <th><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">Type</ins></th>
    <th><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">Value</ins></th>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved"><b>Type</b></ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">name</ins></td>
    <td>
      <ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">
      (<i>Optional</i>) The type of PDF object that this dictionary describes; shall be <b>CMap</b> for a ToUnicode CMap dictionary.
      </ins>
    </td>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved"><b>CMapName</b></ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">name</ins></td>
    <td>
      <ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">
      (<i>Optional</i>) The name of the CMap. It shall be the same as the value of <b>CMapName</b> in the ToUnicode CMap data.
      </ins>
    </td>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved"><b>CIDSystemInfo</b></ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">dictionary</ins></td>
    <td>
      <ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">
      (<i>Optional</i>) A dictionary (see 9.7.3, "CIDSystemInfo dictionaries") containing entries that define the character collection for the CIDFont or CIDFonts associated with the CMap. The value of this entry shall be the same as the value of <b>CIDSystemInfo</b> in the ToUnicode CMap data. (However, it does not need to match the values of <b>CIDSystemInfo</b> for the <i>Identity-H</i> or <i>Identity-V</i> CMaps.)
      </ins>
    </td>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved"><b>WMode</b></ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">integer</ins></td>
    <td>
      <ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">
      (<i>Optional</i>) A code that specifies the writing mode for any CIDFont with which this CMap is combined. The value shall be 0 for horizontal or 1 for vertical. Default value: 0. The value of this entry shall be the same as the value of <b>WMode</b> in the CMap file.
      </ins>
    </td>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved"><b>UseCMap</b></ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">name or stream</ins></td>
    <td>
      <ins onMouseEnter="mouseEnter(this)" data-issue="462" data-iso="approved">
      (<i>Optional</i>) The name of a predefined CMap, or a stream containing a CMap. If this entry is present, the referencing CMap shall specify only the character mappings that differ from the referenced CMap.
      </ins>
    </td>
  </tr>
</table>

<p>...</p>

<p class="location">Change the last paragraph in EXAMPLE 2 as follows:</p>

<p>EXAMPLE 2</p>
<p style="margin-left: 40px;">...</p>
<p style="margin-left: 40px;">Finally, the character code &lt;3A 51&gt; is mapped to the Unicode value
<del onMouseEnter="mouseEnter(this)" data-issue="87" data-iso="approved">UNICODE HAN CHARACTER 'U+2003E'</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="87" data-iso="approved">CJK UNIFIED IDEOGRAPH-2003E</ins>
(U+2003E), which is expressed by the byte sequence &lt;D840DC3E&gt; in UTF-16BE encoding.
</p>


<p class="location">Add the following note below the third paragraph below EXAMPLE 2 as follows:</p>

<p>...</p>
<p>In this case, the last byte of the string shall be incremented for each consecutive code in the source code range.</p>
<p>When defining ranges of this type, the value of the last byte in the string shall be less than or equal to 255 - (<i>srcCode2 - srcCode1</i>). This ensures that the last byte of the string shall not be incremented past 255; otherwise, the result of mapping is undefined.</p>

<ins onMouseEnter="mouseEnter(this)" data-issue="277" data-iso="approved">
<p class="hangingindent">NOTE the above requirements are specific to PDF and are not described in Adobe Technical Note #5411 "ToUnicode Mapping File Tutorial".</p>
</ins>

</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
