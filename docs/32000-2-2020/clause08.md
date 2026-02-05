---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
title: 8. Graphics
last_modified_date: 16 January 2026
parent: ISO 32000-2:2020 PDF 2.0
nav_order: 8
---

<nav class="subclauses">
<ul class="noprint">
 <li><a href="#H8.2">8.2 Graphics objects</a>
 </li>
 <li>8.4 Graphics state
  <ul>
   <li><a href="#H8.4.1">8.4.1 General</a>
   </li>
   <li><a href="#H8.4.2">8.4.2 Graphics state stack</a>
   </li>
   <li>8.4.3 Details of graphics state parameters
    <ul>
     <li><a href="#H8.4.3.5">Miter limit</a>
     </li>
    </ul>
   </li>
   <li><a href="#H8.4.4">8.4.4 Graphics state operators</a>
   </li>
   <li><a href="#H8.4.5">8.4.5 Graphics state parameter dictionaries</a>
   </li>
  </ul>
 </li>
 <li>8.5 Path construction and painting
  <ul>
   <li>8.5.3 Path-painting operators
    <ul>
     <li><a href="#H8.5.3.1">8.5.3.1 General</a>
     </li>
    </ul>
   </li>
  </ul>
 </li>
 <li>8.6 Colour spaces
  <ul>
   <li>8.6.5 CIE-Based colour spaces
    <ul>
     <li><a href="#H8.6.5.5">8.6.5.5 ICCBased colour spaces</a>
     </li>
     <li><a href="#H8.6.5.8">8.6.5.8 Rendering intents</a>
     </li>
    </ul>
   </li>
   <li>8.6.6 Special colour spaces
    <ul>
     <li><a href="#H8.6.6.5">8.6.6.5 DeviceN colour spaces</a>
     </li>
    </ul>
   </li>
   <li><a href="#H8.6.8">8.6.8 Colour operators</a>
   </li>
  </ul>
 </li>
 <li>8.7 Patterns
  <ul>
   <li>8.7.3 Tiling patterns
    <ul>
     <li><a href="#H8.7.3.1">8.7.3.1 General</a>
     </li>
    </ul>
   </li>
   <li>8.7.4 Shading patterns
    <ul>
     <li>8.7.4.5 Shading types
      <ul>
       <li><a href="#H8.7.4.5.8">8.7.4.5.8 Type 7 (tensor-product patch mesh) shadings</a>
       </li>
      </ul>
     </li>
    </ul>
   </li>
  </ul>
 </li>
 <li>8.9 Images
  <ul>
   <li>8.9.5 Image dictionaries
    <ul>
     <li><a href="#H8.9.5.1">8.9.5.1 General</a>
     </li>
     <li><a href="#H8.9.5.4">8.9.5.4 Alternate images</a>
     </li>
    </ul>
   </li>
   <li>8.9.6 Masked images
    <ul>
     <li><a href="#H8.9.6.2">8.9.6.2 Stencil masking</a>
     </li>
    </ul> 
   </li>
   <li><a href="#H8.9.7">8.9.7 Inline images</a>
   </li>
  </ul>
 </li>
 <li>8.10 Form XObjects
  <ul>
   <li><a href="#H8.10.2">8.10.2 Form dictionaries</a>
   </li>
  </ul>
 </li>
 <li>8.11 Optional Content
  <ul>
   <li>8.11.3 Making graphical content optional
    <ul>
     <li><a href="#H8.11.3.2">8.11.3.2 Optional content in content streams</a>
     </li>
    </ul>
   </li>
   <li>8.11.4 Configuring optional content
    <ul>
     <li><a href="#H8.11.4.3">8.11.4.3 Optional content configuration dictionaries</a>
     </li>
     <li><a href="#H8.11.4.4">8.11.4.4 Usage and usage application dictionaries</a>
     </li>
    </ul>
   </li>
  </ul>
 </li>
</ul>
</nav>
<hr>

<div class="isostyle">
<div class="fixedpopup" id="issuelink">
    Issue #xxxx
</div>

<p class="fake-h1">{{ page.title }}</p>

<h2 id="H8.2">8.2 Graphics objects</h2>

<p class="location">Change Table 50 as follows:</p>

<table>
  <caption id="Table50">Table 50 - Operator categories</caption>
  <tr>
    <th>Category</th>
    <th>Operators</th>
    <th>Location</th>
  </tr>
  <tr>
    <td>Shading patterns</td>
    <td>
    <del onMouseEnter="mouseEnter(this)" data-issue="80" data-iso="approved"><b>Sh</b></del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="80" data-iso="approved"><b>sh</b></ins>
    </td>
    <td>"Table 76 — Shading operator"
    </td>
  </tr>
  <tr>
    <td>...</td>
    <td>...</td>
    <td>...</td>
  </tr>
  <tr>
    <td>Marked-content</td>
    <td><b>MP, DP, BMC, BDC, EMC</b></td>
    <td>
    <del onMouseEnter="mouseEnter(this)" data-issue="85" data-iso="approved">"Table 351 — Entries in a data dictionary"</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="85" data-iso="approved">"Table 352 — Marked-content operators"</ins>
    </td>
  </tr>
</table>

<h2 id="H8.4">8.4 Graphics state</h2>

<h3 id="H8.4.1">8.4.1 General</h3>

<p class="location">Add the following row to Table 52 below the Haftone entry as follows:</p>

<table>
  <caption id="Table52">Table 52 - Device-dependent graphics state parameters</caption>
  <tr>
    <th>Parameter</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>flatness</b></td>
    <td>number</td>
    <td>
    The precision with which curves shall be rendered on the output device (see 10.7.2, "Flatness tolerance"). The value of this parameter <del onMouseEnter="mouseEnter(this)" data-issue="371" data-iso="approved">(positive number)</del> gives the maximum error tolerance, measured in output device pixels; smaller numbers give smoother curves at the expense of more computation and memory use. Initial value: <i>1.0</i>.
    </td>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="260" data-iso="approved">halftone origin</ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="260" data-iso="approved">array</ins></td>
    <td>
    <ins onMouseEnter="mouseEnter(this)" data-issue="260" data-iso="approved">
    (<i>PDF 2.0</i>) The X and Y coordinates of the halftone origin. Initial value: a PDF reader shall initialise this to a suitable device dependent value.
    </ins>
    </td>
  </tr>
</table>


<h3 id="H8.4.2">8.4.2 Graphics state stack</h3>

<p class="location">Append a new sentence to the last paragraph as follows:</p>

<p>
Occurrences of the <b>q</b> and <b>Q</b> operators shall be balanced within a given content stream (or within the sequence of streams specified in a page dictionary’s <b>Contents</b> array).
<ins onMouseEnter="mouseEnter(this)" data-issue="368" data-iso="approved">See 9.4.1, "General" for additional information that must be managed as part of the graphics state stack when <b>q</b> and <b>Q</b> operators occur within text objects.</ins>
</p>


<h3 id="H8.4.3">8.4.3 Details of graphics state parameters</h3>

<h4 id="H8.4.3.5">8.4.3.5 Mitre limit</h4>

<p class="location">Change the first paragraph as follows:</p>

<p>
When two line segments meet at a sharp angle and mitered joins have been specified as the
line join style, it is possible for the miter to extend far beyond the thickness of the
line stroking the path. The miter limit
<ins onMouseEnter="mouseEnter(this)" data-issue="154" data-iso="approved">shall be a number greater than or equal to 1.0 and</ins>
shall impose a maximum on the ratio of the miter length to the line width (see
"Figure 15 — Miter length"). When the limit is exceeded, the join is converted from
a miter to a bevel.
</p>

<p>...</p>

<h3 id="H8.4.4">8.4.4 Graphics state operators</h3>

<p class="location">Change Table 56 as follows:</p>

<table>
  <caption id="Table56">Table 56 - Graphics state operators</caption>
  <tr>
    <th>Operands</th>
    <th>Operator</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><i>flatness</i></td>
    <td><b>i</b></td>
    <td>
      Set the flatness tolerance in the graphics state (see 10.7.2, "Flatness tolerance"). <del onMouseEnter="mouseEnter(this)" data-issue="371" data-iso="approved"><i>flatness</i> is a number in the range 0 to 100; a value of 0 shall specify the output device’s default flatness tolerance.</del>
    </td>
  </tr>
</table>


<h3 id="H8.4.5">8.4.5 Graphics state parameter dictionaries</h3>

<p class="location">Change Table 57 as follows:</p>

<table>
  <caption id="Table57">Table 57 - Entries in a graphics state parameter dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>UseBlackPtComp</b></td>
    <td>name</td>
    <td>
      <p>...</p>
      <p><del onMouseEnter="mouseEnter(this)" data-issue="360" data-iso="approved">The default value is: <i>Default</i>.</del></p>
    </td>
  </tr>
</table>


<h2 id="H8.5">8.5 Path constructing and painting</h2>

<h3 id="H8.5.3">8.5.3 Path-painting operators</h3>

<h4 id="H8.5.3.1">8.5.3.1 General</h4>

<p class="location">Change the first paragraph as follows:</p>

<p>
The path-painting operators end a path object, causing it to be painted on the current page in the manner that the operator specifies. The principal path-painting operators shall be <b>S</b> (for stroking) and <b>f</b> (for filling). Variants of these operators combine stroking and filling in a single operation or apply different rules for determining the area to be filled. Attempting to execute a painting operator when the current path is undefined (at the beginning of a new page or immediately after a painting operator has been executed) shall 
<del onMouseEnter="mouseEnter(this)" data-issue="549">generate an error</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="549">be ignored</ins>. 
"Table 59 — Path-painting operators" lists all the path-painting operators.
</p>

<p class="location">Add a new NOTE above Table 59 as follows:</p>

<p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="434" data-iso="approved">
NOTE: While these operators are primarily for path-painting, they also serve a purpose in path construction as they may affect the current graphics path (see 8.5.2, "Path-construction operators").
</ins></p>

<p class="location">Change Table 59 as follows:</p>

<table>
  <caption id="Table59">Table 59 - Path-painting categories</caption>
  <tr>
    <th>Operands</th>
    <th>Operator</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>-</td>
    <td><b>B</b></td>
    <td>
    <p>Fill and then stroke the path, using the non-zero winding number rule to determine the region to fill.
    <ins onMouseEnter="mouseEnter(this)" data-issue="103" data-iso="approved">In the opaque imaging model, this</ins>
    <del onMouseEnter="mouseEnter(this)" data-issue="103" data-iso="approved">This</del> operator shall produce the same result
    as constructing two identical path objects, painting the first with <b>f</b> and the second with <b>S</b>.</p>
    <p>...</p>
    </td>
  </tr>
</table>


<h4 id="H8.6.5.5">8.6.5.5 ICCBased colour spaces</h4>

<p class="location">Change the first paragraph as follows:</p>
<p>
<b>ICCBased</b> colour spaces (<i>PDF 1.3</i>) shall be based on a cross-platform colour profile as defined by the International Color Consortium (ICC). Unlike the <b>CalGray</b>, <b>CalRGB</b>, and <b>Lab</b> colour spaces, which are characterised by entries in the colour space dictionary, an <b>ICCBased</b> colour space shall be characterised by a sequence of bytes in a standard format. Details of the profile format can be found in the ICC specification<ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">s</ins>.
</p>

<p class="location">Replace the paragraph before Table 66 and Table 66 as follows:</p>

<p>
"Table 66 - <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">ICC Specification versions supported by ICC based colour spaces" shows the versions of the ICC specification on which the
<b>ICCBased</b> colour spaces that PDF versions 1.3 and later shall use. (Earlier versions of the ICC specification shall also be supported.)</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">ICC profile versions supported by <b>ICCBased</b> colour spaces" lists the ICC profile versions as specified in the ICC header that shall be supported.</ins>
</p>

<table>
  <caption id="Table66">Table 66 - <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">ICC Specification versions supported by ICC based colour spaces</del><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">ICC profile versions supported by <b>ICCBased</b> colour spaces</ins></caption>
  <tr>
    <th><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">ICC profile header version</ins></th>
    <th><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">ICC Specification</ins></th>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">2.<i>x.y.z</i></ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">"<i>Specification ICC.1:2001-04 - File Format for Color Profiles [REVISION of ICC.1:1998-09]</i>"</ins></td>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">4.<i>x.y.z</i> where <i>x</i> &le; 3</ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">ISO 15076-1:2010, <i>Image technology colour management – Architecture, profile format and data structure — Part 1: Based on ICC.1:2010</i></ins></td>
  </tr>
</table>

<p class="location">Change the bulleted list below Table 66 as follows:</p>

<p>PDF processors shall follow these guidelines for writing and rendering ICC based color spaces:</p>

<ul>
<li>A PDF reader shall support <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">ICC.1:2010 as required by PDF 2.0</del><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">both ICC profile header version 2.x and 4.x profiles</ins>, which will enable it to properly render all embedded ICC profiles regardless of the PDF version.</li>
<li>A PDF reader shall always process an embedded ICC profile according to the <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">corresponding version of the PDF</del><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">ICC specification</ins> being processed as shown in <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">"ICC Specification versions supported by ICC based colour spaces</del><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">"Table 66 - ICC profile versions supported by <b>ICCBased</b> colour spaces"</ins> above; it shall not substitute the alternate colour space in these cases.</li>
<li>A PDF writer should use ICC <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved">1:2010</del> profiles<ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="approved"> conforming to ISO 15076-1:2010</ins>. It may embed profiles conforming to an earlier or later ICC version.</li> 
<li>...</li>
</ul>

<p class="location">Add a new NOTE 2 below NOTE 1 and above Table 67 as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="228" data-iso="approved">NOTE 2 ICC profiles can contain private tags or tags defined in later versions of ICC profile specifications than specified in "Table 66 - ICC Specification versions supported by ICC based colour spaces". This document intentionally does not specify how a PDF processor might use such data in ICC profiles. A PDF processor can ignore such data altogether. Any use of such data is implementation dependent.</ins>
</p>

<h4 id="H8.6.5.8">8.6.5.8 Rendering intents</h4>
<p class="location">Change the NOTE below Table 69 as follows:</p>


<p class="hangingindent">
NOTE The exact set of rendering intents supported can vary from one output device to another; a particular device
<del onMouseEnter="mouseEnter(this)" data-issue="63" data-iso="approved">does not have to support all PDF rendering intents and</del>
can support additional ones beyond those listed in the table above.
</p>



<h3 id="H8.6.6">8.6.6 Special colour spaces</h3>

<h4 id="H8.6.6.5">8.6.6.5 DeviceN colour spaces</h4>

<p>...</p>

<p class="location">Change the paragraph this is 2 paragraphs above NOTE 4 as follows:</p>

<p>
The component names shall all be different from one another, except for the name <b>None</b>, which may be repeated as described later in this subclause. 
<ins onMouseEnter="mouseEnter(this)" data-issue="309" data-iso="approved">The special name <b>None</b> shall not be used in <b>DeviceN</b> colour spaces that have the <b>NChannel</b> subtype</ins>
The special name <b>All</b>, used by <b>Separation</b> colour spaces, shall not be used. The names <b>Cyan</b>, <b>Magenta</b>, <b>Yellow</b> and <b>Black</b> are reserved to name the subtractive process colourants of a CMYK device.
</p>

<p>...</p>

<p class="location">Change the paragraph below NOTE 6 as follows:</p>

<p>
The colour component name <b>None</b>
<del onMouseEnter="mouseEnter(this)" data-issue="309" data-iso="approved">, which may be present only for <b>DeviceN</b> colour spaces that do not have the <b>NChannel</b> subtype,</del> 
indicates that the corresponding colour component shall never be painted on the page, as in a <b>Separation</b> colour space for the <b>None</b> colourant. When a <b>DeviceN</b> colour space is painting the named device colourants directly, colour components corresponding to <b>None</b> colourants shall be discarded. However, when the <b>DeviceN</b> colour space reverts to its alternate colour space, those components shall be passed to the tint transformation function, which may use them as desired.
</p>


<h3 id="H8.6.8">8.6.8 Colour operators</h3>

<p class="location">Change Table 73 as follows:</p>

<table>
  <caption id="Table73">Table 73 - Colour operators</caption>
  <tr>
    <th>Operands</th>
    <th>Operator</th>
    <th>Description</th>
  </tr>
  <tr>
   <td><i>name</i></td>
   <td><b>CS</b></td>
   <td>
     <p>
      (<i>PDF 1.1</i>) Set the current colour space to use for stroking operations. The operand name shall be a name object. If the colour space is one that can be specified by a name and no additional parameters (<b>DeviceGray</b>, <b>>DeviceRGB</b>, <b>DeviceCMYK</b>, and certain cases of <b>Pattern</b>), the name may be specified directly. Otherwise, it shall be a name defined in the <b>ColorSpace</b> subdictionary of the current resource dictionary (see 7.8.3, "Resource dictionaries")
      <del onMouseEnter="mouseEnter(this)" data-issue="551">; the associated value shall be an array describing the colour space (see 8.6.3, "Colour space families")</del>.
     </p>
     <p>...</p>
   </td>
  </tr>
</table>



<h2 id="H8.7">8.7 Patterns</h2>

<h3 id="H8.7.3">8.7.3 Tiling patterns</h3>

<h4 id="H8.7.3.1">8.7.3.1 General</h4>

<p class="location">Change the second paragraph as follows:</p>

<p>
The pattern cell can include graphical elements such as filled areas, text, and sampled images. Its shape need not be rectangular, and the spacing of tiles can differ from the dimensions of the cell itself. When performing painting operations such as <b>S</b> (stroke) or <b>f</b> (fill), the PDF processor shall paint the cell on the current page as many times as necessary to fill an area. The order in which individual tiles (instances of the cell) are painted is unspecified and unpredictable
<ins onMouseEnter="mouseEnter(this)" data-issue="428" data-iso="approved">(implementation dependent)</ins>
; figures on adjacent tiles should not overlap.
</p>

<p>...</p>

<p class="location">Change the caption of Table 74 as follows:</p>

<table>
  <caption id="Table74">Table 74 - Additional entries specific to a Type 1 pattern <ins onMouseEnter="mouseEnter(this)" data-issue="294" data-iso="approved">stream</ins> dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
   <td>...</td>
   <td>...</td>
   <td>...</td>
  </tr>
</table>

<h3 id="H8.7.4">8.7.4 Shading patterns</h3>

<h4 id="H8.7.4.5">8.7.4.5 Shading types</h4>

<h5 id="H8.7.4.5.8">8.7.4.5.8 Type 7 (tensor-product patch mesh) shadings</h5>

<p class="location">Remove the green line below the matrix that is 2 paragraphs before Table 85 as follows:</p>

<p>The coordinates of the control points in a tensor-product patch shall be specified in the shading’s data stream in the following order:</p>

<table style="margin-left: auto; margin-right: auto; border: none;" cellspacing="0" cellpadding="0">
  <tr>
    <td style="border: none">4</td>
    <td style="border: none">5</td>
    <td style="border: none">6</td>
    <td style="border: none">7</td>
  </tr>
  <tr>
    <td style="border: none">3</td>
    <td style="border: none">14</td>
    <td style="border: none">15</td>
    <td style="border: none">8</td>
  </tr>
  <tr>
    <td style="border: none">2</td>
    <td style="border: none">13</td>
    <td style="border: none">16</td>
    <td style="border: none">9</td>
  </tr>
  <tr>
    <td style="border: none">1</td>
    <td style="border: none">12</td>
    <td style="border: none">11</td>
    <td style="border: none">10</td>
  </tr>
</table>

<p><del onMouseEnter="mouseEnter(this)" data-issue="682">&nbsp;<hr style="color:green; width:80%">&nbsp;</del></p>

<p>...</p>

<h2 id="H8.9">8.9 Images</h2>

<h3 id="H8.9.5">8.9.5 Image dictionaries</h3>

<h4 id="H8.9.5.1">8.9.5.1 General</h4>

<p class="location">Change Table 87 as follows:</p>

<table>
  <caption id="Table87">Table 87 - Additional entries specific to an image dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>BitsPerComponent</b></td>
    <td>integer</td>
    <td>
    <p>
      (<i>Required except for image masks and images that use the <b>JPXDecode</b> filter</i>) The number of bits used to represent each colour component.
      Only a single value shall be specified; the number of bits shall be the same for all colour components. The value shall be <i>1</i>, <i>2</i>, 
      <i>4</i>, <i>8</i>, or (<i>from PDF 1.5</i>) <i>16</i>. If <b>ImageMask</b> is <i>true</i>, this entry is optional, but if specified, its
      value shall be <i>1</i>.
    </p>
    <p>
      If the image stream uses a filter, the value of <b>BitsPerComponent</b> shall be consistent with the size of the data samples that the filter
      delivers. In particular, a <b>CCITTFaxDecode</b> or <b>JBIG2Decode</b> filter shall always deliver 1-bit samples, a <b>RunLengthDecode</b> or
      <b>DCTDecode</b> filter shall always deliver 8-bit samples, and an <b>LZWDecode</b> or <b>FlateDecode</b> filter shall deliver samples of
      <del onMouseEnter="mouseEnter(this)" data-issue="366" data-iso="approved">a</del>
      <ins onMouseEnter="mouseEnter(this)" data-issue="366" data-iso="approved">the</ins> 
      specified size <del onMouseEnter="mouseEnter(this)" data-issue="366" data-iso="approved">if a predictor function is used</del>.
    </p>
    <p>
      If the image stream uses the <b>JPXDecode</b> filter, this entry is optional and shall be ignored if present. The bit depth is determined by 
      the PDF processor in the process of decoding the JPEG 2000 image.
    </p>
    </td>
  </tr>
  <tr>
    <td><b>Intent</b></td>
    <td>name</td>
    <td>
       <p>...</p>
       <p><ins onMouseEnter="mouseEnter(this)" data-issue="13" data-iso="approved">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
       Soft-mask images.</ins></p>
    </td>
  </tr>
  <tr>
    <td><b>ImageMask</b></td>
    <td>boolean</td>
    <td>
      (<i>Optional</i>) A flag indicating whether the image shall be treated as an image mask (see 8.9.6, "Masked images"). 
      If this flag is <i>true</i>,
      the value of <b>BitsPerComponent</b>, if present, shall be 1 and 
      <del onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved">Mask</del>
      <ins onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved"><b>Mask</b></ins> and <b>ColorSpace</b> 
      shall not be 
      <del onMouseEnter="mouseEnter(this)" data-issue="215" data-iso="approved">specified</del><ins onMouseEnter="mouseEnter(this)" data-issue="215" data-iso="approved">present (if present, they shall be ignored)</ins>; 
      unmasked areas shall be painted using the current nonstroking colour. Default value: <i>false</i>.
    </td>
  </tr>
  <tr>
    <td><b>Mask</b></td>
    <td>stream or array</td>
    <td>
      <p>(<i>Optional; shall not be present for image masks; PDF 1.3</i>) 
      An image XObject defining an image mask to be applied to this image (see 8.9.6.3, "Explicit masking"), or an array specifying a range of colours to be applied to it as a colour key mask (see 8.9.6.4, "Colour key masking"). 
      If <b>ImageMask</b> is <i>true</i>, this entry shall not be present
      <ins onMouseEnter="mouseEnter(this)" data-issue="215" data-iso="approved">(if present, it shall be ignored)</ins>.
      </p>
      <p class="hangingindent">
      <ins onMouseEnter="mouseEnter(this)" data-issue="215" data-iso="approved">NOTE Interactions between <b>SMask</b>, <b>SMaskInData</b> and the current soft mask in the graphics state are set out in clause 11.6.4.3, "Mask shape and opacity".</ins>
      </p>
    </td>
  </tr>
  <tr>
    <td><b>Alternates</b></td>
    <td>array</td>
    <td>
      <p>...</p>
      <p><ins onMouseEnter="mouseEnter(this)" data-issue="13" data-iso="approved">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.</ins></p></td>
  </tr>
  <tr>
    <td><b>SMask</b></td>
    <td>stream</td>
    <td>
      <p>(<i>Optional; PDF 1.4</i>) A subsidiary image XObject defining a soft-mask image (see 11.6.5.2, "Soft-mask images") that shall be used
      as a source of mask shape or mask opacity values in the transparent imaging model. The alpha source parameter in the graphics state
      determines whether the mask values shall be interpreted as shape or opacity.
      </p>
      <p>If present, this entry shall override the current soft mask in the graphics state, as well as the image’s <b>Mask</b> entry, if any.
      However, the other transparency-related graphics state parameters — blend mode and alpha constant — shall remain in effect. 
      If <b>SMask</b> is absent and <b>SMaskInData</b> has value 0, the image shall have no associated soft mask (although the current soft mask in the graphics state may still apply). 
      <ins onMouseEnter="mouseEnter(this)" data-issue="215" data-iso="approved"><b>SMask</b> shall not be present if <b>SMaskInData</b> has a non-zero value (if present, <b>SMask</b> shall be ignored).</ins>
      </p>
      <p>
      <ins onMouseEnter="mouseEnter(this)" data-issue="13" data-iso="approved">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2 Soft-mask images.</ins>
      </p>
    </td>
  </tr>
  <tr>
    <td><b>SMaskInData</b></td>
    <td>integer</td>
    <td>
      <p>
        (<i>Optional for images that use the <b>JPXDecode</b> filter, meaningless otherwise; PDF 1.5</i>) A code specifying how soft-mask
        information (see 11.6.5.2, "Soft-mask images") encoded with image samples shall be used:
      </p>
      <ol style="counter-reset: list-item 0;">
        <li>
          If present, encoded soft-mask image information shall be ignored.
          <ins onMouseEnter="mouseEnter(this)" data-issue="215" data-iso="approved">If present, <b>SMask</b> shall override the current soft mask in the graphics state, as well as the image’s <b>Mask</b> entry, if any. However, the other transparency-related graphics state parameters — blend mode and alpha constant — shall remain in effect.</ins>
        </li>
        <li>The image’s data stream includes encoded soft-mask values. A PDF processor shall create a soft-mask image from the information to be used as a source of mask shape or mask opacity in the transparency imaging model.</li>
        <li>The image’s data stream includes colour channels that have been premultiplied with an opacity channel; the image data also includes the opacity channel. A PDF processor shall create a soft-mask image from the opacity channel information to be used as a source of mask shape or mask opacity in the transparency model.</li>
      </ol>
      <p>
        If this entry has a non-zero value, <b>SMask</b> shall not be specified
        <ins onMouseEnter="mouseEnter(this)" data-issue="215" data-iso="approved">(if present, <b>SMask</b> shall be ignored). If <b>SMaskInData</b> is non-zero, 
        there shall be only one opacity channel in the JPEG 2000 data and it shall apply to all colour channels</ins>. 
        See also 7.4.9, "JPXDecode filter".
      </p>
      <p class="hangingindent">
        NOTE 2 Interactions between <b>SMask</b>, <b>SMaskInData</b> and the current soft mask in the graphics state are set out in clause 11.6.4.3, "Mask shape and opacity".
      </p>
      <p>Default value: 0.</p>
    </td>
  </tr>
  <tr>
    <td><b>Name</b></td>
    <td>name</td>
    <td>
      <p>...</p>
      <p>
      <ins onMouseEnter="mouseEnter(this)" data-issue="13" data-iso="approved">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2 Soft-mask images.</ins>
      </p>
    </td>
  </tr>
  <tr>
    <td><b>StructParent</b></td>
    <td>integer</td>
    <td>
      <p>...</p><p><ins onMouseEnter="mouseEnter(this)" data-issue="13" data-iso="approved">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
      Soft-mask images.</ins></p>
    </td>
  </tr>
  <tr>
    <td><b>ID</b></td>
    <td>byte string</td>
    <td>
      <p>(<i>Optional; PDF 1.3; indirect reference preferred<ins onMouseEnter="mouseEnter(this)" data-issue="619">; Deprecated in PDF 2.0</ins></i>) 
      The digital identifier of the image’s parent Web Capture content set (see 14.10.6, "Object attributes related to web capture").</p>
      <p><ins onMouseEnter="mouseEnter(this)" data-issue="13" data-iso="approved">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2, Soft-mask images.</ins></p>
    </td>
  </tr>
</table>

<h4 id="H8.9.5.4">8.9.5.4 Alternate images</h4>

<p class="location">Change the list below Table 89 as follows:</p>

<p>In PDF 1.5, optional content (see 8.11, "Optional content") may be used to facilitate selection between alternate images. The following algorithm shall be used to determine which image, if any, shall be rendered:</p>

<p class="hangingindent">NOTE (2020) The following algorithm was changed in this document to <del onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">reflect that <b>OC</b> processing has precedence over <b>DefaultForPrinting</b> functionality, and situations where no image is to be rendered</del><ins onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">clarify the relationship between optional content and <b>DefaultForPrinting</b></ins>.</p>

<ol class="alphalist" style="counter-reset: list-item 0;">
  <li>
    If the base image contains an <b>OC</b> <del onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">key then <b>DefaultForPrinting</b> shall be ignored on all <b>Alternates</b> entries</del><ins onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">entry that specifies that the content is not visible, then nothing shall be shown</ins>.
  </li>

  <li>
    If the base image contains an <b>OC</b> entry that specifies that the base image is visible, then the base image shall be rendered.
  </li>

  <li style="background-color: seashell; color: darkred; text-decoration: line-through; text-decoration-color: red;">
    <del onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">If the base image contains an <b>OC</b> entry that specifies that the base image is not visible, then the list of alternate image dictionaries specified by the base image <b>Alternates</b> entry shall be examined in order, and the first entry not containing an <b>OC</b> key, or containing an <b>OC</b> entry specifying that the alternate image should be visible, shall be selected. Further, if this selected alternate image has an <b>OC</b> entry, then that <b>OC</b> entry shall also be processed to determine if the alternate image shall be rendered or not. If none of the alternate image dictionaries have an <b>OC</b> key, or none of the alternate image dictionaries with an <b>OC</b> entry specify that that alternate image is visible, then nothing shall be shown. <b>DefaultForPrinting</b> shall be ignored on all <b>Alternates</b> entries.</del>
  </li>

  <li value="3" style="background-color: lightyellow; color: green; text-decoration-style: double; text-decoration-color: green;">
    <ins onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">Otherwise if the PDF is being printed and any of the <b>Alternates</b> entries has <b>DefaultForPrinting</b> set to true, then that alternate image shall be printed.</ins>
  </li>

  <li value ="4" style="background-color: seashell; color: darkred; text-decoration: line-through; text-decoration-color: red;">
    <del onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">If the base image does not contain an <b>OC</b> key and the PDF is being printed then the first entry in the <b>Alternates</b> array of the base image that has <b>DefaultForPrinting</b> set to true shall be selected. Further, if this selected alternate image has an <b>OC</b> entry, then that <b>OC</b> entry shall also be processed to determine if the alternate image shall be printed or not. If no alternate image dictionary in the Alternates array has <b>DefaultForPrinting</b> set to true, then the base image shall be printed.</del>
  </li>

  <li value="4" style="background-color: lightyellow; color: green; text-decoration-style: double; text-decoration-color: green;">
    <ins onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">Otherwise, the list of alternates specified by the base image <b>Alternates</b> entry is examined, and the first alternate containing an <b>OC</b> entry specifying that its content is visible shall be shown (<b>Alternates</b> that have no <b>OC</b> entry shall not be shown.) Furthermore if the image dictionary that forms the value of the <b>Image</b> key of the selected alternate contains an <b>OC</b> entry, then that <b>OC</b> in the image dictionary shall not be examined.</ins>
  </li>

  <li value="5" style="background-color: lightyellow; color: green; text-decoration-style: double; text-decoration-color: green;">
    <ins onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">If steps c and d above do not identify an alternate to be rendered then the base image shall be rendered.</ins>
  </li>
</ol>

<p>...</p>

<h3 id="H8.9.6">8.9.6 Masked images</h3>

<h4 id="H8.9.6.2">8.9.6.2 Stencil masking</h4>

<p>...</p>

<p class="location">Change the NOTE as follows:</p>

<p class="hangingindent">
NOTE One of the most important uses of stencil masking is for painting character glyphs represented as bitmaps. Using such a glyph as a stencil mask transfers only its "black" bits to the page, leaving the "white" bits (which are really just background) unchanged. For reasons discussed in 
<del onMouseEnter="mouseEnter(this)" data-issue="333" data-iso="approved">9.6.5.3, "Encodings for Type 3 fonts"</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="333" data-iso="approved">9.6.4, "Type 3 fonts"</ins>
, an image mask, rather than an image, 
<del onMouseEnter="mouseEnter(this)" data-issue="333" data-iso="approved">need almost always be used to paint glyph bitmaps</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="333" data-iso="approved">is normally used to paint glyph bitmaps</ins>.
</p>


<h3 id="H8.9.7">8.9.7 Inline images</h3>

<p class="location">Change the paragraphs below Table 90 as follows:</p>

<p>
Inline image objects shall not be nested; that is, two <b>BI</b> operators shall not appear without an intervening <b>EI</b> to close the first object.
Similarly, an <b>ID</b> operator shall only appear between a <b>BI</b> and its balancing <b>EI</b>. Unless the image uses <b>ASCIIHexDecode</b> or
<b>ASCII85Decode</b> as <del onMouseEnter="mouseEnter(this)" data-issue="20" data-iso="approved">one of its filters</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="20" data-iso="approved">its final or only filter</ins>, the <b>ID</b> operator shall be followed by a
single white-space character, and the next character shall be interpreted as the first byte of image data.
</p>

<p>
The key-value pairs appearing between the <b>BI</b> and <b>ID</b> operators (as listed in "Table 91 - Entries in an inline
image object") are analogous to their respective key-value pairs in an image XObject dictionary (see "Table 87 - Additional
entries specific to an image dictionary") or a stream dictionary (see "Table 5 - Entries common to all stream dictionaries").
For convenience, the abbreviations shown in "Table 91 - Entries in an inline image object" and "Table 92 - Additional
abbreviations in an inline image object" may be used in place of the full names.
<ins onMouseEnter="mouseEnter(this)" data-issue="3" data-iso="approved">In the situation where both an abbreviated key name and the corresponding full key name from Table 91 are present, the abbreviated key name shall take precedence.</ins>
Entries other than those listed shall be ignored.
</p>

<p>...</p>

<p class="location">Change Table 91 as follows:</p>

<table>
  <caption id="Table91">Table 91 - Entries in an inline image object</caption>
  <tr>
    <th><b>Full Name</b></th>
    <th><b>Abbreviation</b></th>
  </tr>
  <tr>
    <td><b>Interpolate</b></td>
    <td><b>I</b> (uppercase <del onMouseEnter="mouseEnter(this)" data-issue="306" data-iso="approved">I</del><ins onMouseEnter="mouseEnter(this)" data-issue="306" data-iso="approved">i</ins>)</td>
  </tr>
</table>

<p>...</p>

<p class="location">Replace NOTE 3 as follows:</p>

<p class="hangingindent">NOTE 3
The names <b>DeviceGray</b>, <b>DeviceRGB</b>, and <b>DeviceCMYK</b> (as well as their abbreviations <b>G</b>, <b>RGB</b>, and <b>CMYK</b>)
<del onMouseEnter="mouseEnter(this)" data-issue="19" data-iso="approved">always identify the corresponding colour spaces directly; they never refer to resources in the <b>ColorSpace</b> subdictionary.</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="19" data-iso="approved">never refer to resources in the <b>ColorSpace</b> subdictionary; they always identify
the corresponding colour spaces either directly or via a default colour space (see 8.6.5.6 "Default colour spaces").</ins>
</p>

<p>...</p>

<h2 id="H8.10">8.10 Form XObjects</h2>

<h3 id="H8.10.2">8.10.2 Form dictionaries</h3>

<p class="location">Change Table 93 as follows:</p>

<table>
  <caption id="Table93">Table 93 - Additional entries specific to a Type 1 form dictionary</caption>
  <tr>
    <th><b>Key</b></th>
    <th><b>Type</b></th>
    <th><b>Value</b></th>
  </tr>
  <tr>
    <td><b>Resources</b></td>
    <td>dictionary</td>
    <td>
     <p>
       <i>(<del onMouseEnter="mouseEnter(this)" data-issue="292" data-iso="approved">Optional but strongly recommended</del> <ins onMouseEnter="mouseEnter(this)" data-issue="292" data-iso="approved">Sometimes required</ins>; PDF 1.2)</i> A dictionary specifying any resources (such as fonts and images) required by the form XObject (see 7.8, "Content streams and resources").
     </p>
     <p><del onMouseEnter="mouseEnter(this)" data-issue="292" data-iso="approved">
      In a PDF whose version is 1.1 and earlier, all named resources used in the form XObject shall be included in the resource dictionary of each page object on which the form XObject appears, regardless of whether they also appear in the resource dictionary of the form XObject. These resources should also be specified in the form XObject’s resource dictionary as well, to determine which resources are used inside the form XObject. If a resource is included in both dictionaries, it shall have the same name in both locations.
    </del></p>
    <p>
      In PDF 1.2 and later versions, <del onMouseEnter="mouseEnter(this)" data-issue="292" data-iso="approved">form XObjects may be independent of the content streams in which they appear, and this is strongly recommended although not required</del><ins onMouseEnter="mouseEnter(this)" data-issue="292" data-iso="approved">it is strongly recommended that form XObjects be independent of the content streams in which they appear; from PDF 2.0 this is required</ins>. In an independent form XObject, the resource dictionary of the form XObject is required and shall contain all named resources used by the form XObject. These resources shall not be promoted to the outer content stream’s resource dictionary, although that stream’s resource dictionary refers to the form XObject.
     </p>
     <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="292" data-iso="approved">
      NOTE 1 In PDF 1.1 and earlier, all named resources used in the form XObject were defined to be included in the resource dictionary of each page object on which the form XObject appears, regardless of whether they also appeared in the resource dictionary of the form XObject. These resources also needed to be specified in the form XObject’s resource dictionary as well, to determine which resources were used inside the form XObject. If a resource was included in both dictionaries, it needed to have the same name in both locations.
    </ins></p>
    <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="291" data-iso="approved">
     NOTE 2 Linearized PDF files impose additional requirements on resources - see "Annex F - (normative) Linearized PDF".
    </ins></p>
    </td>
  </tr>
  <tr>
    <td><b>StructParent</b></td>
    <td>integer</td>
    <td>
      (<i>Required if the form XObject is a structural content item; PDF 1.3</i>) The integer key of the form XObject’s entry in the structural parent tree (see 14.7.5.4, "Finding structure elements from content items").
      <ins onMouseEnter="mouseEnter(this)" data-issue="463" data-iso="approved">At most one of the entries <b>StructParent</b> or <b>StructParents</b> shall be present. A form XObject shall be either a content item in its entirety or a container for marked-content sequences that are content items, but not both.</ins>
    </td>
  </tr>
</table>


<h2 id="H8.11">8.11 Optional Content</h2>

<h3 id="H8.11.3">8.11.3 Making graphical content optional</h3>

<h4 id="H8.11.3.2">8.11.3.2 Optional content in content streams</h4>

<p class="location">Change EXAMPLE 1 as follows (whitespace changes are not marked up):</p>

<pre><code><ins onMouseEnter="mouseEnter(this)" data-issue="707">9 0 obj
&lt;&lt; /Length ... &gt;&gt;
stream</ins>          % Within a content stream 
...
/OC /oc1 BDC    % Optional content follows 
  BT 
    /F1 1 Tf 
    12 0 0 12 100 600 Tm 
    (Hello) Tj 
  ET 
EMC             % End of optional content 
... 
<ins onMouseEnter="mouseEnter(this)" data-issue="707">endstream
endobj

10 0 obj</ins>
&lt;&lt;                             % In the resources dictionary 
  /Properties &lt;&lt; /oc1 5 0 R &gt;&gt; % This dictionary maps the name oc1 to an 
...                            % optional content group (object 5) 
&gt;&gt; 
<ins onMouseEnter="mouseEnter(this)" data-issue="707">endobj</ins>
 
5 0 obj                        % The OCG controlling the visibility of the text.
&lt;&lt; /Type /OCG 
   /Name (Show Greeting) 
&gt;&gt; 
endobj
</code></pre>

<p>...</p>

<p class="location">Change EXAMPLE 2 as follows (whitespace changes are not marked up):</p>

<pre><code><ins onMouseEnter="mouseEnter(this)" data-issue="686">5 0 obj
&lt;&lt; /Length ... &gt;&gt;
stream</ins>
% Within a content stream
…
/OC /OC2 BDC                 % Draws a black rectangle frame
    0 g
    4 w
    100 100 412 592 re s
EMC
/OC /OC3 BDC                 % Draws an image XObject
    q
      412 0 0 592 100 100 cm
      /Im3 Do
    Q
EMC
/OC /OC4 BDC                 % Draws an image XObject
    q
      412 0 0 592 100 100 cm
      /Im4 Do
    Q
EMC
… 
<ins onMouseEnter="mouseEnter(this)" data-issue="686">endstream
endobj

10 0 obj</ins>
&lt;&lt;    % The resource dictionary
  /Properties &lt;&lt; /OC2 20 0 R /OC3 30 0 R /OC4 40 0 R &gt;&gt;
  /XObject    &lt;&lt; /Im3 50 0 R /Im4 /60 0 R &gt;&gt;
&gt;&gt;
endobj

20 0 obj    % Optional content membership dictionary
&lt;&lt;
  /Type /OCMD
  /OCGs [ 30 0 R 40 0 R ]
  /P    /AnyOn
&gt;&gt;
endobj
 
30 0 obj    % Optional content group "Image A"
&lt;&lt;
  /Type /OCG
  /Name (Image A)
&gt;&gt;
endobj
 
40 0 obj    % Optional content group "Image B"
&lt;&lt;
  /Type /OCG
  /Name (Image B)
&gt;&gt;
endobj
</code></pre>

<h3 id="H8.11.4">8.11.4 Configuring optional content</h3>

<h4 id="H8.11.4.3">8.11.4.3 Optional content configuration dictionaries</h4>
 
<p class="location">Change Table 99 as follows:</p>

<table>
  <caption id="Table99">Table 99 - Entries in an optional content configuration dictionary</caption>
  <tr>
    <th><b>Key</b></th>
    <th><b>Type</b></th>
    <th><b>Value</b></th>
  </tr>
  <tr>
    <td><b>RBGroups</b></td>
    <td>array</td>
    <td>
     <p>
      (<i>Optional</i>) An array consisting of one or more arrays<del onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="approved">, each of which</del><ins onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="approved">. Each of the inner arrays</ins> represents a collection of optional content groups whose states shall be intended to follow a radio button paradigm. That is, the state of at most one optional content group in each <ins onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="approved">inner</ins> array shall be <b>ON</b> at a time. If one group is turned <b>ON</b>, all others shall be turned <b>OFF</b>. However, turning a group from <b>ON</b> to <b>OFF</b> does not force any other group to be turned <b>ON</b>. <ins onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="approved">None of the inner array elements shall be an empty array.</ins> 
      </p>
      <p>
      <del onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="approved">An empty array [] explicitly indicates that no such collections exist.</del>
      <ins onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="approved">If the value of <b>RBGroups</b> is an empty array [], then this explicitly indicates that no such collections exist.</ins>
      </p>
      <p>
      In the default configuration dictionary, the default value <ins onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="approved">for <b>RBGroups</b></ins> shall be an empty array; in other configuration dictionaries, the default is the <b>RBGroups</b> value from the default configuration dictionary.     
      </p>
    </td>
  </tr>
</table>

<h4 id="H8.11.4.4">8.11.4.4 Usage and usage application dictionaries</h4>
 
<p class="location">Change Table 100 as follows:</p>

<table>
  <caption id="Table100">Table 100 - Entries in an optional content usage dictionary</caption>
  <tr>
    <th><b>Key</b></th>
    <th><b>Type</b></th>
    <th><b>Value</b></th>
  </tr>
  <tr>
    <td><b>Language</b></td>
    <td>dictionary</td>
    <td>
      <p>(<i>Optional</i>) A dictionary specifying the language of the content controlled by this optional content group. It shall contain the following entry:</p>
      <ul>
        <li class="hangingindent"><b>Lang</b> (<i>required</i>) A text string that specifies a language and possibly a locale (see 14.9.2, "Natural language specification"). For example, <code>es-MX</code> represents Mexican Spanish.</li>
      </ul>
      <p>Additionally, it may contain the following entry:</p>
      <ul>
        <li class="hangingindent"><b>Preferred</b> (<i>optional</i>) A name whose values shall be either <i>ON</i> or <i>OFF</i>. Default value: <i>OFF</i>. It shall be used by PDF processors when there is a partial match but no exact match between the system language and the language strings in all usage dictionaries. <del onMouseEnter="mouseEnter(this)" data-issue="567">See 8.11.4.4, "Usage and usage application dictionaries" for more information</del>.</li>
      </ul>
      <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="567">NOTE: This entry does not change the natural language of any content.</ins></p>
    </td>
  </tr>
</table>

<p>...</p>

</div>
