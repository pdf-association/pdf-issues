---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 12
title: Interactive features
---

{% include iso-style.html %}
<div class="isostyle">


<h1>{{ page.clause }}. {{ page.title }}</h1>


<h2>12.2 Viewer preferences</h2>


<table>
  <caption>Table 147 - Entries in a viewer preferences dictionary</caption>
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
    (see <span class="deleted-text">7.7.3, "Page tree"<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span>
    <span class="new-text">"Table 31 - entries in a page object<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <span class="deleted-text"><b>CropBox</b><span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span>
    <span class="new-text"><i>CropBox</i><span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span>
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
    (see <span class="deleted-text">7.7.3, "Page tree"<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span>
    <span class="new-text">"Table 31 - entries in a page object<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <span class="deleted-text"><b>CropBox</b><span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span>
    <span class="new-text"><i>CropBox</i><span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span>
    <br/>...
    </td>
  </tr>
  <tr>
    <td><b>PrintArea</b></td>
    <td>name</td>
    <td>
    (<i>Optional; PDF 1.4; deprecated in PDF 2.0</i>) The name of the page boundary representing the area of a page that shall be
    rendered when printing the document. The value is the key designating the relevant page boundary in the page object
    (see <span class="deleted-text">7.7.3, "Page tree"<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span>
    <span class="new-text">"Table 31 - entries in a page object<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <span class="deleted-text"><b>CropBox</b><span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span>
    <span class="new-text"><i>CropBox</i><span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span>
    <br/>...
    </td>
  </tr>
  <tr>
    <td><b>PrintClip</b></td>
    <td>name</td>
    <td>
    (<i>Optional; PDF 1.4; deprecated in PDF 2.0</i>) The name of the page boundary to which the contents of the page shall be clipped
    when printing the document. The value is the key designating the relevant page boundary in the page object
    (see <span class="deleted-text">7.7.3, "Page tree"<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span>
    <span class="new-text">"Table 31 - entries in a page object<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <span class="deleted-text"><b>CropBox</b><span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span>
    <span class="new-text"><i>CropBox</i><span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span>
    <br/>...
    </td>
  </tr>
</table>


<h3>12.4.2 Page labels <span class="new-text"> and indices<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/73" target="_blank">Issue #73</a></span></span></h3>


<p>...</p>


<h3>12.4.4 Presentations</h3>


<h4>12.4.4.1 General</h4>


<table>
  <caption>Table 164 - Entries in a transition dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Di</b></td>
    <td><span class="deleted-text">number<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/36" target="_blank">Issue #36</a></span></span><span class="new-text">integer<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/36" target="_blank">Issue #36</a></span></span> or name</td>
    <td>
      <p>...</p>
      <p>If the value is a <span class="deleted-text">number<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/36" target="_blank">Issue #36</a></span></span><span class="new-text">integer<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/36" target="_blank">Issue #36</a></span></span>, it shall be one of:</p>
      <p>...</p>
    </td>
  </tr>
</table>


<h3>12.5.2 Annotation dictionaries</h3>


<table>
  <caption>Table 166 - Entries common to all annotation dictionaries</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>AP</b></td>
    <td>dictionary</td>
    <td>
    (<i><span class="deleted-text">Optional; PDF 1.2<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/22" target="_blank">Issue #22</a></span></span>
     <span class="new-text">Required except for conditions listed below (PDF 2.0); optional in PDF 1.2 through PDF 1.7<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/22" target="_blank">Issue #22</a></span></span></i>)
     An appearance dictionary specifying how the annotation shall be presented visually on the page ...
    </td>
  </tr>
</table>

<p>
<span class="deleted-text">A PDF reader shall render the appearance dictionary without regard to any other keys and values in the annotation dictionary and <span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/34" target="_blank">Issue #34</a></span></span>
<span class="new-text">When rendering the appearance dictionary, a PDF reader<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/34" target="_blank">Issue #34</a></span></span>

shall ignore the values of the <b>C</b>, <b>IC</b>, <b>Border</b>, <b>BS</b>, <b>BE</b>,
<span class="deleted-text"><b>BM</b>,<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/34" target="_blank">Issue #34</a></span></span>
<b>CA</b>, <b>ca</b>, <b>H</b>, <b>DA</b>, <b>Q</b>, <b>DS</b>, <b>LE</b>, <b>LL</b>, <b>LLE</b>,
<span class="new-text"><b>MK</b>,<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/56" target="_blank">Issue #56</a></span></span>
and <b>Sy</b> keys.
</p>

<p>
<span class="new-text">NOTE 1 Some of these keys are only relevant to certain annotation subtypes as described in the following subclauses.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/34" target="_blank">Issue #34</a></span></span>
</p>


<p>
NOTE <span class="new-text">2<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/34" target="_blank">Issue #34</a></span></span> Requiring an appearance dictionary for each annotation ensures the reliable rendering of the annotations.
<span class="new-text">When an appearance dictionary is not present, the rendered appearance will be implementation dependent.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/34" target="_blank">Issue #34</a></span></span>
</p>

<h4>12.5.6.2 Markup annotations</h4>

<p>...</p>

<p>
When
<span class="new-text">providing the <b>Contents</b> key, if<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/90" target="_blank">Issue #90</a></span></span>
separating text into paragraphs, a CARRIAGE RETURN (0Dh) shall be used and not, for example, a LINE FEED character (0Ah).
</p>

<p>...</p>


<h4>12.5.6.5 Link annotations</h4>


<table>
  <caption>Table 176 - Additional entries specific to a link annotation</caption>
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
    <p><span class="new-text">NOTE 1 When <b>QuadPoints</b> is used, the activation area and the visual appearance (including border) of the link annotation are not
    required to be the same.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/17" target="_blank">Issue #17</a></span></span></p>
    <p>NOTE <span class="new-text">2<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/17" target="_blank">Issue #17</a></span></span> The last paragraph above was clarified in this document (2020).</p>
    </td>
  </tr>
</table>


<h4>12.5.6.6 Free text annotations</h4>

<table>
  <caption>Table 177 - Additional entries specific to a free text annotation</caption>
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
    <p>The annotation dictionary's <b>AP</b> entry <span class="deleted-text">, if present,<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/42" target="_blank">Issue #42</a></span></span> shall take precedence over the <b>DA</b> entry (see "Table 170 - Entries in an appearance dictionary" and 12.5.5, "Appearance streams").</p>
    </td>
  </tr>
</table>


<h4>12.5.6.18 Screen annotations</h4>

<p>...</p>

<ul>
<li>...</li>
<li>
The <b>AP</b> entry refers to an appearance dictionary (see "Table 170 - Entries in an appearance dictionary") whose normal appearance provides the visual
appearance for a screen annotation that shall be used for printing and default display when a media clip is not being played.
<span class="deleted-text">If <b>AP</b> is not present, the screen annotation shall not have a default visual appearance and shall not be printed.<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/42" target="_blank">Issue #42</a></span></span>
</li>
</ul>


<h4>12.5.6.24 Projection annotations</h4>

<p>A <i>projection annotation (PDF 2.0)</i> is a markup annotation subtype (see 12.5.6.2, "Markup annotations") that has much of the functionality of other markup annotations.
However, a projection annotation is only valid within the context of an associated run-time environment, such as an activated 3D model<span class="new-text">, and thus an <b>AP</b> dictionary is not required<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/94" target="_blank">Issue #94</a></span></span>.</p>

<p>...</p>


<p><span class="deleted-text">A projection annotation with a <b>Rect</b> entry that has zero height or zero width shall not have an <b>AP</b> dictionary.<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/42" target="_blank">Issue #42</a></span></span></p>

<h3>12.7.4 Field dictionaries</h3>


<h4>12.7.4.1 General</h4>


<table>
  <caption>Table 226 - Entries common to all field dictionaries</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>T</b></td>
    <td>text string</td>
    <td>
    (<i><span class="deleted-text">Required<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/28" target="_blank">Issue #28</a></span></span>
        <span class="new-text">Optional<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/28" target="_blank">Issue #28</a></span></span></i>)
    The partial field name (see 12.7.4.2, "Field names").
    </td>
  </tr>
</table>


<h4>12.7.5.5 Signature Fields</h4>


<table>
  <caption>Table 237 - Entries in a signature field seed value dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>AddRevInfo</b></td>
    <td>boolean</td>
    <td>NOTE 3 <span class="deleted-text"><i>adbe.pkcs7.detached</i><span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/4" target="_blank">Issue #4</a></span></span><span class="new-text"><i>adbe.x509.rsa_sha1</i>
    <span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/4" target="_blank">Issue #4</a></span></span> and <i>adbe.pkcs7.sha1</i> are deprecated in PDF 2.0.</td>
  </tr>
</table>


<h3>12.7.9 Non-interactive forms</h3>


<p>
Unlike interactive forms, non-interactive forms do not use widget annotations but are represented with page content. Non-interactive forms are defined by the
<b>PrintField</b> attrib<span class="deleted-text">0<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/54" target="_blank">Issue #54</a></span></span>ute (14.8.5.6, "PrintField attributes") for repurposing and accessibility purposes.
</p>


<h3>12.8.1 Signature Fields</h3>

<p>...</p>

<p>A PDF document may contain the following standard types of signatures:</p>
<ul>
  <li><p>...</p></li>
  <li>
  Any number of document timestamp signatures, see 12.8.5, "Document timestamp (DTS) dictionary". The timestamp signature dictionary of a document timestamp signature
  shall be the value of a signature field and shall contain a <b>ByteRange</b> entry. <span class="new-text">These shall follow the certification signature if one
  is present.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/55" target="_blank">Issue #55</a></span></span>
  </li>
</ul>

<p>A signature dictionary is used by all of these types of signatures.</p>

<table>
  <caption>Table 255 - Entries in a signature dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Cert</b></td>
    <td>byte string or array</td>
    <td>
    <p>...</p>
    <span class="new-text">NOTE <i>adbe.x509.rsa_sha1</i> and <i>adbe.pkcs7.sha1</i> are deprecated in PDF 2.0.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/4" target="_blank">Issue #4</a></span></span></td>
  </tr>
</table>


<h4>12.8.2.4 FieldMDP</h4>


<table>
  <caption>Table 259 - Entries in the FieldMDP transform parameters dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Fields</b></td>
    <td>array</td>
    <td>
    (<i>Required if <b>Action</b> is Include or Exclude</i>) An array of text strings containing <span class="new-text">fully qualified<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/33" target="_blank">Issue #33</a></span></span>
    field names <span class="new-text">(see 12.7.4.2 "Field names")<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/33" target="_blank">Issue #33</a></span></span>.
    </td>
  </tr>
</table>


<h3>12.8.3 Signature interoperability</h3>


<h4>12.8.3.1 General</h4>


<table>
  <caption>Table 260 - SubFilter value algorithm support</caption>
  <tr>
    <th>SubFilter values</th>
    <th>adbe.pkcs7.detached,<br/>ETSI.CAdES.detached or<br/>ETSI.RFC3161</th>
    <th>adbe.pkcs7.sha1 <sup>c</sup> </th>
    <th>adbe.x509.rsa_sha1 <sup>a</sup> <span class="new-text"><sup>c</sup><span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/4" target="_blank">Issue #4</a></span></span></th>
  </tr>
  <tr>
    <td>...</td>
    <td>...</td>
    <td>...</td>
    <td>...</td>
  </tr>
  <tr>
    <td colspan="4"><p>...</p>
    <sup>c</sup> The values <i>adbe.x509.rsa_sha1</i> and <i>adbe.pkcs7.sha1</i> have been deprecated with PDF 2.0.<br/>
    <p>...</p></td>
  </tr>
</table>

<p>
<span class="new-text"><sup>Note that in Table 260 italic formatting of PDF versions (such as "(<i>PDF 1.5</i>)") is inconsistently applied and needs to be corrected.</sup><span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/109" target="_blank">Issue #109</a></span></span>
<p>

</div>


<hr>
<p class="footnote">Last modified: 30 July 2021</p>
