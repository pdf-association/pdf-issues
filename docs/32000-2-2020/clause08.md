---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 8
title: Graphics
modified: 15 September 2023
---

<ul class="noprint">
 <li><a href="#H8.2">8.2 Graphics objects</a>
 </li>
 <li>8.4 Graphics state
  <ul>
   <li><a href="#H8.4.1">8.4.1 General</a>
   </li>
   <li>8.4.3 Details of graphics state parameters
    <ul>
     <li><a href="#H8.4.3.5">Miter limit</a>
     </li>
    </ul>
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
     <li><a href="#H8.6.6.5">8.6.6.5 DeviceN colour spaces</a>
     </li>
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
     <li><a href="#H8.9.6.2">8.9.6.2 Stencil masking</a>
     </li>
   </li>
   <li><a href="#H8.9.7">8.9.7 Inline images</a>
   </li>
  </ul>
 </li>
 <li>8.11 Optional Content
  <ul>
   <li>8.11.4 Configuring optional content
    <ul>
     <li><a href="#H8.11.4.3">8.11.4.3 Optional content configuration dictionaries</a>
     </li>
    </ul>
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
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="260">halftone origin</ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="260">array</ins></td>
    <td>
    <ins onMouseEnter="mouseEnter(this)" data-issue="260">
    (<i>PDF 2.0</i>) The X and Y coordinates of the halftone origin. Initial value: a PDF reader shall initialise this to a suitable device dependent value.
    </ins>
    </td>
  </tr>
</table>

<h3 id="H8.4.3">8.4.3 Details of graphics state parameters</h3>

<h4 id="H8.4.3.5">8.4.3.5 Mitre limit</h4>

<p class="location">Change the first paragraph as follows:</p>

<p>
When two line segments meet at a sharp angle and mitered joins have been specified as the
line join style, it is possible for the miter to extend far beyond the thickness of the
line stroking the path. The miter limit
<ins onMouseEnter="mouseEnter(this)" data-issue="154" data-iso="submitted">shall be a number greater than or equal to 1.0 and</ins>
shall impose a maximum on the ratio of the miter length to the line width (see
"Figure 15 — Miter length"). When the limit is exceeded, the join is converted from
a miter to a bevel.
</p>

<p>...</p>

<h2 id="H8.5">8.5 Path constructing and painting</h2>

<h3 id="H8.5.3">8.5.3 Path-painting operators</h3>

<h4 id="H8.5.3.1">8.5.3.1 General</h4>

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
<b>ICCBased</b> colour spaces (<i>PDF 1.3</i>) shall be based on a cross-platform colour profile as defined by the International Color Consortium (ICC). Unlike the <b>CalGray</b>, <b>CalRGB</b>, and <b>Lab</b> colour spaces, which are characterised by entries in the colour space dictionary, an <b>ICCBased</b> colour space shall be characterised by a sequence of bytes in a standard format. Details of the profile format can be found in the ICC specification<ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">s</ins>.
</p>

<p class="location">Replace the paragraph before Table 66 and Table 66 as follows:</p>

<p>
"Table 66 - <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">ICC Specification versions supported by ICC based colour spaces" shows the versions of the ICC specification on which the
<b>ICCBased</b> colour spaces that PDF versions 1.3 and later shall use. (Earlier versions of the ICC specification shall also be supported.)</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">ICC profile versions supported by <b>ICCBased</b> colour spaces" lists the ICC profile versions as specified in the ICC header that shall be supported.</ins>
</p>

<table>
  <caption id="Table66">Table 66 - <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">ICC Specification versions supported by ICC based colour spaces</del><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">ICC profile versions supported by <b>ICCBased</b> colour spaces</ins></caption>
  <tr>
    <th><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">ICC profile header version</ins></th>
    <th><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">ICC Specification</ins></th>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">2.<i>x.y.z</i></ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">"<i>Specification ICC.1:2001-04 - File Format for Color Profiles [REVISION of ICC.1:1998-09]</i>"</ins></td>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">4.<i>x.y.z</i></ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">ISO 15076-1, <i>Image technology colour management – Architecture, profile format and data structure — Part 1: Based on ICC.1:2010</i></ins></td>
  </tr>
</table>

<p class="location">Change the bulleted list below Table 66 as follows:</p>

<p>PDF processors shall follow these guidelines for writing and rendering ICC based color spaces:</p>

<ul>
<li>A PDF reader shall support <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">ICC.1:2010 as required by PDF 2.0</del><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">both ICC profile header version 2.x and 4.x profiles</ins>, which will enable it to properly render all embedded ICC profiles regardless of the PDF version.</li>
<li>A PDF reader shall always process an embedded ICC profile according to the <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">corresponding version of the PDF</del><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">ICC specification</ins> being processed as shown in <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">"ICC Specification versions supported by ICC based colour spaces</del><ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">"Table 66 - ICC profile versions supported by <b>ICCBased</b> colour spaces"</ins> above; it shall not substitute the alternate colour space in these cases.</li>
<li>A PDF writer should use ICC <del onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted">1:2010</del> profiles<ins onMouseEnter="mouseEnter(this)" data-issue="181" data-iso="submitted"> conforming to ISO 15076</ins>. It may embed profiles conforming to an earlier or later ICC version.</li>
<li>...</li>
</ul>

<p class="location">Add a new NOTE 2 below NOTE 1 and above Table 67 as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="228" data-iso="submitted">NOTE 2 ICC profiles can contain private tags. This document intentionally does not specify how a PDF processor might use such data in ICC profiles. A PDF processor can ignore such data altogether. Any use of such data is implementation dependent.</ins>
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
<ins onMouseEnter="mouseEnter(this)" data-issue="309">The special name <b>None</b> shall not be used in <b>DeviceN</b> colour spaces that have the <b>NChannel</b> subtype</ins>
The special name <b>All</b>, used by <b>Separation</b> colour spaces, shall not be used. The names <b>Cyan</b>, <b>Magenta</b>, <b>Yellow</b> and <b>Black</b> are reserved to name the subtractive process colourants of a CMYK device.
</p>

<p>...</p>

<p class="location">Change the paragraph below NOTE 6 as follows:</p>

<p>
The colour component name <b>None</b>
<del onMouseEnter="mouseEnter(this)" data-issue="309">, which may be present only for <b>DeviceN</b> colour spaces that do not have the <b>NChannel</b> subtype,</del> 
indicates that the corresponding colour component shall never be painted on the page, as in a <b>Separation</b> colour space for the <b>None</b> colourant. When a <b>DeviceN</b> colour space is painting the named device colourants directly, colour components corresponding to <b>None</b> colourants shall be discarded. However, when the <b>DeviceN</b> colour space reverts to its alternate colour space, those components shall be passed to the tint transformation function, which may use them as desired.
</p>


<h2 id="H8.9">Images</h2>

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
    <td>(<i>Optional</i>) A flag indicating whether the image shall be treated as an image mask (see 8.9.6, "Masked images"). If this flag is <i>true</i>,
    the value of <b>BitsPerComponent</b>, if present, shall be 1 and <del onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved">Mask</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved"><b>Mask</b></ins> and <b>ColorSpace</b> shall not be specified; unmasked areas shall be
    painted using the current nonstroking colour. Default value: <i>false</i>.
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
    <td><p>...</p>
    <p>
    <ins onMouseEnter="mouseEnter(this)" data-issue="13" data-iso="approved">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2 Soft-mask images.</ins>
    </p></td>
  </tr>
  <tr>
    <td><b>Name</b></td>
    <td>name</td>
    <td><p>...</p>
    <p>
    <ins onMouseEnter="mouseEnter(this)" data-issue="13" data-iso="approved">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2 Soft-mask images.</ins>
    </p></td>
  </tr>
  <tr>
    <td><b>StructParent</b></td>
    <td>integer</td>
    <td><p>...</p><p><ins onMouseEnter="mouseEnter(this)" data-issue="13" data-iso="approved">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.</ins></p></td>
  </tr>
  <tr>
    <td><b>ID</b></td>
    <td>byte string</td>
    <td><p>...</p><p><ins onMouseEnter="mouseEnter(this)" data-issue="13" data-iso="approved">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.</ins></p></td>
  </tr>
</table>

<h4 id="H8.9.5.4">8.9.5.4 Alternate images</h4>

<p class="location">Change the list below Table 89 as follows:</p>

<p>In PDF 1.5, optional content (see 8.11, "Optional content") may be used to facilitate selection between alternate images. The following algorithm shall be used to determine which image, if any, shall be rendered:</p>

<p class="hangingindent">NOTE (2020) The following algorithm was changed in this document to <del onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">reflect that <b>OC</b> processing has precedence over <b>DefaultForPrinting</b> functionality, and situations where no image is to be rendered</del><ins onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">clarify the relationship between optional content and <b>DefaultForPrinting</b></ins>.</p>

<ol type="a">
 <li value ="1">If the base image contains an <b>OC</b> <del onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">key then <b>DefaultForPrinting</b> shall be ignored on all <b>Alternates</b> entries</del><ins onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">entry that specifies that the content is not visible, then nothing shall be shown</ins>.
 <p></p></li>

 <li value ="2">If the base image contains an <b>OC</b> entry that specifies that the base image is visible, then the base image shall be rendered.
 <p></p></li>

 <li value ="3" style="background-color: seashell; color: darkred; text-decoration: line-through; text-decoration-color: red;">
 <del onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">If the base image contains an <b>OC</b> entry that specifies that the base image is not visible, then the list of alternate image dictionaries specified by the base image <b>Alternates</b> entry shall be examined in order, and the first entry not containing an <b>OC</b> key, or containing an <b>OC</b> entry specifying that the alternate image should be visible, shall be selected. Further, if this selected alternate image has an <b>OC</b> entry, then that <b>OC</b> entry shall also be processed to determine if the alternate image shall be rendered or not. If none of the alternate image dictionaries have an <b>OC</b> key, or none of the alternate image dictionaries with an <b>OC</b> entry specify that that alternate image is visible, then nothing shall be shown. <b>DefaultForPrinting</b> shall be ignored on all <b>Alternates</b> entries.</del>
 <p></p></li>

 <li value="3" style="background-color: lightyellow; color: green; text-decoration-style: double; text-decoration-color: green;">
 <ins onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">Otherwise if the PDF is being printed and any of the <b>Alternates</b> entries has <b>DefaultForPrinting</b> set to true, then that alternate image shall be printed.</ins>
 <p></p></li>

 <li value ="4" style="background-color: seashell; color: darkred; text-decoration: line-through; text-decoration-color: red;">
 <del onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">If the base image does not contain an <b>OC</b> key and the PDF is being printed then the first entry in the <b>Alternates</b> array of the base image that has <b>DefaultForPrinting</b> set to true shall be selected. Further, if this selected alternate image has an <b>OC</b> entry, then that <b>OC</b> entry shall also be processed to determine if the alternate image shall be printed or not. If no alternate image dictionary in the Alternates array has <b>DefaultForPrinting</b> set to true, then the base image shall be printed.</del>
 <p></p></li>

 <li value="4" style="background-color: lightyellow; color: green; text-decoration-style: double; text-decoration-color: green;">
 <ins onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">Otherwise, the list of alternates specified by the base image <b>Alternates</b> entry is examined, and the first alternate containing an <b>OC</b> entry specifying that its content is visible shall be shown (<b>Alternates</b> that have no <b>OC</b> entry shall not be shown.) Furthermore if the image dictionary that forms the value of the <b>Image</b> key of the selected alternate contains an <b>OC</b> entry, then that <b>OC</b> in the image dictionary shall not be examined.</ins>
 <p></p></li>

 <li value="5" style="background-color: lightyellow; color: green; text-decoration-style: double; text-decoration-color: green;">
 <ins onMouseEnter="mouseEnter(this)" data-issue="79" data-iso="approved">If steps c and d above do not identify an alternate to be rendered then the base image shall be rendered.</ins>
 <p></p></li>
</ol>

<p>...</p>


<h3 id="H8.9.6">8.9.6 Masked images</h3>

<h4 id="H8.9.6.2">8.9.6.2 Stencil masking</h4>

<p>...</p>

<p class="location">Change the NOTE as follows:</p>

<p class="hangingindent">
NOTE One of the most important uses of stencil masking is for painting character glyphs represented as bitmaps. Using such a glyph as a stencil mask transfers only its "black" bits to the page, leaving the "white" bits (which are really just background) unchanged. For reasons discussed in 
<del onMouseEnter="mouseEnter(this)" data-issue="333">9.6.5.3, "Encodings for Type 3 fonts"</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="333">9.6.4, "Type 3 fonts"</ins>
, an image mask, rather than an image, 
<del onMouseEnter="mouseEnter(this)" data-issue="333">need almost always be used to paint glyph bitmaps</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="333">is normally used to paint glyph bitmaps</ins>.
<p>


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

<p class="location">Replace NOTE 3 as follows:</p>

<p class="hangingindent">NOTE 3
The names <b>DeviceGray</b>, <b>DeviceRGB</b>, and <b>DeviceCMYK</b> (as well as their abbreviations <b>G</b>, <b>RGB</b>, and <b>CMYK</b>)
<del onMouseEnter="mouseEnter(this)" data-issue="19" data-iso="approved">always identify the corresponding colour spaces directly; they never refer to resources in the <b>ColorSpace</b> subdictionary.</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="19" data-iso="approved">never refer to resources in the <b>ColorSpace</b> subdictionary; they always identify
the corresponding colour spaces either directly or via a default colour space (see 8.6.5.6 "Default colour spaces").</ins>
</p>

<p>...</p>

<h2>8.11 Optional Content</h2>

<h3>8.11.4 Configuring optional content</h3>

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
      (<i>Optional</i>) An array consisting of one or more arrays<del onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="submitted">, each of which</del><ins onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="submitted">. Each of the inner arrays</ins> represents a collection of optional content groups whose states shall be intended to follow a radio button paradigm. That is, the state of at most one optional content group in each <ins onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="submitted">inner</ins> array shall be <b>ON</b> at a time. If one group is turned <b>ON</b>, all others shall be turned <b>OFF</b>. However, turning a group from <b>ON</b> to <b>OFF</b> does not force any other group to be turned <b>ON</b>. <ins onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="submitted">None of the inner array elements shall be an empty array.</ins> 
      </p>
      <p>
      <del onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="submitted">An empty array [] explicitly indicates that no such collections exist.</del>
      <ins onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="submitted">If the value of <b>RBGroups</b> is an empty array [], then this explicitly indicates that no such collections exist.</ins>
      </p>
      <p>
      In the default configuration dictionary, the default value <ins onMouseEnter="mouseEnter(this)" data-issue="225" data-iso="submitted">for <b>RBGroups</b></ins> shall be an empty array; in other configuration dictionaries, the default is the <b>RBGroups</b> value from the default configuration dictionary.     
      </p>
    </td>
  </tr>
</table>

</div>

<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
