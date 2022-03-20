---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 8
title: Graphics
modified: 20 March 2022
---

<ul class="noprint">
 <li><a href="#H8.2">8.2 Graphics objects</a>
 </li>
 <li>8.4 Graphics state
  <ul>
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
     <li><a href="#H8.6.5.8">8.6.5.8 Rendering intents</a>
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
   <li><a href="#H8.9.7">8.9.7 Inline images</a>
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
    <del onMouseEnter="mouseEnter(this)" data-issue="80"><b>Sh</b></del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="80"><b>sh</b></ins>
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
    <del onMouseEnter="mouseEnter(this)" data-issue="85">"Table 351 — Entries in a data dictionary"</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="85">"Table 352 — Marked-content operators"</ins>
    </td>
  </tr>
</table>

<h2 id="H8.4">8.4 Graphics state</h2>

<h3 id="H8.4.3">8.4.3 Details of graphics state parameters</h3>

<h4 id="H8.4.3.5">8.4.3.5 Mitre limit</h4>

<p class="location">Change the first paragraph as follows:</p>

<p>
When two line segments meet at a sharp angle and mitered joins have been specified as the
line join style, it is possible for the miter to extend far beyond the thickness of the
line stroking the path. The miter limit
<ins onMouseEnter="mouseEnter(this)" data-issue="154">shall be a number greater than or equal to 1.0 and</ins>
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
    <ins onMouseEnter="mouseEnter(this)" data-issue="103">In the opaque imaging model, this</ins>
    <del onMouseEnter="mouseEnter(this)" data-issue="103">This</del> operator shall produce the same result
    as constructing two identical path objects, painting the first with <b>f</b> and the second with <b>S</b>.</p>
    <p>...</p>
    </td>
  </tr>
</table>


<h4 id="H8.6.5.8">8.6.5.8 Rendering intents</h4>

<p class="location">Change the NOTE below Table 69 as follows:</p>

<p class="hangingindent">
NOTE The exact set of rendering intents supported can vary from one output device to another; a particular device
<del onMouseEnter="mouseEnter(this)" data-issue="63">does not have to support all PDF rendering intents and</del>
can support additional ones beyond those listed in the table above.
</p>

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
        <p><ins onMouseEnter="mouseEnter(this)" data-issue="13">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
        Soft-mask images.</ins></p>
    </td>
  </tr>
  <tr>
    <td><b>ImageMask</b></td>
    <td>boolean</td>
    <td>(<i>Optional</i>) A flag indicating whether the image shall be treated as an image mask (see 8.9.6, "Masked images"). If this flag is <i>true</i>,
    the value of <b>BitsPerComponent</b>, if present, shall be 1 and <del onMouseEnter="mouseEnter(this)" data-issue="14">Mask</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14"><b>Mask</b></ins> and <b>ColorSpace</b> shall not be specified; unmasked areas shall be
    painted using the current nonstroking colour. Default value: <i>false</i>.
    </td>
  </tr>
  <tr>
    <td><b>Alternates</b></td>
    <td>array</td>
    <td>
        <p>...</p>
        <p><ins onMouseEnter="mouseEnter(this)" data-issue="13">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.</ins></p></td>
  </tr>
  <tr>
    <td><b>SMask</b></td>
    <td>stream</td>
    <td><p>...</p>
    <p>
    <ins onMouseEnter="mouseEnter(this)" data-issue="13">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2 Soft-mask images.</ins>
    </p></td>
  </tr>
  <tr>
    <td><b>Name</b></td>
    <td>name</td>
    <td><p>...</p>
    <p>
    <ins onMouseEnter="mouseEnter(this)" data-issue="13">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2 Soft-mask images.</ins>
    </p></td>
  </tr>
  <tr>
    <td><b>StructParent</b></td>
    <td>integer</td>
    <td><p>...</p><p><ins onMouseEnter="mouseEnter(this)" data-issue="13">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.</ins></p></td>
  </tr>
  <tr>
    <td><b>ID</b></td>
    <td>byte string</td>
    <td><p>...</p><p><ins onMouseEnter="mouseEnter(this)" data-issue="13">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.</ins></p></td>
  </tr>
</table>

<h4 id="H8.9.5.4">8.9.5.4 Alternate images</h4>

<p class="location">Change the list below Table 89 as follows:</p>

<p>In PDF 1.5, optional content (see 8.11, "Optional content") may be used to facilitate selection between alternate images. The following algorithm shall be used to determine which image, if any, shall be rendered:</p>

<p class="hangingindent">NOTE (2020) The following algorithm was changed in this document to <del onMouseEnter="mouseEnter(this)" data-issue="79">reflect that <b>OC</b> processing has precedence over <b>DefaultForPrinting</b> functionality, and situations where no image is to be rendered</del><ins onMouseEnter="mouseEnter(this)" data-issue="79">clarify the relationship between optional content and <b>DefaultForPrinting</b></ins>.</p>

<ol type="a">
 <li value ="1">If the base image contains an <b>OC</b> <del onMouseEnter="mouseEnter(this)" data-issue="79">key then <b>DefaultForPrinting</b> shall be ignored on all <b>Alternates</b> entries</del><ins onMouseEnter="mouseEnter(this)" data-issue="79">entry that specifies that the content is not visible, then nothing shall be shown</ins>.
 <p></p></li>

 <li value ="2">If the base image contains an <b>OC</b> entry that specifies that the base image is visible, then the base image shall be rendered.
 <p></p></li>

 <li value ="3" style="background-color: seashell; color: darkred; text-decoration: line-through; text-decoration-color: red;">
 <del onMouseEnter="mouseEnter(this)" data-issue="79">If the base image contains an <b>OC</b> entry that specifies that the base image is not visible, then the list of alternate image dictionaries specified by the base image <b>Alternates</b> entry shall be examined in order, and the first entry not containing an <b>OC</b> key, or containing an <b>OC</b> entry specifying that the alternate image should be visible, shall be selected. Further, if this selected alternate image has an <b>OC</b> entry, then that <b>OC</b> entry shall also be processed to determine if the alternate image shall be rendered or not. If none of the alternate image dictionaries have an <b>OC</b> key, or none of the alternate image dictionaries with an <b>OC</b> entry specify that that alternate image is visible, then nothing shall be shown. <b>DefaultForPrinting</b> shall be ignored on all <b>Alternates</b> entries.</del>
 <p></p></li>

 <li value="3" style="background-color: lightyellow; color: green; text-decoration-style: double; text-decoration-color: green;">
 <ins onMouseEnter="mouseEnter(this)" data-issue="79">Otherwise if the PDF is being printed and any of the <b>Alternates</b> entries has <b>DefaultForPrinting</b> set to true, then that alternate image shall be printed.</ins>
 <p></p></li>

 <li value ="4" style="background-color: seashell; color: darkred; text-decoration: line-through; text-decoration-color: red;">
 <del onMouseEnter="mouseEnter(this)" data-issue="79">If the base image does not contain an <b>OC</b> key and the PDF is being printed then the first entry in the <b>Alternates</b> array of the base image that has <b>DefaultForPrinting</b> set to true shall be selected. Further, if this selected alternate image has an <b>OC</b> entry, then that <b>OC</b> entry shall also be processed to determine if the alternate image shall be printed or not. If no alternate image dictionary in the Alternates array has <b>DefaultForPrinting</b> set to true, then the base image shall be printed.</del>
 <p></p></li>

 <li value="4" style="background-color: lightyellow; color: green; text-decoration-style: double; text-decoration-color: green;">
 <ins onMouseEnter="mouseEnter(this)" data-issue="79">Otherwise, the list of alternates specified by the base image <b>Alternates</b> entry is examined, and the first alternate containing an <b>OC</b> entry specifying that its content is visible shall be shown (<b>Alternates</b> that have no <b>OC</b> entry shall not be shown.) Furthermore if the image dictionary that forms the value of the <b>Image</b> key of the selected alternate contains an <b>OC</b> entry, then that <b>OC</b> in the image dictionary shall not be examined.</ins>
 <p></p></li>

 <li value="5" style="background-color: lightyellow; color: green; text-decoration-style: double; text-decoration-color: green;">
 <ins onMouseEnter="mouseEnter(this)" data-issue="79">If steps c and d above do not identify an alternate to be rendered then the base image shall be rendered.</ins>
 <p></p></li>
</ol>

<p>...</p>

<h3 id="H8.9.7">8.9.7 Inline images</h3>

<p class="location">Change the paragraphs below Table 90 as follows:</p>

<p>
Inline image objects shall not be nested; that is, two <b>BI</b> operators shall not appear without an intervening <b>EI</b> to close the first object.
Similarly, an <b>ID</b> operator shall only appear between a <b>BI</b> and its balancing <b>EI</b>. Unless the image uses <b>ASCIIHexDecode</b> or
<b>ASCII85Decode</b> as <del onMouseEnter="mouseEnter(this)" data-issue="20">one of its filters</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="20">its final or only filter</ins>, the <b>ID</b> operator shall be followed by a
single white-space character, and the next character shall be interpreted as the first byte of image data.
</p>

<p>
The key-value pairs appearing between the <b>BI</b> and <b>ID</b> operators (as listed in "Table 91 - Entries in an inline
image object") are analogous to their respective key-value pairs in an image XObject dictionary (see "Table 87 - Additional
entries specific to an image dictionary") or a stream dictionary (see "Table 5 - Entries common to all stream dictionaries").
For convenience, the abbreviations shown in "Table 91 - Entries in an inline image object" and "Table 92 - Additional
abbreviations in an inline image object" may be used in place of the full names.
<ins onMouseEnter="mouseEnter(this)" data-issue="3">In the situation where both an abbreviated key name and the corresponding full key name from Table 91 are present, the abbreviated key name shall take precedence.</ins>
Entries other than those listed shall be ignored.
</p>

<p>...</p>

<p class="location">Replace NOTE 3 as follows:</p>

<p class="hangingindent">NOTE 3
<del onMouseEnter="mouseEnter(this)" data-issue="19">
The names <b>DeviceGray</b>, <b>DeviceRGB</b>, and <b>DeviceCMYK</b> (as well as their abbreviations <b>G</b>, <b>RGB</b>, and <b>CMYK</b>) always
identify the corresponding colour spaces directly; they never refer to resources in the <b>ColorSpace</b> subdictionary.</del>


<ins onMouseEnter="mouseEnter(this)" data-issue="19">The names <b>DeviceGray</b>, <b>DeviceRGB</b>, and <b>DeviceCMYK</b> (as well as their abbreviations <b>G</b>, <b>RGB</b>, and <b>CMYK</b>) never refer to resources in the <b>ColorSpace</b> subdictionary; they always identify the corresponding colour spaces either directly or via a default colour space (see
8.6.5.6 "Default colour spaces").</ins>
</p>

<p>...</p>

</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
