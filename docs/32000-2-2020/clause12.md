---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 12
title: Interactive features
modified: 26 May 2022
---

<ul class="noprint">
 <li><a href="#H12.2">12.2 Viewer preferences</a>
 </li>
 <li>12.3 Document-level navigation
  <ul>
   <li><a href="#H12.3.3">12.3.3 Document outline</a>
   </li>
  </ul>
 </li>
 <li>12.4 Page-level navigation
  <ul>
   <li><a href="#H12.4.2">12.4.2 Page labels <ins onMouseEnter="mouseEnter(this)" data-issue="73" data-iso="approved"> and indices</ins></a>
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
 <li>12.6 Actions
  <ul>
   <li>12.6.4 Action types
    <ul>
     <li><a href="#H12.6.4.2">12.6.4.2 Go-To actions</a>
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
     <li><a href="#H12.7.6.3">12.7.6.3 Reset-form action</a>
     </li>
    </ul>
   </li>
   <li>12.7.8 Form data format
    <ul>
     <li><a href="#H12.7.8.1">12.7.8.1 General</a>
     </li>
    </ul>
   </li>
   <li><a href="#H12.7.9">12.7.9 Non-interactive forms</a>
   </li>
  </ul>
 </li>
 <li>12.8 Digital signatures
  <ul>
   <li><a href="#H12.8.1">12.8.1 General</a>
   </li>
   <li>12.8.2 Transform methods
    <ul>
     <li>12.8.2.2 DocMDP
      <ul>
       <li><a href="#H12.8.2.2.2">12.8.2.2.2 Validating signatures that use the DocMDP transform method</a>
       </li>
      </ul>
     </li>
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

<p class="location">Change Table 147 as follows:</p>

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
    (see <del onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved">7.7.3, "Page tree"</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved">"Table 31 - entries in a page object"</ins> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <del onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved"><b>CropBox</b></del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved"><i>CropBox</i></ins>
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
    (see <del onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved">7.7.3, "Page tree"</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved">"Table 31 - entries in a page object"</ins> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <del onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved"><b>CropBox</b></del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved"><i>CropBox</i></ins>
    <br/>...
    </td>
  </tr>
  <tr>
    <td><b>PrintArea</b></td>
    <td>name</td>
    <td>
    (<i>Optional; PDF 1.4; deprecated in PDF 2.0</i>) The name of the page boundary representing the area of a page that shall be
    rendered when printing the document. The value is the key designating the relevant page boundary in the page object
    (see <del onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved">7.7.3, "Page tree"</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved">"Table 31 - entries in a page object"</ins> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <del onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved"><b>CropBox</b></del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved"><i>CropBox</i></ins>
    <br/>...
    </td>
  </tr>
  <tr>
    <td><b>PrintClip</b></td>
    <td>name</td>
    <td>
    (<i>Optional; PDF 1.4; deprecated in PDF 2.0</i>) The name of the page boundary to which the contents of the page shall be clipped
    when printing the document. The value is the key designating the relevant page boundary in the page object
    (see <del onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved">7.7.3, "Page tree"</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved">"Table 31 - entries in a page object"</ins> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <del onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved"><b>CropBox</b></del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved"><i>CropBox</i></ins>
    <br/>...
    </td>
  </tr>
</table>

<h2 id="H12.3">12.3 Document-level navigation</h2>

<h3 id="H12.3.3">12.3.3 Document outline</h3>

<p class="location">Change Table 151 as follows:</p>

<table>
  <caption id="Table151">Table 151 - Entries in an outline item dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Prev</b></td>
    <td>dictionary</td>
    <td>
    <p>(<i>Required for all but the first item at each level; <ins onMouseEnter="mouseEnter(this)" data-issue="139">shall not be present on the first item at each level;</ins>
        shall be an indirect reference</i>) The previous item at this outline level.</p>
    </td>
  </tr>
  <tr>
    <td><b>Next</b></td>
    <td>dictionary</td>
    <td>
    <p>(<i>Required for all but the last item at each level; <ins onMouseEnter="mouseEnter(this)" data-issue="139">shall not be present on the last item at each level;</ins>
        shall be an indirect reference</i>) The next item at this outline level.</p>
    </td>
  </tr>
</table>

<p>...</p>

<p class="location">Change the title of clause 12.4.2 as follows:</p>

<h3 id="H12.4.2">12.4.2 Page labels <ins onMouseEnter="mouseEnter(this)" data-issue="73" data-iso="approved"> and indices</ins></h3>

<p>...</p>


<h3 id="H12.4.4">12.4.4 Presentations</h3>


<h4 id="H12.4.4.1">12.4.4.1 General</h4>

<p class="location">Change Table 164 as follows:</p>

<table>
  <caption id="Table164">Table 164 - Entries in a transition dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
   <td><b>M</b></td>
   <td>name</td>
   <td>
    <p>(<i>Optional; Split, Box and Fly transition styles only</i>) The direction of motion for the specified transition effect:</p>
    <p><i>I</i> Inward from the edges of the page (<del onMouseEnter="mouseEnter(this)" data-issue="75" data-iso="approved">upper case</del> <ins onMouseEnter="mouseEnter(this)" data-issue="75" data-iso="approved">uppercase</ins> i)</p>
    <p><i>O</i> Outward from the centre of the page (<del onMouseEnter="mouseEnter(this)" data-issue="75" data-iso="approved">upper case</del> <ins onMouseEnter="mouseEnter(this)" data-issue="75" data-iso="approved">uppercase</ins> o)</p>
    <p>Default value: <i>I</i>.</p>
   </td>
  </tr>
  <tr>
    <td><b>Di</b></td>
    <td><del onMouseEnter="mouseEnter(this)" data-issue="36" data-iso="approved">number</del><ins onMouseEnter="mouseEnter(this)" data-issue="36" data-iso="approved">integer</ins> or name</td>
    <td>
      <p>...</p>
      <p>If the value is <del onMouseEnter="mouseEnter(this)" data-issue="36" data-iso="approved">a number</del><ins onMouseEnter="mouseEnter(this)" data-issue="36" data-iso="approved">an integer</ins>, it shall be one of:</p>
      <p>...</p>
    </td>
  </tr>
</table>

<h2 id="H12.5">12.5 Annotations</h2>

<h3 id="H12.5.1">12.5.1 General</h3>

<p class="location">Change the last paragraph as follows:</p>

<p>
These descriptions assume the page is being viewed in the orientation specified by the <b>Rotate</b> entry. Conceptually, the behaviour of each annotation type may be
implemented by a software module called an annotation handler. A PDF processor shall provide annotation handlers for all of the conforming annotation types.
The set of annotation types is extensible. An interactive PDF processor shall provide certain expected behaviour for all annotation types that it does not
recognise, as documented in <del onMouseEnter="mouseEnter(this)" data-issue="1" data-iso="approved">12.5.2, "Annotation dictionaries"</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="1" data-iso="approved">12.5.5, "Appearance streams" and "Table 167 - Annotation flags" (bit positions 1 and 2)</ins>
.</p>

<h3 id="H12.5.2">12.5.2 Annotation dictionaries</h3>

<p class="location">Change Table 166 as follows:</p>

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
    <p>(<i><del onMouseEnter="mouseEnter(this)" data-issue="22" data-iso="approved">Optional; PDF 1.2</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="22" data-iso="approved">Required except for conditions listed below (PDF 2.0); optional in PDF 1.2 through PDF 1.7</ins></i>)
    An appearance dictionary specifying how the annotation shall be presented visually on the page. A PDF writer shall include an appearance dictionary when writing or updating the PDF file except for the two cases listed below.</p>
    <p>Every annotation (including those whose <b>Subtype</b> value is <i>Widget</i>, as used for form fields), except for the two cases listed below, shall have at least one appearance dictionary.</p>
    <ul>
      <li>Annotations where the value of the <b>Rect</b> key consists of an array where the value at index <del onMouseEnter="mouseEnter(this)" data-issue="124" data-iso="approved">1</del><ins onMouseEnter="mouseEnter(this)" data-issue="124" data-iso="approved">0</ins> is equal to the value at index <del onMouseEnter="mouseEnter(this)" data-issue="124" data-iso="approved">3</del><ins onMouseEnter="mouseEnter(this)" data-issue="124" data-iso="approved">2</ins> and the value at index <del onMouseEnter="mouseEnter(this)" data-issue="124" data-iso="approved">2</del><ins onMouseEnter="mouseEnter(this)" data-issue="124" data-iso="approved">1</ins> is equal to the value at index <del onMouseEnter="mouseEnter(this)" data-issue="124" data-iso="approved">4</del><ins onMouseEnter="mouseEnter(this)" data-issue="124" data-iso="approved">3</ins>.</li>
    </ul>
    <p class="hangingindent">NOTE (2020) The bullet point above was changed from "or" to "and" in this document to match requirements in other published ISO PDF standards (such as PDF/A). <ins onMouseEnter="mouseEnter(this)" data-issue="124" data-iso="approved">Array indices were also corrected to be zero-based as described in 3.2 "array object".</ins></p>
    <ul>
      <li>Annotations whose <b>Subtype</b> value is <i>Popup</i>, <i>Projection</i> or <i>Link</i>.</li>
    </ul>
    </td>
  </tr>
</table>

<p class="location">Change the paragraph and NOTEs below Table 166 as follows:</p>

<p>
<del onMouseEnter="mouseEnter(this)" data-issue="23,34" data-iso="approved,approved">A PDF reader shall render the appearance dictionary without regard to any other keys and values in the annotation dictionary and </del>
<ins onMouseEnter="mouseEnter(this)" data-issue="23,34" data-iso="approved,approved">When rendering the appearance dictionary, a PDF reader</ins>
shall ignore the values of the <b>C</b>, <b>IC</b>, <b>Border</b>, <b>BS</b>, <b>BE</b>,
<del onMouseEnter="mouseEnter(this)" data-issue="23,34" data-iso="approved,approved"><b>BM</b>,</del>
<b>CA</b>, <b>ca</b>, <b>H</b>, <b>DA</b>, <b>Q</b>, <b>DS</b>, <b>LE</b>, <b>LL</b>, <b>LLE</b>,
<ins onMouseEnter="mouseEnter(this)" data-issue="56" data-iso="approved"><b>MK</b>,</ins>
and <b>Sy</b> keys.
</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="34" data-iso="approved">NOTE 1 Some of these keys are only relevant to certain annotation subtypes as described in the following subclauses.</ins>
</p>


<p class="hangingindent">
NOTE <ins onMouseEnter="mouseEnter(this)" data-issue="34" data-iso="approved">2</ins> Requiring an appearance dictionary for each annotation ensures the reliable rendering of the annotations.
<ins onMouseEnter="mouseEnter(this)" data-issue="34" data-iso="approved">When an appearance dictionary is not present, the rendered appearance will be implementation dependent.</ins>
</p>

<h4 id="H12.5.6.2">12.5.6.2 Markup annotations</h4>

<p class="location">Change the paragraph below NOTE 1 as follows:</p>

<p>
When
<ins onMouseEnter="mouseEnter(this)" data-issue="90">providing the <b>Contents</b> key, if</ins>
separating text into paragraphs, a CARRIAGE RETURN (0Dh) shall be used and not, for example, a LINE FEED character (0Ah).
</p>

<p>...</p>

<h4 id="H12.5.6.5">12.5.6.5 Link annotations</h4>

<p class="location">Change Table 176 as follows:</p>

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
    <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="17" data-iso="approved">NOTE 1 When <b>QuadPoints</b> is used, the activation area and the visual appearance (including border) of the link annotation are not required to be the same.</ins></p>
    <p class="hangingindent">NOTE <ins onMouseEnter="mouseEnter(this)" data-issue="17" data-iso="approved">2</ins> The last paragraph above was clarified in this document (2020).</p>
    </td>
  </tr>
</table>

<h4 id="H12.5.6.6">12.5.6.6 Free text annotations</h4>

<p class="location">Change Table 177 as follows:</p>

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
    <p>The annotation dictionary's <b>AP</b> entry <del onMouseEnter="mouseEnter(this)" data-issue="42" data-iso="approved">, if present,</del> shall take precedence over the <b>DA</b> entry (see "Table 170 - Entries in an appearance dictionary" and 12.5.5, "Appearance streams").</p>
    </td>
  </tr>
</table>

<h4 id="H12.5.6.18">12.5.6.18 Screen annotations</h4>

<p class="location">Change the last bullet below Table 190 as follows:</p>

<ul>
<li>...</li>
<li>
The <b>AP</b> entry refers to an appearance dictionary (see "Table 170 - Entries in an appearance dictionary") whose normal appearance provides the visual
appearance for a screen annotation that shall be used for printing and default display when a media clip is not being played.
<del onMouseEnter="mouseEnter(this)" data-issue="42" data-iso="approved">If <b>AP</b> is not present, the screen annotation shall not have a default visual appearance and shall not be printed.</del>
</li>
</ul>

<h4 id="H12.5.6.24">12.5.6.24 Projection annotations</h4>

<p class="location">Change the first paragraph as follows:</p>

<p>A <i>projection annotation (PDF 2.0)</i> is a markup annotation subtype (see 12.5.6.2, "Markup annotations") that has much of the functionality of other markup annotations.
However, a projection annotation is only valid within the context of an associated run-time environment, such as an activated 3D model<ins onMouseEnter="mouseEnter(this)" data-issue="94">, and thus an <b>AP</b> dictionary is not required</ins>.</p>

<p>...</p>

<p class="location">Delete the last paragraph as follows:</p>

<p><del onMouseEnter="mouseEnter(this)" data-issue="42" data-iso="approved">A projection annotation with a <b>Rect</b> entry that has zero height or zero width shall not have an <b>AP</b> dictionary.</del></p>



<h2 id="H12.6">12.6 Actions</h2>

<h3 id="H12.6.4">12.6.4 Action types</h3>

<h4 id="H12.6.4.2">12.6.4.2 Go-To actions</h4>

<p class="location">Change Table 202 as follows:</p>

<table>
  <caption id="Table202">Table 202 - Additional entries specific to a go-to action</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>D</b></td>
    <td>name, byte string, or array</td>
    <td>
     <p>(<i>Required</i>) The <ins onMouseEnter="mouseEnter(this)" data-issue="140">explicit destination or named</ins> destination to jump to (see 12.3.2, "Destinations").
     </p>
    </td>
  </tr>
</table>


<h2 id="H12.7">Forms</h2>

<h3 id="H12.7.4">12.7.4 Field dictionaries</h3>

<h4 id="H12.7.4.1">12.7.4.1 General</h4>

<p class="location">Change Table 226 as follows:</p>

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
    (<i><del onMouseEnter="mouseEnter(this)" data-issue="28" data-iso="approved">Required</del>
        <ins onMouseEnter="mouseEnter(this)" data-issue="28" data-iso="approved">Optional</ins></i>)
    The partial field name (see 12.7.4.2, "Field names").
    </td>
  </tr>
</table>

<h4 id="H12.7.5.5">12.7.5.5 Signature Fields</h4>

<p class="location">Change Table 236 as follows:</p>

<table>
  <caption id="Table236">Table 236 - Entries in a signature field lock dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>P</b></td>
    <td>number</td>
    <td>
    <p>(<i>Optional; PDF 2.0</i>) The access permissions granted for this document. <ins onMouseEnter="mouseEnter(this)" data-issue="131" data-iso="approved">Changes to a PDF that are incremental updates which include only the data necessary to add DSS’s 12.8.4.3, "Document Security Store (DSS)" and/or document timestamps 12.8.5, "Document timestamp (DTS) dictionary" to the document shall not be considered as changes to the document as defined in the choices below.</ins></p>
    <p>...</p>
    </td>
  </tr>
</table>

<p>...</p>

<p class="location">Change Table 237 as follows:</p>

<table>
  <caption id="Table237">Table 237 - Entries in a signature field seed value dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>DigestMethod</b></td>
    <td>array</td>
    <td>
    <p>(<i>Optional; PDF 1.7</i>) An <ins onMouseEnter="mouseEnter(this)" data-issue="159">unordered</ins> array of names indicating acceptable digest
    algorithms to use while signing. <del onMouseEnter="mouseEnter(this)" data-issue="159">The value
    </del><ins onMouseEnter="mouseEnter(this)" data-issue="159">Array values</ins> shall be <i>SHA1</i> (<i>deprecated with PDF 2.0</i>), <i>SHA256</i>,
    <i>SHA384</i>, <i>SHA512</i> <del onMouseEnter="mouseEnter(this)" data-issue="159">and</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="159">or</ins> <i>RIPEMD160</i>. The default value is implementation-specific.
    </p>
    <p><del onMouseEnter="mouseEnter(this)" data-issue="158">This property is only applicable if the digital credential signing contains RSA public/private
    keys. If it contains DSA public/private keys, the digest algorithm is always SHA-1 and this attribute shall be ignored.</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="158">Some signature mechanisms require a specific digest function to be used. In such cases, the value of this entry shall be ignored.</ins>
    </p>
    </td>
  </tr>
  <tr>
    <td><b>AddRevInfo</b></td>
    <td>boolean</td>
    <td><p  class="hangingindent">
    NOTE 3 <del onMouseEnter="mouseEnter(this)" data-issue="4" data-iso="approved"><i>adbe.pkcs7.detached</i></del> <ins onMouseEnter="mouseEnter(this)" data-issue="4" data-iso="approved"><i>adbe.x509.rsa_sha1</i></ins>
    and <i>adbe.pkcs7.sha1</i> are deprecated in PDF 2.0.</p></td>
  </tr>
</table>

<h3 id="H12.7.6">12.7.6 Form actions</h3>

<h4 id="H12.7.6.2">12.7.6.2 Submit-form action</h4>

<p class="location">Change Table 239 as follows:</p>

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
    <p>(<i>Optional<del onMouseEnter="mouseEnter(this)" data-issue="122" data-iso="approved">; inheritable</del></i>) ... </p>
    </td>
  </tr>
  <tr>
    <td><b>CharSet</b></td>
    <td>string</td>
    <td>
    <p>(<i>Optional<del onMouseEnter="mouseEnter(this)" data-issue="122" data-iso="approved">; inheritable</del></i>) ... </p>
    </td>
  </tr>
</table>

<h4 id="H12.7.6.3">12.7.6.3 Reset-form action</h4>

<p class="location">Change Table 242 as follows:</p>

<table>
  <caption id="Table242">Table 242 - Flag for reset-form actions</caption>
  <tr>
    <th>Bit position</th>
    <th>Name</th>
    <th>Meaning</th>
  </tr>
  <tr>
    <td>1</td>
    <td>Include/Exclude</td>
    <td>
    <p>
    If clear, the <b>Fields</b> array (see "Table 241 — Additional entries specific to a reset-form action") specifies which fields to reset.
    (All descendants of the specified fields in the field hierarchy are reset as well.) If set, the <b>Fields</b> array indicates which fields
    to exclude from resetting; that is, all fields in the document’s interactive form shall be reset <i>except</i> those listed in the <b>Fields</b> array.
    <ins onMouseEnter="mouseEnter(this)" data-issue="174">(All descendants of the specified fields in the field hierarchy are also exempt from being reset.)</ins>
    </p>
    </td>
  </tr>
</table>


<h3 id="H12.7.8">12.7.8 Forms data format</h3>

<h4 id="H12.7.8.1">12.7.8.1 General</h4>

<p>...</p>

<p class="location">Change the last paragraph as follows:</p>

<p>
FDF shall use the MIME media type <ins onMouseEnter="mouseEnter(this)" data-issue="176"><code>application/fdf</code>, or the deprecated alias</ins> <code>application/vnd.fdf</code>.
On the Microsoft Windows&trade; and UNIX platforms, FDF files shall have the extension <code>.fdf</code>; on Mac OS, they shall have file type 'FDF'.
</p>

<p class="location">Add the following NOTE after the last paragraph:</p>

<p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="176">
NOTE See <a href="https://www.iana.org/assignments/media-types/application/fdf">https://www.iana.org/assignments/media-types/application/fdf</a> for more information.
</ins></p>

<h3 id="H12.7.9">12.7.9 Non-interactive forms</h3>

<p class="location">Change the first paragraph as follows:</p>

<p>
Unlike interactive forms, non-interactive forms do not use widget annotations but are represented with page content. Non-interactive forms are defined by the
<b>PrintField</b> attrib<del onMouseEnter="mouseEnter(this)" data-issue="54" data-iso="approved">0</del>ute (14.8.5.6, "PrintField attributes") for repurposing and accessibility purposes.
</p>


<h3 id="H12.8.1">12.8.1 General</h3>

<p class="location">Change the list item below NOTE 2 as follows:</p>

<p>A PDF document may contain the following standard types of signatures:</p>
<ul>
  <li><p>...</p></li>
  <li>
  Any number of document timestamp signatures, see 12.8.5, "Document timestamp (DTS) dictionary". The timestamp signature dictionary of a document timestamp signature
  shall be the value of a signature field and shall contain a <b>ByteRange</b> entry. <ins onMouseEnter="mouseEnter(this)" data-issue="55" data-iso="approved">These shall follow the certification signature if one is present.</ins>
  </li>
</ul>

<p>A signature dictionary is used by all of these types of signatures.</p>

<p class="location">Change Table 255 as follows:</p>

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
    <p>(<i>Required<del onMouseEnter="mouseEnter(this)" data-issue="121" data-iso="approved">; inheritable</del></i>) ... </p>
    </td>
  </tr>
  <tr>
    <td><b>Cert</b></td>
    <td>byte string or array</td>
    <td>
    <p>...</p>
    <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="4" data-iso="approved">NOTE <i>adbe.x509.rsa_sha1</i> and <i>adbe.pkcs7.sha1</i> are deprecated in PDF 2.0.</ins></p>
    </td>
  </tr>
</table>

<p>...</p>

<p class="location">Change Table 256 as follows:</p>

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
    <p>(<i><del onMouseEnter="mouseEnter(this)" data-issue="117" data-iso="approved">Required</del><ins onMouseEnter="mouseEnter(this)" data-issue="117" data-iso="approved">Optional; deprecated in PDF 2.0</ins></i>) ... </p>
    </td>
  </tr>
</table>

<h3 id="H12.8.2">12.8.2 Transform methods</h3>

<h4 id="H12.8.2.2">12.8.2.2 DocMDP</h4>

<h5 id="H12.8.2.2.2">12.8.2.2.2 Validating signatures that use the DocMDP transform method</h5>

<p class="location">Change Table 257 as follows:</p>

<table>
  <caption id="Table257">Table 257 - Entries in the DocMDP transform parameters dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>P</b></td>
    <td><del onMouseEnter="mouseEnter(this)" data-issue="152">number</del><ins onMouseEnter="mouseEnter(this)" data-issue="152">integer</ins></td>
    <td>
    <p>...</p>
    </td>
  </tr>
</table>

<h4 id="H12.8.2.4">12.8.2.4 FieldMDP</h4>

<p class="location">Change Table 259 as follows:</p>

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
    (<i>Required if <b>Action</b> is Include or Exclude</i>) An array of text strings containing <ins onMouseEnter="mouseEnter(this)" data-issue="33" data-iso="approved">fully qualified</ins>
    field names <ins onMouseEnter="mouseEnter(this)" data-issue="33" data-iso="approved">(see 12.7.4.2 "Field names")</ins>.
    </td>
  </tr>
</table>

<h3 id="H12.8.3">12.8.3 Signature interoperability</h3>

<h4 id="H12.8.3.1">12.8.3.1 General</h4>

<p class="location">Change Table 260 as follows:</p>

<table>
  <caption id="Table260">Table 260 - SubFilter value algorithm support</caption>
  <tr>
    <th>SubFilter values</th>
    <th>adbe.pkcs7.detached,<br/>ETSI.CAdES.detached or<br/>ETSI.RFC3161</th>
    <th>adbe.pkcs7.sha1 <sup>c</sup> </th>
    <th>adbe.x509.rsa_sha1 <sup>a</sup> <ins onMouseEnter="mouseEnter(this)" data-issue="4" data-iso="approved"><sup>c</sup></ins></th>
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

<p class="editornote">EDITOR NOTE: Table 260 italic formatting of PDF versions (such as "(<i>PDF 1.5</i>)") is inconsistently applied and needs to be corrected.</p>

</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
