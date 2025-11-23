---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 13
title: Multimedia features
modified: 23 November 2025
---

<ul class="noprint">
 <li><a href="#H13.1">13.1 General</a>
 </li>
 <li>13.2 Multimedia
  <ul>
   <li>13.2.3 Renditions
    <ul>
     <li><a href="#H13.2.3.1">13.2.3.1 General</a>
     </li>
    </ul>
   </li>
   <li>13.2.4 Media clip objects
    <ul>
     <li><a href="#H13.2.4.2">13.2.4.2 Media clip data</a>
     </li>
    </ul>
   </li>
   <li>13.2.6 Media screen parameters
    <ul>
     <li><a href="#H13.2.6.1">13.2.6.1 General</a>
     </li>
    </ul>
   </li>
   <li>13.2.7 Other multimedia objects
    <ul>
     <li>13.2.7.2 Media players dictionary
      <ul>
       <li><a href="#H13.2.7.2.1">13.2.7.2.1 General</a>
       </li>
       <li><a href="#H13.2.7.2.2">13.2.7.2.2 Algorithm: Media Player</a>
       </li>
      </ul>
     </li>
    </ul>
   </li>
  </ul>
 </li>
 <li><a href="#H13.5">13.5 Alternate presentations</a>
 </li>
 <li>13.6 3D Artwork
  <ul>
   <li><a href="#H13.6.2">13.6.2 3D annotations</a>
   </li>
   <li>13.6.3 3D streams
    <ul>
     <li><a href="#H13.6.3.1">13.6.3.1 General</a>
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
     <li><a href="#H13.6.4.7">13.6.4.7 3D node dictionaries</a>
     </li>
    </ul>
   </li>
   <li>13.6.7 Persistence of 3D measurements and markups
    <ul>
     <li>13.6.7.3 3D measurement/markup dictionary
      <ul>
       <li><a href="#H13.6.7.3.3">13.6.7.3.3 3D perpendicular dimension measurement</a>
       </li>
       <li><a href="#H13.6.7.3.6">13.6.7.3.6 3D comment note</a>
       </li>
      </ul>
     </li>
    </ul>
   </li>
  </ul>
 </li>
 <li>13.7 Rich media
  <ul>
   <li>13.7.2 RichMedia annotations
    <ul>
     <li><a href="#H13.7.2.1">13.7.2.1 General</a>
     </li>
     <li>13.7.2.2 RichMediaSettings dictionary
      <ul>
       <li><a href="#H13.7.2.2.1">13.7.2.2.1 General</a>
       </li>
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

<hr>

<link rel="stylesheet" href="../assets/iso-style.css">
<div class="isostyle">
<div class="fixedpopup" id="issuelink">
    Issue #xxxx
</div>

<p class="fake-h1">{{ page.clause }}. {{ page.title }}</p>

<h2 id="H13.1">13.1 General</h2>

<p class="location">Change the bulleted list below the first paragraph as follows:</p>

<p>This clause describes those features of PDF that support embedding and playing multimedia content. It contains the following subclauses:</p>
<ul>
<li>13.2, "Multimedia" describes the comprehensive set of multimedia capabilities that were introduced in PDF 1.5.</li>
<li>13.3, "Sounds" and 13.4, "Movies" describe deprecated features superseded by 13.7, "<ins onMouseEnter="mouseEnter(this)" data-issue="109" data-iso="approved">Rich media".</ins></li>
<li>13.6, "3D Artwork" describes the capability of embedding three-dimensional graphics in a document, introduced in PDF 1.6.</li>
<li>13.7, "<ins onMouseEnter="mouseEnter(this)" data-issue="109" data-iso="approved">Rich media" describes rich media annotations providing a common framework for video, audio, animations and other multimedia presentations.</ins></li>
</ul>

<h2 id="H13.2">13.2 Multimedia</h2>
<h3 id="H13.2.3">13.2.3 Renditions</h3>
<h4 id="H13.2.3.1">13.2.3.1 General</h4>

<p class="location">Change Table 277 as follows:</p>

<table>
  <caption id="Table277">Table 277 - Entries common to all rendition dictionaries</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>N</b></td>
    <td>text string</td>
    <td>
     <p>(<i>Optional</i>) A <del onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="approved">Unicode</del><ins onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="approved">UTF-16BE</ins>-encoded
         text string specifying the name of the rendition for use in a user interface and for name tree lookup by ECMAScript actions.
     </p>
    </td>
  </tr>
</table>


<h3 id="H13.2.4">13.2.4 Media clip objects</h3>
<h4 id="H13.2.4.2">13.2.4.2 Media clip data</h4>

<p class="location">Change Table 285 as follows:</p>

<table>
  <caption id="Table285">Table 285 - Additional entries in a media clip data dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>CT</b></td>
    <td>ASCII string</td>
    <td>
    <p>(<i>Optional; shall not be present for form XObjects</i>) An ASCII string identifying the type of data in <b>D</b>. The string 
    <del onMouseEnter="mouseEnter(this)" data-issue="257" data-iso="approved">should</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="257" data-iso="approved">shall</ins> 
    conform to the content type specification described in <i>Internet RFC 2045</i>.</p>
    </td>
  </tr>
  <tr>
    <td><b>MH</b></td>
    <td>dictionary</td>
    <td>
     <p>(<i>Optional</i>) A dictionary whose entries (see
     <del onMouseEnter="mouseEnter(this)" data-issue="179" data-iso="approved">"Table 287 — Entries in a media clip data MH/BE dictionary"</del>
     <ins onMouseEnter="mouseEnter(this)" data-issue="179" data-iso="approved">"Table 289 — Entries in a media clip section MH/BE dictionary"</ins>)
     shall be honoured for the media clip data to be considered viable.
     </p>
    </td>
  </tr>
</table>

<p>...</p>

<p class="location">Delete the single sentence paragraph immediately below Table 286 as follows:</p>

<p><del onMouseEnter="mouseEnter(this)" data-issue="414" data-iso="approved">An unrecognised value shall be treated as <i>(TEMPNEVER)</i>.</del></p>

<p>...</p>

<h3 id="H13.2.6">13.2.6 Media screen parameters</h3>

<h4 id="H13.2.6.1">13.2.6.1 General</h4>

<p class="location">Change Table 293 as follows:</p>

<table>
  <caption id="Table293">Table 293 - Entries in a media screen parameters dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>BE</b></td>
    <td>dictionary</td>
    <td>
      <p>(<i>Optional</i>) A dictionary whose entries (see "Table 294 — Entries in a media screen parameters MH/BE dictionary")
      <del onMouseEnter="mouseEnter(this)" data-issue="662">should be honoured</del> 
      <ins onMouseEnter="mouseEnter(this)" data-issue="662">shall only be honoured in a 'best effort' sense.</ins>.</p>
    </td>
  </tr>
</table>


<h3 id="H13.2.7">13.2.7 Other multimedia objects</h3>

<h4 id="H13.2.7.2">13.2.7.2 Media players dictionary</h4>

<h5 id="H13.2.7.2.1">13.2.7.2.1 General</h5>

<p class="location">Move the last paragraph to below the heading "13.2.7.2.2 Algorithm: Media Player" as follows:</p>

<p><del onMouseEnter="mouseEnter(this)" data-issue="449" data-iso="approved">
Since both media clip data and media play parameters dictionaries may be employed in a play operation, and each may reference a media players dictionary, there is a potential for conflict between the contents of the two media players dictionaries.
</del></p>

<h5 id="H13.2.7.2.2">13.2.7.2.2 Algorithm: Media Player</h5>

<p><ins onMouseEnter="mouseEnter(this)" data-issue="449" data-iso="approved">
Since both media clip data and media play parameters dictionaries may be employed in a play operation, and each may reference a media players dictionary, there is a potential for conflict between the contents of the two media players dictionaries.
</ins></p>


<h2 id="H13.5">13.5 Alternate Presentations</h2>

<p class="location">Change NOTE 2 below Table 308 as follows:</p>

<p class="hangingindent">
NOTE 2: Typically, images are stored in the document as image XObjects (see 8.9.5, "Image dictionaries"), thereby allowing them to be shared between the standard PDF representation and the slideshow. Other media objects are stored 
<del onMouseEnter="mouseEnter(this)" data-issue="481" data-iso="approved">or embedded file streams (see 7.11.4, "Embedded file streams")</del> 
<ins onMouseEnter="mouseEnter(this)" data-issue="481" data-iso="approved">as file specification dictionaries (see 7.11.3, "File specification dictionaries"), typically with an embedded file stream</ins>.
</p>

<h2 id="H13.6">13.6 3D Artwork</h2>

<h3 id="H13.6.2">13.6.2 3D annotations</h3>

<p class="location">Change the first paragraph as follows:</p>

<p>
3D annotations (<i>PDF 1.6</i>) are a way to include 3D artwork in PDF documents. Rich media annotations are another method (see <del onMouseEnter="mouseEnter(this)" data-issue="142" data-iso="approved">0 "<br/>
Rich media"</del><ins onMouseEnter="mouseEnter(this)" data-issue="142" data-iso="approved">13.7 "Rich media"</ins>). "Table 309 — Additional entries specific to a 3D annotation" shows the entries specific to a 3D annotation dictionary. "Table 166 — Entries common to all annotation dictionaries" describes the entries common to all annotation dictionaries.
</p>

<h3 id="H13.6.3">13.6.3 3D streams</h3>

<h4 id="H13.6.3.1">13.6.3.1 General</h4>

<p class="location">Change Table 311 as follows:</p>

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
    <ins onMouseEnter="mouseEnter(this)" data-issue="18" data-iso="approved">If the name is <b>DeviceRGB</b> and the page where the annotation referencing the 3D stream is used has a <b>DefaultRGB</b> color space, then the <b>DefaultRGB</b> color space shall be used (see 8.6.5.6 Default colour spaces).</ins>
    If this key is not present, the colour space for the 3D artwork colour values  <del onMouseEnter="mouseEnter(this)" data-issue="18" data-iso="approved">are</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="18" data-iso="approved">is</ins> considered undefined and a PDF processor may choose any appropriate
    RGB-based colour space, such as sRGB.
    </td>
  </tr>
  <tr>
    <td><b>Resources</b></td>
    <td>name tree</td>
    <td>
    <p>
      (<i>Optional<ins onMouseEnter="mouseEnter(this)" data-issue="362" data-iso="approved">; Deprecated in PDF 2.0</ins></i>) A name tree that maps name strings to objects that may be used by applications or scripts to modify the default view of the 3D artwork.
    </p>
    <p>
      The names in this name tree shall be text strings so as to be encoded in a way that will be accessible from ECMAScript.
    </p>
    <p class="hangingindent">
    <ins onMouseEnter="mouseEnter(this)" data-issue="362" data-iso="approved">NOTE <b>Resources</b> was deprecated in PDF 2.0 because it was insufficiently specified to ensure interoperable implementations.</ins>
    </p>
    </td>
  </tr>
</table>

<h3 id="H13.6.4">13.6.4 3D Views</h3>

<h4 id="H13.6.4.1">13.6.4.1 General</h4>

<p class="location">Change Table 315 as follows:</p>

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
    <del onMouseEnter="mouseEnter(this)" data-issue="91" data-iso="approved"><i>Perspective</i></del><ins onMouseEnter="mouseEnter(this)" data-issue="91" data-iso="approved"><i>P</i> (perspective)</ins>,
    the value of <b>FOV</b> is 90, and all other entries take their default values.
    </p>
    </td>
  </tr>
  <tr>
    <td><b>NA</b></td>
    <td>array</td>
    <td>
    <p>(<i>Optional; PDF 1.7; <del onMouseEnter="mouseEnter(this)" data-issue="150" data-iso="approved">meaningful only if <b>NR</b> is present</del></i>) An array ...
    </p>
    </td>
  </tr>
</table>


<h4 id="H13.6.4.3">13.6.4.3 3D background dictionaries</h4>

<p class="location">Insert the following new paragraph before the existing NOTE:</p>

<ins onMouseEnter="mouseEnter(this)" data-issue="39" data-iso="approved">PDF processors that render 3D data streams shall do so directly and without regard to keys and values in the annotation dictionary that define appearance streams or how appearance streams would be rendered onto the page. They shall ignore the values of the <b>C</b>, <b>IC</b>, <b>Border</b>, <b>BS</b>, <b>BE</b>, <b>BM</b>, <b>CA</b> and <b>ca</b> keys from "Table 166 - Entries common to all annotation dictionaries".</ins>

<p>...</p>

<p class="location">Change Table 317 as follows:</p>

<table>
  <caption id="Table317">Table 317 - Entries in a 3D background dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>CS</b></td>
    <td>name <del onMouseEnter="mouseEnter(this)" data-issue="38" data-iso="approved">or array</del></td>
    <td>
    <p>(<i>Optional</i>) The colour space of the background. The only valid value shall be the name <i>DeviceRGB</i>.</p>
    <p>Default value: <i>DeviceRGB</i>.</p>
    <p><del onMouseEnter="mouseEnter(this)" data-issue="38" data-iso="approved">PDF consumers shall be prepared to encounter other values that may be supported in future versions of PDF.</del></p>
    </td>
  </tr>
  <tr>
    <td><b>C</b></td>
    <td><del onMouseEnter="mouseEnter(this)" data-issue="38" data-iso="approved">(various)</del>
        <ins onMouseEnter="mouseEnter(this)" data-issue="38" data-iso="approved">array</ins>
    </td>
    <td>
    <p>(<i>Optional</i>)
    <ins onMouseEnter="mouseEnter(this)" data-issue="38" data-iso="approved">An array of 3 numbers in the range 0.0 to 1.0, representing the</ins>
    <del onMouseEnter="mouseEnter(this)" data-issue="38" data-iso="approved">The</del>
    colour of the background in the colour space defined by <b>CS</b>.</p>
    <p>Default value: an array [1 1 1] representing the colour white when the value of <b>CS</b> is <i>DeviceRGB</i>.</p>
    </td>
  </tr>
</table>


<h4 id="H13.6.4.6">13.6.4.6 3D cross section dictionaries</h4>

<p class="location">Change Table 322 as follows:</p>

<table>
  <caption id="Table322">Table 322 - Entries in a 3D cross section dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="49" data-iso="approved"><b>PV</b></ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="49" data-iso="approved">boolean</ins></td>
    <td>
    <p>
    <ins onMouseEnter="mouseEnter(this)" data-issue="49" data-iso="approved">(<i>Optional</i>) A flag indicating the visibility of the cutting plane. If <i>true</i>, then the cutting plane shall be visible. If <i>false</i>, then the cutting plane shall not be visible.<br/>Default value: <i>true</i></ins>
    </p>
    </td>
  </tr>
  <tr>
    <td><b>IV</b></td>
    <td>boolean</td>
    <td>
    <p>...</p>
    <p>Default value: <del onMouseEnter="mouseEnter(this)" data-issue="50" data-iso="approved">false</del> <ins onMouseEnter="mouseEnter(this)" data-issue="50" data-iso="approved">true</ins></p>
    </td>
  </tr>
</table>


<h4 id="H13.6.4.7">13.6.4.7 3D node dictionaries</h4>

<p class="location">Change Table 323 as follows:</p>

<table>
  <caption id="Table323">Table 323 - Entries in a 3D node dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>N</b></td>
    <td>text string</td>
    <td>
    <p>
    (<i>Required</i>) The name of the node being described by the node dictionary. All names in the node dictionary shall be unique. Interpretation of this entry shall depend upon the 3D format <del onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved">specified in the Subtype entry in "Table 311 — Entries in a 3D stream dictionary" as described below:</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved">and annotation type as defined in Table 323a below.</ins>
    </p>
    <p><del onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved"><i>U3D</i> If the <b>Subtype</b> of the corresponding 3D Stream is <i>U3D</i>, this entry shall correspond to the field Node block name, specified in the Universal 3D file format.</del>
    </p>
    <p><del onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved"><i>PRC</i> (<i>PDF 2.0</i>) If the <b>Subtype</b> of the corresponding 3D Stream is <i>PRC</i>, this entry shall be the Unique Identifier (UUID) as specified in ISO 14739-1.</del>
    </p>
    <p class="hangingindent">NOTE 1 When comparing this entry to node names for a particular<del onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved"> convention (such as Universal 3D or PRC)</del><ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved">3D model format</ins>, PDF processors will need to translate between the PDF text encoding used by PDF and the character encoding specified in the stream specified in the 3D stream.
    </p>
    <p class="hangingindent">NOTE 2 The description of the value of the <b>N</b> key was clarified in this document (2020).
    </p>
    </td>
  </tr>
</table>

<p class="location">Insert this new table below Table 323:</p>

<table>
  <caption id="Table323a"><ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved">Table 323a - Interpretation of 3D Node Subtype entry</ins></caption>
  <tr>
    <th>3D model format</th>
    <th>When using a 3D annotation</th>
    <th>When using a RichMedia annotation (<i>PDF 2.0</i>)</th>
  </tr>
  <tr>
   <td><ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved">U3D</ins></td>
   <td>
   <ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved">
    The <b>Subtype</b> of the corresponding 3D Stream shall be <i>U3D</i> (see Table 311 "Entries in a 3D stream dictionary") and the value of the
    <b>N</b> entry in the 3D node dictionary (see Table 323 "Entries in a 3D node dictionary") shall correspond to the field Node block name, 
    specified in the Universal 3D file format (ECMA-363).
    </ins>
   </td>
   <td>
   <ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved">
    (<i>PDF 2.0</i>) The <b>Subtype</b> of the corresponding Embedded File Specification dictionary (see Table 44 "Additional entries in an embedded file stream dictionary")
    shall be the registered IANA MIME media type for U3D "<code>model/u3d</code>" (when expressed as a PDF name is <i>model#2Fu3d</i>) and the value of
    the <b>N</b> entry in the 3D node dictionary (see Table 323 "Entries in a 3D node dictionary") shall correspond to the field Node block name,
    specified in the Universal 3D file format (ECMA-363).
   </ins>
   </td>
  </tr>
  <tr>
   <td><ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved">PRC (<i>PDF 2.0</i>)</ins></td>
   <td>
   <ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved">
    (<i>PDF 2.0</i>) The <b>Subtype</b> of the corresponding 3D Stream shall be <i>PRC</i> (see Table 311 "Entries in a 3D stream dictionary") and the value of the
    <b>N</b> entry in the 3D node dictionary (see Table 323 "Entries in a 3D node dictionary") shall be the Unique Identifier (UUID) as specified 
    in ISO 14739-1.
   </ins>
   </td>
   <td>
   <ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved">
    (<i>PDF 2.0</i>) The <b>Subtype</b> of the corresponding Embedded File Specification dictionary (see Table 44 "Additional entries in an embedded file stream dictionary") 
    shall be the registered IANA MIME media type for PRC "<code>model/prc</code>" (when expressed as a PDF name is <i>model#2Fprc</i>) and the value of the <b>N</b> entry in the 3D node dictionary (see Table 323 "Entries in a 3D node dictionary") shall be the Unique Identifier (UUID) as specified in ISO 14739-1.
   </ins>
   </td>
  </tr>
  <tr>
   <td><ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved">STEP (<i>PDF 2.0; see ISO/TS 24064</i>)</ins></td>
   <td><ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved">Prohibited.</ins></td>
   <td>
   <ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="approved">
    (<i>PDF 2.0</i>) The <b>Subtype</b> of the corresponding Embedded File Specification dictionary (see Table 44 "Additional entries in an embedded file stream dictionary") shall be one of the
    registered IANA MIME media types for STEP ("<code>model/step</code>", "<code>model/step+xml</code>", "<code>model/step+zip</code>", "<code>model/step-xml+zip</code>")
    and the value of the <b>N</b> entry in the 3D node dictionary (see Table 323 "Entries in a 3D node dictionary") shall be the unique identifier 
    (UUID), specified in the STEP AP 242 stream.
   </ins>
   </td>
  </tr>
</table>

<h3 id="H13.6.7">13.6.7 Persistence of 3D measurements and markups</h3>

<h4 id="H13.6.7.3">13.6.7.3 3D measurement/markup dictionary</h4>

<h5 id="H13.6.7.3.3">13.6.7.3.3 3D perpendicular dimension measurement</h5>

<p class="location">Change the paragraph above Table 328 as follows:</p>

<p>
In addition to the entries in "Table 326 — Entries in a 3D measurement/markup dictionary common to 
all markup subtypes", the following entries are defined for a 
<del onMouseEnter="mouseEnter(this)" data-issue="645"><b>I</b></del><ins onMouseEnter="mouseEnter(this)" data-issue="645">3D measurement dictionary</ins> 
with a <b>Subtype</b> value of <i>PD3</i> for 3D perpendicular measurement.
</p>

<p class="location">Modify Table 328 as follows:</p>

<table>
  <caption id="Table328">Table 328 - Additional entries in a 3D measurement/markup dictionary for a 3D perpendicular dimension measurement</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td>
      <b>A1</b>
      <ins onMouseEnter="mouseEnter(this)" data-issue="645"><i>(digit 1)</i></ins>
    </td>
    <td>array</td>
    <td>...</td>
  </tr>
  <tr>
    <td>
      <b>N1</b>
      <ins onMouseEnter="mouseEnter(this)" data-issue="645"><i>(digit 1)</i></ins>
    </td>
    <td>array</td>
    <td>...</td>
  </tr>
  <tr>
    <td>
      <b>D1</b>
      <ins onMouseEnter="mouseEnter(this)" data-issue="645"><i>(digit 1)</i></ins>
    </td>
    <td>array</td>
    <td>...</td>
  </tr>
</table>




<h5 id="H13.6.7.3.6">13.6.7.3.6 3D comment note</h5>

<p class="location">Modify Table 331 as follows:</p>

<table>
  <caption id="Table331">Table 331 - Additional entries in a 3D measurement/markup dictionary for a 3D comment note</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>S</b></td>
    <td>dictionary</td>
    <td>
      (<i>Optional; PDF 2.0</i>) A comment reference is an indirect reference to a projection annotation that may be associated with this 3D measurement. 
      <del onMouseEnter="mouseEnter(this)" data-issue="283" data-iso="approved">See "Table 341 — Entries in a RichMediaContent dictionary".</del>
      <ins onMouseEnter="mouseEnter(this)" data-issue="283" data-iso="approved">See 13.6.7.4, "3D measurements and projection annotations" .</ins>
    </td>
  </tr>
</table>



<h3 id="H13.7.2">13.7.2 RichMedia annotations</h3>

<h4 id="H13.7.2.1">13.7.2.1 General</h4>

<p class="location">Modify the first paragraph as follows:</p>

<p>
The annotation subtype <i>RichMedia</i> shares many low-level structural similarities with the 3D Artwork
defined in 13.6, "3D Artwork". At the top level, the <i>rich media annotation</i> has two primary custom structures.
The <i>RichMediaSettings dictionary</i> <del onMouseEnter="mouseEnter(this)" data-issue="163" data-iso="approved">is</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="163" data-iso="approved">, if present, shall be</ins> unique to each annotation,
while the <i>RichMediaContent dictionary</i> can be shared across rich-media annotations.
</p>

<p>...</p>

<p class="location">Change Table 333 as follows:</p>

<table>
  <caption id="Table333">Table 333 - Additional entries specific to a RichMedia annotation</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>RichMediaSettings</b></td>
    <td>dictionary</td>
    <td>
    <p>(<i>Optional; PDF 2.0</i>) A RichMediaSettings dictionary that <ins onMouseEnter="mouseEnter(this)" data-issue="163" data-iso="approved">shall be unique to each annotation and</ins>
    stores conditions and responses that determine when the annotation should be activated and deactivated by an interactive
    PDF processor and the initial state of artwork in those states. See "Table 334 — Entries in a RichMediaSettings dictionary".
    </p>
    <p>...</p>
    </td>
  </tr>
</table>


<h4 id="H13.7.2.2">13.7.2.2 RichMediaSettings dictionary</h4>

<h5 id="H13.7.2.2.1">13.7.2.2.1 General</h5>

<p class="location">Modify the first paragraph as follows:</p>

<p>
The <i>RichMediaSettings dictionary</i> has a purpose similar to that of the 3D activation dictionary ("Table 310 — Entries in a 3D
activation dictionary") with the 3D Annotation described in 13.6.2, "3D Annotations". The RichMediaSettings dictionary stores the
conditions and responses that occur in response to certain events, such as activation and deactivation of the annotation, and contains two dictionaries.
<ins onMouseEnter="mouseEnter(this)" data-issue="163" data-iso="approved">It shall be unique to each annotation.</ins>
"Table 334 — Entries in a RichMediaSettings dictionary" gives the details of the content of this dictionary.
</p>


<h5 id="H13.7.2.2.2">13.7.2.2.2 RichMediaActivation dictionary</h5>

<p class="location">Change Table 335 as follows:</p>

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
    <p>(<i>Optional; PDF 2.0</i>) An indirect object reference to a 3D view dictionary (see <del onMouseEnter="mouseEnter(this)" data-issue="127" data-iso="approved">"Table 315 — Entries in a 3D view dictionary"</del><ins onMouseEnter="mouseEnter(this)" data-issue="127" data-iso="approved">13.7.2.3.5, "View dictionary"</ins> that shall also be referenced by the <b>Views</b> array within the annotation’s RichMediaContent dictionary (see "Table 341 — Entries in a RichMediaContent dictionary").</p>
    <p>Default value: The first element in the <b>Views</b> array of the <del onMouseEnter="mouseEnter(this)" data-issue="145" data-iso="approved">annotation specified in the RichMediaContent dictionary</del> <ins onMouseEnter="mouseEnter(this)" data-issue="145" data-iso="approved">RichMediaContent dictionary specified in the annotation</ins>. If a <b>Views</b> array does not exist, default values for the components of a 3D view dictionary (see "Table 344 — Additional entries in a 3D view dictionary") are used.</p>
    </td>
  </tr>
  <tr>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="59" data-iso="approved"><b>Scripts</b></ins></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="59" data-iso="approved">array</ins></td>
    <td>
    <ins onMouseEnter="mouseEnter(this)" data-issue="59" data-iso="approved"><p>(<i>Optional; PDF 2.0</i>) An array of indirect object references to file specification dictionaries, each of which describe a JavaScript file that shall be present in the <b>Assets</b> name tree of the RichMediaContent dictionary. If the array has no elements, no script is executed.</p>
    <p>Default value: an empty array.</p></ins>
    </td>
  </tr>
</table>

<h4 id="H13.7.2.3">13.7.2.3 RichMediaContent dictionary</h4>

<h5 id="H13.7.2.3.1">13.7.2.3.1 General</h5>

<p class="location">Change Table 341 as follows:</p>

<table>
  <caption id="Table341">Table 341 - Entries in a RichMediaContent dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Configurations</b></td>
    <td>array</td>
    <td>
    <p>(<i><del onMouseEnter="mouseEnter(this)" data-issue="166" data-iso="approved">Optional</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="166" data-iso="approved">Required</ins>;
    PDF 2.0</i>) A <ins onMouseEnter="mouseEnter(this)" data-issue="166" data-iso="approved">non-empty</ins> array where each element is
    an indirect object reference to a RichMediaConfiguration dictionary.</p>
    </td>
  </tr>
  <tr>
    <td><b>Views</b></td>
    <td>array</td>
    <td>
    <p>(<i>Optional; PDF 2.0</i>) An array where each element is an indirect object reference to a 3D view dictionary. See <del onMouseEnter="mouseEnter(this)" data-issue="127" data-iso="approved">"Table 315 — Entries in a 3D view dictionary" for the details of the entries of this dictionary</del><ins onMouseEnter="mouseEnter(this)" data-issue="127" data-iso="approved">13.7.2.3.5, "View dictionary"</ins>.</p>
    <p>...</p>
    </td>
  </tr>
</table>

<h5 id="H13.7.2.3.4">13.7.2.3.4 RichMediaInstance dictionary</h5>

<p class="location">Change Table 343 as follows:</p>

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
    <del onMouseEnter="mouseEnter(this)" data-issue="58" data-iso="approved">is also</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="58" data-iso="approved">may also be</ins>
    referenced in the <b>Assets</b> name tree specified in the RichMediaContent dictionary of the annotation.
    </p>
    <p class="hangingindent">
    <ins onMouseEnter="mouseEnter(this)" data-issue="58" data-iso="approved">NOTE the RichMedia asset itself is not referenced by name, however other assets may be referenced from the RichMedia asset by name and thus need to be in the <b>Assets</b> name tree.</ins>
    </p>
    </td>
  </tr>
</table>

</div>

<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
