---
number: 9
title: Text
---


<html>
<head>
<title>ISO 32000-2:2020 Clause 9: Text</title>
</head>
<body>


{% include iso-style.html %}


<div class="iso32000">


<h1>9. Text</h1>


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


...<br/>

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

</div>


<br/><hr>
<p class="footnote">Last modified: 16 February 2021</p>

</body>
</html>
