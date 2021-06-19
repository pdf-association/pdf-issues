---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 9
title: Text
---

{% include iso-style.html %}
<div class="isostyle">


<h1>{{ page.clause }}. {{ page.title }}</h1>


<h3>9.6.2 Type 1 fonts</h3>


<h4>9.6.2.1 General</h4>


<table>
  <caption>Table 109 - Entries in a Type 1 font dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>FontDescritpor</b></td>
    <td>dictionary</td>
    <td>
    <p>(<i>Required; optional in PDF 1.0-1.7 for the standard 14 fonts; shall be an indirect reference</i>) A font descriptor describing the
    font's metrics other than its glyph widths (see 9.8, "Font descriptors").</p>
    <p><span class="deleted-text">For the standard 14 fonts, the entries <b>FirstChar</b>, <b>LastChar</b>, <b>Widths</b>, and <b>FontDescriptor</b> shall either all be
    present or all be absent. Ordinarily, these dictionary keys may be absent; specifying them enables a standard font to be overridden; see<span class="deleted-tooltiptext">
    Issue #47 and #48</span></span> <span class="new-text">See also<span class="new-tooltiptext">Issue #47 and #48</span></span> 9.6.2.2, "Standard Type 1 fonts (standard 14 fonts) (PDF 1.0-1.7)".</p>
    </td>
  </tr>
</table>


<p>
<span class="deleted-text">
PDF versions 1.0 to 1.7 did not require Type 1 font dictionaries to include <b>FirstChar</b>, <b>LastChar</b>, <b>Widths</b> and <b>FontDescriptor</b> entries
as described in 9.6.2.2, "Standard Type 1 fonts (standard 14 fonts) (PDF 1.0-1.7)". For compatibility reasons PDF processors shall provide glyph widths and font
descriptor data for those standard fonts for use in processing PDF files when the entries are absent.
<span class="deleted-tooltiptext">Issue #47 and #48</span></span>
<span class="new-text">See also 9.6.2.2, "Standard Type 1 fonts (standard 14 fonts) (PDF 1.0-1.7)".<span class="new-tooltiptext">Issue #47 and #48</span></span>
</p>


<p>...</p>

<h4>9.6.2.2 Standard Type 1 fonts (standard 14 fonts) (PDF 1.0-1.7)</h4>

<p>...</p>

<p>
<span class="new-text">NOTE: <span class="new-tooltiptext">Issue #47 and #48</span></span>
In PDF 1.0 to PDF 1.7, the <b>FirstChar</b>, <b>LastChar</b>, <b>Widths</b> and <b>FontDescriptor</b> (see "Table 109 - Entries in a Type 1 font dictionary") were
optional in Type 1 font dictionaries for the standard 14 fonts. PDF processors supporting PDF 1.0 to PDF 1.7 files
<span class="deleted-text">shall<span class="deleted-tooltiptext">Issue #47 and #48</span></span>
<span class="new-text">are required to<span class="new-tooltiptext">Issue #47 and #48</span></span>
have these fonts, or their font metrics and suitable substitution fonts available.</p>

<p><span class="deleted-text">These fonts, or their font metrics and suitable substitution fonts, shall be available to the PDF processor.
<span class="deleted-tooltiptext">Issue #47 and #48</span></span></p>


<h3>9.6.4 Type 3 fonts</h3>


<table>
  <caption>Table 111 - Type 3 font operators</caption>
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
    <span class="new-text">The number<span class="new-tooltiptext">Issue #43</span></span> <i>w<sub>x</sub></i> denotes the horizontal displacement in the glyph coordinate system; it shall be consistent with the corresponding width in the font's
    <b>Widths</b> array. <span class="new-text">The number <span class="new-tooltiptext">Issue #43</span></span><i>w<sub>y</sub></i> shall be 0 (see 9.2.4, "Glyph positioning and metrics").
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
    <span class="new-text">The number<span class="new-tooltiptext">Issue #43</span></span> <i>w<sub>x</sub></i> denotes the horizontal displacement in the glyph coordinate system; it shall be consistent with the corresponding width in the font's
    <b>Widths</b> array. <span class="new-text">The number<span class="new-tooltiptext">Issue #43</span></span> <i>w<sub>y</sub></i> shall be 0 (see 9.2.4, "Glyph positioning and metrics").
    </p>
    <p>
    <span class="new-text">The numbers<span class="new-tooltiptext">Issue #43</span></span> <i>ll<sub>x</sub></i> and <i>ll<sub>y</sub></i> denote the coordinates of the lower-left corner,
    and <span class="new-text">The numbers<span class="new-tooltiptext">Issue #43</span></span> <i>ur<sub>x</sub></i> and <i>ur<sub>y</sub></i> denote the upper-right corner, of the glyph bounding box. ...
    </p>
    <p>...</p>
    </td>
  </tr>
</table>

<p>EXAMPLE
This example shows the definition of a Type 3 font with only two glyphs - a filled square and a filled triangle
<span class="deleted-text">, selected by the character codes a and b<span class="deleted-tooltiptext">Issue #44</span></span>.
<span class="new-text">at positions 97 and 98 of the font's <b>Encoding</b> (corresponding to 'a' and 'b' in PDFDocEncoding) in the <b>Tj</b> string operand<span class="new-tooltiptext">Issue #44</span></span>.
"Figure 62 - Output from the example" shows the result of showing the string ( ababab ) using this font.
</p>

<code>
  <p>...</p>
  <span class="deleted-text">%Type 3 font definition encoding two glyphs, 'a' and 'b'<span class="deleted-tooltiptext">Issue #44</span></span><br/>
  <span class="new-text">%Type 3 font definition encoding the two glyphs square and triangle<span class="new-tooltiptext">Issue #44</span></span><br/>
  4 0 obj<br/>
  &nbsp;&nbsp;&nbsp;&lt;&lt;<br/>
  <p>...</p>
</code>


<h2>9.8 Font descriptors</h2>


<h3>9.8.1 General</h3>


<table>
  <caption>Table 120 - Entries common to all font descriptors</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>FontName</b></td>
    <td>name</td>
    <td>
    (<i>Required <span class="new-text">for non-Type 3 fonts<span class="new-tooltiptext">Issue #11</span></span></i>)
    The PostScript name of the font. <span class="deleted-text">This name shall be the same as the value of <b>BaseFont</b>
    in the font or CIDFont dictionary that refers to this font descriptor.<span class="deleted-tooltiptext">Issue #11</span></span>
    <span class="new-text">For Type 3 fonts that include a <b>Name</b> entry in the Type 3 font dictionary, this name shall match
    the value of that key. For all fonts other than Type 3 this name shall be the same as the value of <b>BaseFont</b> in the font
    or CIDFont dictionary that refers to this font descriptor.<span class="new-tooltiptext">Issue #11</span></span>
    </td>
  </tr>
</table>


<h4>9.8.3.3 FD</h4>


<p>...</p>

<p>
The key for each entry in an <b>FD</b> dictionary shall be the name of a class of glyphs - that is, a particular subset of the CIDFont's
character collection. The entry's value shall be a font descriptor whose contents shall <span class="new-text">be a subset of the keys defined
in "Table 120 - Entries common to all font descriptors" that<span class="new-tooltiptext">Issue #5</span></span> override the font-wide attributes for that
class only. This font descriptor <span class="deleted-text">shall contain<span class="deleted-tooltiptext">Issue #5</span></span><span class="new-text">contains<span
class="new-tooltiptext">Issue #5</span></span> entries for metric information only; it shall not include <b>FontFile</b>, <b>FontFile2</b>,
<b>FontFile3</b>, or any of the entries listed in <span class="deleted-text">"Table 120 - Entries common to all font descriptors"
<span class="deleted-tooltiptext">Issue #5</span></span><span class="new-text">"Table 122 - Additional font descriptor entries for CIDFonts"
<span class="new-tooltiptext">Issue #5</span></span>.
</p>

<h3>9.10.3 ToUnicode CMaps</h3>

<p>...</p>
<p>EXAMPLE 2</p>
<p style="margin-left: 40px;">...</p>
<p style="margin-left: 40px;">Finally, the character code &lt;3A 51&gt; is mapped to the Unicode value
<span class="deleted-text">UNICODE HAN CHARACTER 'U+2003E'<span class="deleted-tooltiptext">Issue #87</span></span>
<span class="new-text">CJK UNIFIED IDEOGRAPH-2003E<span class="new-tooltiptext">Issue #87</span></span>
(U+2003E), which is expressed by the byte sequence &lt;D840DC3E&gt; in UTF-16BE encoding.
</p>


</div>


<hr>
<p class="footnote">Last modified: 18 June 2021</p>
