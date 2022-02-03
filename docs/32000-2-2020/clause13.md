---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 13
title: Multimedia features
modified: 4 February 2022
---

<ul class="noprint">
 <li><a href="#H13.1">13.1 General</a>
 </li>
 <li>13.6 3D Artwork
  <ul>
   <li><a href="#H13.6.2">13.6.2 3D annotations</a>
   </li>
   <li>13.6.3 3D streams
    <ul>
     <li><a href="#H13.3.6.1">13.3.6.1 General</a>
     </li>
    </ul>
   </li>
   <li>13.6.4 3D Views
    <ul>
     <li><a href="#H13.6.4.1">13.6.4.1 General</a>
     </li>
     <li><a href="#H13.6.4.3">13.6.4.3 3D background dictionaries</a>
     </li>
     <li><a href="#H13.6.4.6">13.6.4.6 3D cross section dictionaries</a>
     </li>
    </ul>
   </li>
   <li>13.7 Rich media
    <ul>
     <li>13.7.2 RichMedia annotations
      <ul>
       <li>13.7.2.2 RichMediaSettings dictionary
        <ul>
         <li><a href="#H13.7.2.2.2">13.7.2.2.2 RichMediaActivation dictionary</a>
         </li>
        </ul>
       </li>
       <li>13.7.2.3 RichMediaContent dictionary
        <ul>
         <li><a href="#H13.7.2.3.1">13.7.2.3.1 General</a>
         </li>
         <li><a href="#H13.7.2.3.4">13.7.2.3.4 RichMediaInstance dictionary</a>
         </li>
        </ul>
       </li>
      </ul>
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

<h2 id="H13.1">13.1 General</h2>

<p>This clause describes those features of PDF that support embedding and playing multimedia content. It contains the following subclauses:</p>
<ul>
<li>13.2, "Multimedia" describes the comprehensive set of multimedia capabilities that were introduced in PDF 1.5.</li>
<li>13.3, "Sounds" and 13.4, "Movies" describe deprecated features superseded by 13.7, "<ins onMouseEnter="mouseEnter(this)" data-issue="109">Rich media".</ins></li>
<li>13.6, "3D Artwork" describes the capability of embedding three-dimensional graphics in a document, introduced in PDF 1.6.</li>
<li>13.7, "<ins onMouseEnter="mouseEnter(this)" data-issue="109">Rich media" describes rich media annotations providing a common framework for video, audio, animations and other multimedia presentations.</ins></li>
</ul>

<h3 id="H13.6.2">13.6.2 3D annotations</h3>

<p>
3D annotations (<i>PDF 1.6</i>) are a way to include 3D artwork in PDF documents. Rich media annotations are another method (see <del onMouseEnter="mouseEnter(this)" data-issue="142">0 "<br/>
Rich media"</del><ins onMouseEnter="mouseEnter(this)" data-issue="142">13.7 "Rich media"</ins>). "Table 309 — Additional entries specific to a 3D annotation" shows the entries specific to a 3D annotation dictionary. "Table 166 — Entries common to all annotation dictionaries" describes the entries common to all annotation dictionaries.
</p>

<h3 id="H13.6.3">13.6.3 3D streams</h3>

<h4 id="H13.3.6.1">13.3.6.1 General</h4>


<table>
  <caption id="Table311">Table 311 - Entries in a 3D stream dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>ColorSpace</b></td>
    <td>name or array</td>
    <td>
    (<i>Optional, PDF 2.0</i>) The RGB colour space in which the 3D artwork's colour values are encoded. Valid values are the name
    <b>DeviceRGB</b>, an array specifying a valid <b>CalRGB</b> color space (see 8.6.5.3 "CalRGB colour spaces"), or an array specifying
    a valid RGB-based <b>ICCBased</b> color space (see 8.6.5.5 "ICCBased colour spaces").
    <ins onMouseEnter="mouseEnter(this)" data-issue="18">If the name is <b>DeviceRGB</b> and the page where the annotation referencing the 3D stream is used has a <b>DefaultRGB</b> color space, then the <b>DefaultRGB</b> color space shall be used (see 8.6.5.6 Default colour spaces).</ins>
    If this key is not present, the colour space for the 3D artwork colour values  <del onMouseEnter="mouseEnter(this)" data-issue="18">are</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="18">is</ins> considered undefined and a PDF processor may choose any appropriate
    RGB-based colour space, such as sRGB.
    </td>
  </tr>
</table>

<h3 id="H13.6.4">13.6.4 3D Views</h3>

<h4 id="H13.6.4.1">13.6.4.1 General</h4>

<table>
  <caption id="Table315">Table 315 - Entries in a 3D view dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>P</b></td>
    <td>dicionary</td>
    <td>
    <p>...</p>
    <p>Default value: a projection dictionary where the value of <b>Subtype</b> is
    <del onMouseEnter="mouseEnter(this)" data-issue="91"><i>Perspective</i></del><ins onMouseEnter="mouseEnter(this)" data-issue="91"><i>P</i> (perspective)</ins>,
    the value of <b>FOV</b> is 90, and all other entries take their default values.
    </p>
    </td>
  </tr>
  <tr>
    <td><b>NA</b></td>
    <td>array</td>
    <td>
    <p>(<i>Optional; PDF 1.7; <del onMouseEnter="mouseEnter(this)" data-issue="150">meaningful only if <b>NR</b> is present</del></i>) An array ...
    </p>
    </td>
  </tr>
</table>


<h4 id="H13.6.4.3">13.6.4.3 3D background dictionaries</h4>

<p>...</p>

<p><i>New paragraph is added before existing NOTE:</i></p>

<ins onMouseEnter="mouseEnter(this)" data-issue="39">PDF processors that render 3D data streams shall do so directly and without regard to keys and values in the annotation dictionary that define appearance streams or how appearance streams would be rendered onto the page. They shall ignore the values of the <b>C</b>, <b>IC</b>, <b>Border</b>, <b>BS</b>, <b>BE</b>, <b>BM</b>, <b>CA</b> and <b>ca</b> keys from "Table 166 - Entries common to all annotation dictionaries".</ins>

<p>...</p>


<table>
  <caption id="Table317">Table 317 - Entries in a 3D background dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>CS</b></td>
    <td>name <del onMouseEnter="mouseEnter(this)" data-issue="38">or array</del></td>
    <td>
    <p>(<i>Optional</i>) The colour space of the background. The only valid value shall be the name <i>DeviceRGB</i>.</p>
    <p>Default value: <i>DeviceRGB</i>.</p>
    <p><del onMouseEnter="mouseEnter(this)" data-issue="38">PDF consumers shall be prepared to encounter other values that may be supported in future versions of PDF.</del></p>
    </td>
  </tr>
  <tr>
    <td><b>C</b></td>
    <td><del onMouseEnter="mouseEnter(this)" data-issue="38">(various)</del>
        <ins onMouseEnter="mouseEnter(this)" data-issue="38">array</ins>
    </td>
    <td>
    <p>(<i>Optional</i>)
    <ins onMouseEnter="mouseEnter(this)" data-issue="38">An array of 3 numbers in the range 0.0 to 1.0, representing the</ins>
    <del onMouseEnter="mouseEnter(this)" data-issue="38">The</del>
    colour of the background in the colour space defined by <b>CS</b>.</p>
    <p>Default value: an array [1 1 1] representing the colour white when the value of <b>CS</b> is <i>DeviceRGB</i>.</p>
    </td>
  </tr>
</table>


<h4 id="H13.6.4.6">13.6.4.6 3D cross section dictionaries</h4>


<table>
  <caption id="Table322">Table 322 - Entries in a 3D cross section dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="49"><b>PV</b></ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="49">boolean</ins></td>
    <td>
    <p>
    <ins onMouseEnter="mouseEnter(this)" data-issue="49">(<i>Optional</i>) A flag indicating the visibility of the cutting plane. If <i>true</i>, then the cutting plane shall be visible. If <i>false</i>, then the cutting plane shall not be visible.<br/>Default value: <i>true</i></ins>
    </p>
    </td>
  </tr>
  <tr>
    <td><b>IV</b></td>
    <td>boolean</td>
    <td>
    <p>...</p>
    <p>Default value: <del onMouseEnter="mouseEnter(this)" data-issue="50">false</del> <ins onMouseEnter="mouseEnter(this)" data-issue="50">true</ins></p>
    </td>
  </tr>
</table>


<h5 id="H13.7.2.2.2">13.7.2.2.2 RichMediaActivation dictionary</h5>


<table>
  <caption id="Table335">Table 335 - Entries in a RichMediaActivation dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>View</b></td>
    <td>dictionary</td>
    <td>
    <p>(<i>Optional; PDF 2.0</i>) An indirect object reference to a 3D view dictionary (see <del onMouseEnter="mouseEnter(this)" data-issue="127">"Table 315 — Entries in a 3D view dictionary"</del><ins onMouseEnter="mouseEnter(this)" data-issue="127">13.7.2.3.5, "View dictionary"</ins> that shall also be referenced by the <b>Views</b> array within the annotation’s RichMediaContent dictionary (see "Table 341 — Entries in a RichMediaContent dictionary").</p>
    <p>Default value: The first element in the <b>Views</b> array of the <del onMouseEnter="mouseEnter(this)" data-issue="145">annotation specified in the RichMediaContent dictionary</del> <ins onMouseEnter="mouseEnter(this)" data-issue="145">RichMediaContent dictionary specified in the annotation</ins>. If a <b>Views</b> array does not exist, default values for the components of a 3D view dictionary (see "Table 344 — Additional entries in a 3D view dictionary") are used.</p>
    </td>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="59"><b>Scripts</b></ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="59">array</ins></td>
    <td>
    <ins onMouseEnter="mouseEnter(this)" data-issue="59"><p>(<i>Optional; PDF 2.0</i>) An array of indirect object references to file specification dictionaries, each of which describe a JavaScript file that shall be present in the <b>Assets</b> name tree of the RichMediaContent dictionary. If the array has no elements, no script is executed.</p><p>Default value: an empty array.</p></ins>
    </td>
  </tr>
</table>

<h4 id="H13.7.2.3">13.7.2.3 RichMediaContent dictionary</h4>

<h5 id="H13.7.2.3.1">13.7.2.3.1 General</h5>

<table>
  <caption id="Table341">Table 341 - Entries in a RichMediaContent dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Views</b></td>
    <td>array</td>
    <td>
    <p>(<i>Optional; PDF 2.0</i>) An array where each element is an indirect object reference to a 3D view dictionary. See <del onMouseEnter="mouseEnter(this)" data-issue="127">"Table 315 — Entries in a 3D view dictionary" for the details of the entries of this dictionary</del><ins onMouseEnter="mouseEnter(this)" data-issue="127">13.7.2.3.5, "View dictionary"</ins>.</p>
    <p>...</p>
    </td>
  </tr>
</table>

<h5 id="H13.7.2.3.4">13.7.2.3.4 RichMediaInstance dictionary</h5>


<table>
  <caption id="Table343">Table 343 - Entries in a RichMediaInstance dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Asset</b></td>
    <td>dictionary</td>
    <td>
    <p>(<i>Required; PDF 2.0</i>) A dictionary that shall be an indirect object reference to a file specification dictionary that
    <del onMouseEnter="mouseEnter(this)" data-issue="58">is also</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="58">may also be</ins>
    referenced in the <b>Assets</b> name tree specified in the RichMediaContent dictionary of the annotation.
    </p>
    <p class="hangingindent">
    <ins onMouseEnter="mouseEnter(this)" data-issue="58">NOTE the RichMedia asset itself is not referenced by name, however other assets may be referenced from the RichMedia asset by name and thus need to be in the <b>Assets</b> name tree.</ins>
    </p>
    </td>
  </tr>
</table>

</div>

<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
