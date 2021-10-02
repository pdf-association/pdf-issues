---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 12
title: Interactive features
modified: 30 July 2021
---

<ul>
 <li><a href="#H12.2">12.2 Viewer preferences</a>
 </li>
 <li>12.4 Page-level navigation
  <ul>
   <li><a href="#H12.4.2">12.4.2 Page labels <ins onMouseEnter="mouseEnter(this)" data-issue="73"> and indices</ins></a>
   </li>
   <li>12.4.4 Presentations
    <ul>
     <li><a href="#H12.4.4.1">12.4.4.1 General</a>
     </li>
    </ul>
   </li>
  </ul>
 </li>
 <li>12.5 Annotations
  <ul>
   <li><a href="#H12.5.1">12.5.1 General</a>
   </li>
   <li><a href="#H12.5.2">12.5.2 Annotation dictionaries</a>
   </li>
   <li>12.5.6 Annotation types
    <ul>
     <li><a href="#H12.5.6.2">12.5.6.2 Markup annotations</a>
     </li>
     <li><a href="#H12.5.6.5">12.5.6.5 Link annotations</a>
     </li>
     <li><a href="#H12.5.6.6">12.5.6.6 Free text annotations</a>
     </li>
     <li><a href="#H12.5.6.18">12.5.6.18 Screen annotations</a>
     </li>
     <li><a href="#H12.5.6.24">12.5.6.24 Projection annotations</a>
     </li>
    </ul>
   </li>
  </ul>
 </li>
 <li>12.7 Forms
  <ul>
   <li>12.7.4 Field dictionaries
    <ul>
     <li><a href="#H12.7.4.1">12.7.4.1 General</a>
     </li>
    </ul>
   </li>
   <li>12.7.5 Field types
    <ul>
     <li><a href="#H12.7.5.5">12.7.5.5 Signature Fields</a>
     </li>
    </ul>
   </li>
   <li>12.7.6 Form actions
    <ul>
     <li><a href="#H12.7.6.2">12.7.6.2 Submit-form action</a>
     </li>
    </ul>
   </li>
   <li><a href="#H12.7.9">12.7.9 Non-interactive forms</a>
   </li>
  </ul>
 </li>
 <li>12.8 Digital signatures
  <ul>
   <li><a href="#H12.8.1">12.8.1 Signature Fields</a>
    <ul>
     <li><a href="#H12.8.2.4">12.8.2.4 FieldMDP</a>
     </li>
    </ul>
   </li>
   <li>12.8.3 Signature interoperability
    <ul>
     <li><a href="#H12.8.3.1">12.8.3.1 General</a>
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

<h2 id="H12.2">12.2 Viewer preferences</h2>


<table>
  <caption id="Table147">Table 147 - Entries in a viewer preferences dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>ViewArea</b></td>
    <td>name</td>
    <td>
    (<i>Optional; PDF 1.4; deprecated in PDF 2.0</i>) The name of the page boundary representing the area of a page that shall be
    displayed when viewing the document on the screen. The value is the key designating the relevant page boundary in the page object
    (see <del onMouseEnter="mouseEnter(this)" data-issue="14">7.7.3, "Page tree"</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14">"Table 31 - entries in a page object</ins> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <del onMouseEnter="mouseEnter(this)" data-issue="14"><b>CropBox</b></del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14"><i>CropBox</i></ins>
    <br/>...
    </td>
  </tr>
  <tr>
    <td><b>ViewClip</b></td>
    <td>name</td>
    <td>
    (<i>Optional; PDF 1.4; deprecated in PDF 2.0</i>) The name of the page boundary representing the area of a page that shall be
    displayed to which the contents of a page shall be clipped when viewing the document on the screen. The value is the key designating
    the relevant page boundary in the page object
    (see <del onMouseEnter="mouseEnter(this)" data-issue="14">7.7.3, "Page tree"</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14">"Table 31 - entries in a page object</ins> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <del onMouseEnter="mouseEnter(this)" data-issue="14"><b>CropBox</b></del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14"><i>CropBox</i></ins>
    <br/>...
    </td>
  </tr>
  <tr>
    <td><b>PrintArea</b></td>
    <td>name</td>
    <td>
    (<i>Optional; PDF 1.4; deprecated in PDF 2.0</i>) The name of the page boundary representing the area of a page that shall be
    rendered when printing the document. The value is the key designating the relevant page boundary in the page object
    (see <del onMouseEnter="mouseEnter(this)" data-issue="14">7.7.3, "Page tree"</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14">"Table 31 - entries in a page object</ins> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <del onMouseEnter="mouseEnter(this)" data-issue="14"><b>CropBox</b></del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14"><i>CropBox</i></ins>
    <br/>...
    </td>
  </tr>
  <tr>
    <td><b>PrintClip</b></td>
    <td>name</td>
    <td>
    (<i>Optional; PDF 1.4; deprecated in PDF 2.0</i>) The name of the page boundary to which the contents of the page shall be clipped
    when printing the document. The value is the key designating the relevant page boundary in the page object
    (see <del onMouseEnter="mouseEnter(this)" data-issue="14">7.7.3, "Page tree"</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14">"Table 31 - entries in a page object</ins> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <del onMouseEnter="mouseEnter(this)" data-issue="14"><b>CropBox</b></del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14"><i>CropBox</i></ins>
    <br/>...
    </td>
  </tr>
</table>


<h3 id="H12.4.2">12.4.2 Page labels <ins onMouseEnter="mouseEnter(this)" data-issue="73"> and indices</ins></h3>


<p>...</p>


<h3 id="H12.4.4">12.4.4 Presentations</h3>


<h4 id="H12.4.4.1">12.4.4.1 General</h4>


<table>
  <caption id="Table164">Table 164 - Entries in a transition dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Di</b></td>
    <td><del onMouseEnter="mouseEnter(this)" data-issue="36">number</del><ins onMouseEnter="mouseEnter(this)" data-issue="36">integer</ins> or name</td>
    <td>
      <p>...</p>
      <p>If the value is a <del onMouseEnter="mouseEnter(this)" data-issue="36">number</del><ins onMouseEnter="mouseEnter(this)" data-issue="36">integer</ins>, it shall be one of:</p>
      <p>...</p>
    </td>
  </tr>
</table>


<h2 id="H12.5">12.5 Annotations</h2>

<h3 id="H12.5.1">12.5.1 General</h3>

<p>...</p>

<p>
These descriptions assume the page is being viewed in the orientation specified by the <b>Rotate</b> entry. Conceptually, the behaviour of each annotation type may be
implemented by a software module called an annotation handler. A PDF processor shall provide annotation handlers for all of the conforming annotation types.
The set of annotation types is extensible. An interactive PDF processor shall provide certain expected behaviour for all annotation types that it does not
recognise, as documented in <del onMouseEnter="mouseEnter(this)" data-issue="1">12.5.2, "Annotation dictionaries"</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="1">12.5.5, "Appearance streams" and "Table 167 - Annotation flags" (bit positions 1 and 2)</ins>
.</p>

<h3 id="H12.5.2">12.5.2 Annotation dictionaries</h3>


<table>
  <caption id="Table166">Table 166 - Entries common to all annotation dictionaries</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>AP</b></td>
    <td>dictionary</td>
    <td>
    (<i><del onMouseEnter="mouseEnter(this)" data-issue="22">Optional; PDF 1.2</del>
     <ins onMouseEnter="mouseEnter(this)" data-issue="22">Required except for conditions listed below (PDF 2.0); optional in PDF 1.2 through PDF 1.7</ins></i>)
     An appearance dictionary specifying how the annotation shall be presented visually on the page ...
    </td>
  </tr>
</table>

<p>
<del onMouseEnter="mouseEnter(this)" data-issue="34">A PDF reader shall render the appearance dictionary without regard to any other keys and values in the annotation dictionary and </del>
<ins onMouseEnter="mouseEnter(this)" data-issue="34">When rendering the appearance dictionary, a PDF reader</ins>

shall ignore the values of the <b>C</b>, <b>IC</b>, <b>Border</b>, <b>BS</b>, <b>BE</b>,
<del onMouseEnter="mouseEnter(this)" data-issue="34"><b>BM</b>,</del>
<b>CA</b>, <b>ca</b>, <b>H</b>, <b>DA</b>, <b>Q</b>, <b>DS</b>, <b>LE</b>, <b>LL</b>, <b>LLE</b>,
<ins onMouseEnter="mouseEnter(this)" data-issue="56"><b>MK</b>,</ins>
and <b>Sy</b> keys.
</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="34">NOTE 1 Some of these keys are only relevant to certain annotation subtypes as described in the following subclauses.</ins>
</p>


<p class="hangingindent">
NOTE <ins onMouseEnter="mouseEnter(this)" data-issue="34">2</ins> Requiring an appearance dictionary for each annotation ensures the reliable rendering of the annotations.
<ins onMouseEnter="mouseEnter(this)" data-issue="34">When an appearance dictionary is not present, the rendered appearance will be implementation dependent.</ins>
</p>

<h4 id="H12.5.6.2">12.5.6.2 Markup annotations</h4>

<p>...</p>

<p>
When
<ins onMouseEnter="mouseEnter(this)" data-issue="90">providing the <b>Contents</b> key, if</ins>
separating text into paragraphs, a CARRIAGE RETURN (0Dh) shall be used and not, for example, a LINE FEED character (0Ah).
</p>

<p>...</p>


<h4 id="H12.5.6.5">12.5.6.5 Link annotations</h4>


<table>
  <caption id="Table176">Table 176 - Additional entries specific to a link annotation</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>QuadPoints</b></td>
    <td>array</td>
    <td>
    <p>(<i>Optional; PDF 1.6</i>) An array of 8 &times; <i>n</i> numbers specifying the coordinates of n quadrilaterals in default user space that comprise
    the region in which the link should be activated. The coordinates for each quadrilateral are given in the order:<br/>
    <i>x</i><sub>1</sub> <i>y</i><sub>1</sub> <i>x</i><sub>2</sub> <i>y</i><sub>2</sub> <i>x</i><sub>3</sub> <i>y</i><sub>3</sub> <i>x</i><sub>4</sub> <i>y</i><sub>4</sub><br/>
    specifying the four vertices of the quadrilateral in counterclockwise order. For orientation purposes, such as when applying an underline border style, the bottom of a
    quadrilateral is the line formed by (<i>x</i><sub>1</sub>, <i>y</i><sub>1</sub>) and (<i>x</i><sub>2</sub>, <i>y</i><sub>2</sub>).<br/>
    If this entry is not present, or the PDF processor does not recognise it, or if any coordinates in the <b>QuadPoints</b> array lie outside the region specified by
    <b>Rect</b> then the activation region for the link annotation shall be defined by its <b>Rect</b> entry.
    </p>
    <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="17">NOTE 1 When <b>QuadPoints</b> is used, the activation area and the visual appearance (including border) of the link annotation are not required to be the same.</ins></p>
    <p class="hangingindent">NOTE <ins onMouseEnter="mouseEnter(this)" data-issue="17">2</ins> The last paragraph above was clarified in this document (2020).</p>
    </td>
  </tr>
</table>


<h4 id="H12.5.6.6">12.5.6.6 Free text annotations</h4>

<table>
  <caption id="Table177">Table 177 - Additional entries specific to a free text annotation</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>DA</b></td>
    <td>string</td>
    <td>
    <p>(<i>Required</i>) The default appearance string that shall be used in formatting the text (see 12.7.4.3, "Variable text").</p>
    <p>The annotation dictionary's <b>AP</b> entry <del onMouseEnter="mouseEnter(this)" data-issue="42">, if present,</del> shall take precedence over the <b>DA</b> entry (see "Table 170 - Entries in an appearance dictionary" and 12.5.5, "Appearance streams").</p>
    </td>
  </tr>
</table>


<h4 id="H12.5.6.18">12.5.6.18 Screen annotations</h4>

<p>...</p>

<ul>
<li>...</li>
<li>
The <b>AP</b> entry refers to an appearance dictionary (see "Table 170 - Entries in an appearance dictionary") whose normal appearance provides the visual
appearance for a screen annotation that shall be used for printing and default display when a media clip is not being played.
<del onMouseEnter="mouseEnter(this)" data-issue="42">If <b>AP</b> is not present, the screen annotation shall not have a default visual appearance and shall not be printed.</del>
</li>
</ul>


<h4 id="H12.5.6.24">12.5.6.24 Projection annotations</h4>

<p>A <i>projection annotation (PDF 2.0)</i> is a markup annotation subtype (see 12.5.6.2, "Markup annotations") that has much of the functionality of other markup annotations.
However, a projection annotation is only valid within the context of an associated run-time environment, such as an activated 3D model<ins onMouseEnter="mouseEnter(this)" data-issue="94">, and thus an <b>AP</b> dictionary is not required</ins>.</p>

<p>...</p>


<p><del onMouseEnter="mouseEnter(this)" data-issue="42">A projection annotation with a <b>Rect</b> entry that has zero height or zero width shall not have an <b>AP</b> dictionary.</del></p>

<h3 id="H12.7.4">12.7.4 Field dictionaries</h3>


<h4 id="H12.7.4.1">12.7.4.1 General</h4>


<table>
  <caption id="Table226">Table 226 - Entries common to all field dictionaries</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>T</b></td>
    <td>text string</td>
    <td>
    (<i><del onMouseEnter="mouseEnter(this)" data-issue="28">Required</del>
        <ins onMouseEnter="mouseEnter(this)" data-issue="28">Optional</ins></i>)
    The partial field name (see 12.7.4.2, "Field names").
    </td>
  </tr>
</table>


<h4 id="H12.7.5.5">12.7.5.5 Signature Fields</h4>


<table>
  <caption id="Table237">Table 237 - Entries in a signature field seed value dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>AddRevInfo</b></td>
    <td>boolean</td>
    <td><p  class="hangingindent">
    NOTE 3 <del onMouseEnter="mouseEnter(this)" data-issue="4"><i>adbe.pkcs7.detached</i></del> <ins onMouseEnter="mouseEnter(this)" data-issue="4"><i>adbe.x509.rsa_sha1</i></ins>
    and <i>adbe.pkcs7.sha1</i> are deprecated in PDF 2.0.</p></td>
  </tr>
</table>

<h3 id="H12.7.6">12.7.6 Form actions</h3>

<h4 id="H12.7.6.2">12.7.6.2 Submit-form action</h4>

<table>
  <caption id="Table239">Table 239 - Additional entries specific to a submit-form action</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Flags</b></td>
    <td>integer</td>
    <td>
    <p>(<i>Optional<del onMouseEnter="mouseEnter(this)" data-issue="122">; inheritable</del></i>) ... </p>
    </td>
  </tr>
  <tr>
    <td><b>CharSet</b></td>
    <td>string</td>
    <td>
    <p>(<i>Optional<del onMouseEnter="mouseEnter(this)" data-issue="122">; inheritable</del></i>) ... </p>
    </td>
  </tr>
</table>

<h3 id="H12.7.9">12.7.9 Non-interactive forms</h3>


<p>
Unlike interactive forms, non-interactive forms do not use widget annotations but are represented with page content. Non-interactive forms are defined by the
<b>PrintField</b> attrib<del onMouseEnter="mouseEnter(this)" data-issue="54">0</del>ute (14.8.5.6, "PrintField attributes") for repurposing and accessibility purposes.
</p>


<h3 id="H12.8.1">12.8.1 Signature Fields</h3>

<p>...</p>

<p>A PDF document may contain the following standard types of signatures:</p>
<ul>
  <li><p>...</p></li>
  <li>
  Any number of document timestamp signatures, see 12.8.5, "Document timestamp (DTS) dictionary". The timestamp signature dictionary of a document timestamp signature
  shall be the value of a signature field and shall contain a <b>ByteRange</b> entry. <ins onMouseEnter="mouseEnter(this)" data-issue="55">These shall follow the certification signature if one is present.</ins>
  </li>
</ul>

<p>A signature dictionary is used by all of these types of signatures.</p>

<table>
  <caption id="Table255">Table 255 - Entries in a signature dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Filter</b></td>
    <td>name</td>
    <td>
    <p>(<i>Required<del onMouseEnter="mouseEnter(this)" data-issue="121">; inheritable</del></i>) ... </p>
    </td>
  </tr>
  <tr>
    <td><b>Cert</b></td>
    <td>byte string or array</td>
    <td>
    <p>...</p>
    <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="4">NOTE <i>adbe.x509.rsa_sha1</i> and <i>adbe.pkcs7.sha1</i> are deprecated in PDF 2.0.</ins></p>
    </td>
  </tr>
</table>

<p>...</p>

<table>
  <caption id="Table256">Table 256 - Entries in a signature reference dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>DigestMethod</b></td>
    <td>name</td>
    <td>
    <p>(<i><del onMouseEnter="mouseEnter(this)" data-issue="171">Required</del><ins onMouseEnter="mouseEnter(this)" data-issue="171">Optional; deprecated in PDF 2.0</ins></i>) ... </p>
    </td>
  </tr>
</table>

<h4 id="H12.8.2.4">12.8.2.4 FieldMDP</h4>


<table>
  <caption id="Table259">Table 259 - Entries in the FieldMDP transform parameters dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Fields</b></td>
    <td>array</td>
    <td>
    (<i>Required if <b>Action</b> is Include or Exclude</i>) An array of text strings containing <ins onMouseEnter="mouseEnter(this)" data-issue="33">fully qualified</ins>
    field names <ins onMouseEnter="mouseEnter(this)" data-issue="33">(see 12.7.4.2 "Field names")</ins>.
    </td>
  </tr>
</table>


<h3 id="H12.8.3">12.8.3 Signature interoperability</h3>


<h4 id="H12.8.3.1">12.8.3.1 General</h4>


<table>
  <caption id="Table260">Table 260 - SubFilter value algorithm support</caption>
  <tr>
    <th>SubFilter values</th>
    <th>adbe.pkcs7.detached,<br/>ETSI.CAdES.detached or<br/>ETSI.RFC3161</th>
    <th>adbe.pkcs7.sha1 <sup>c</sup> </th>
    <th>adbe.x509.rsa_sha1 <sup>a</sup> <ins onMouseEnter="mouseEnter(this)" data-issue="4"><sup>c</sup></ins></th>
  </tr>
  <tr>
    <td>...</td>
    <td>...</td>
    <td>...</td>
    <td>...</td>
  </tr>
  <tr>
    <td colspan="4">
      <p>...</p>
      <p><sup>c</sup> The values <i>adbe.x509.rsa_sha1</i> and <i>adbe.pkcs7.sha1</i> have been deprecated with PDF 2.0.</p>
      <p>...</p>
    </td>
  </tr>
</table>

<p>
<ins onMouseEnter="mouseEnter(this)" data-issue="109"><sup>Note that in Table 260 italic formatting of PDF versions (such as "(<i>PDF 1.5</i>)") is inconsistently applied and needs to be corrected.</sup></ins>
</p>

</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
