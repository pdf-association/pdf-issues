---
number: 12
title: Interactive features
---


<html>
<head>
<title>ISO 32000-2:2020 Clause 12: Interactive features</title>
</head>
<body>


{% include iso-style.html %}


<div class="iso32000">


<h1>12. Interactive features</h1>


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
    (see <span class="deleted-text">7.7.3, "Page tree"<span class="deleted-tooltiptext">Issue #14</span></span>
    <span class="new-text">"Table 31 - entries in a page object<span class="new-tooltiptext">Issue #14</span></span> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <span class="deleted-text"><b>CropBox</b><span class="deleted-tooltiptext">Issue #14</span></span>
    <span class="new-text"><i>CropBox</i><span class="new-tooltiptext">Issue #14</span></span>
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
    (see <span class="deleted-text">7.7.3, "Page tree"<span class="deleted-tooltiptext">Issue #14</span></span>
    <span class="new-text">"Table 31 - entries in a page object<span class="new-tooltiptext">Issue #14</span></span> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <span class="deleted-text"><b>CropBox</b><span class="deleted-tooltiptext">Issue #14</span></span>
    <span class="new-text"><i>CropBox</i><span class="new-tooltiptext">Issue #14</span></span>
    <br/>...
    </td>
  </tr>
  <tr>
    <td><b>PrintArea</b></td>
    <td>name</td>
    <td>
    (<i>Optional; PDF 1.4; deprecated in PDF 2.0</i>) The name of the page boundary representing the area of a page that shall be
    rendered when printing the document. The value is the key designating the relevant page boundary in the page object
    (see <span class="deleted-text">7.7.3, "Page tree"<span class="deleted-tooltiptext">Issue #14</span></span>
    <span class="new-text">"Table 31 - entries in a page object<span class="new-tooltiptext">Issue #14</span></span> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <span class="deleted-text"><b>CropBox</b><span class="deleted-tooltiptext">Issue #14</span></span>
    <span class="new-text"><i>CropBox</i><span class="new-tooltiptext">Issue #14</span></span>
    <br/>...
    </td>
  </tr>
  <tr>
    <td><b>PrintClip</b></td>
    <td>name</td>
    <td>
    (<i>Optional; PDF 1.4; deprecated in PDF 2.0</i>) The name of the page boundary to which the contents of the page shall be clipped
    when printing the document. The value is the key designating the relevant page boundary in the page object
    (see <span class="deleted-text">7.7.3, "Page tree"<span class="deleted-tooltiptext">Issue #14</span></span>
    <span class="new-text">"Table 31 - entries in a page object<span class="new-tooltiptext">Issue #14</span></span> and 14.11.2, "Page boundaries").
    If the specified page boundary is not defined in the page object, its default value shall be used, as specified in "Table 31 - Entries in a page object".
    <br/>Default value: <span class="deleted-text"><b>CropBox</b><span class="deleted-tooltiptext">Issue #14</span></span>
    <span class="new-text"><i>CropBox</i><span class="new-tooltiptext">Issue #14</span></span>
    <br/>...
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
    (<i><span class="deleted-text">Optional<span class="deleted-tooltiptext">Issue #22</span></span>
     <span class="new-text"><i>Required except for conditions listed below</i><span class="new-tooltiptext">Issue #22</span></span>; PDF 1.2</i>)
     An appearance dictionary specifying how the annotation shall be presented visually on the page ...
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
    <td>NOTE 3 <span class="deleted-text">adbe.pkcs7.detached<span class="deleted-tooltiptext">Issue #4</span></span><span class="new-text">adbe.x509.rsa_sha1<span class="new-tooltiptext">Issue #4</span></span> and adbe.pkcs7.sha1 are deprecated in PDF 2.0.</td>
  </tr>
</table>


<h3>12.8.1 Signature Fields</h3>


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
    ...<br/>
    <span class="new-text">NOTE adbe.x509.rsa_sha1 and adbe.pkcs7.sha1 are deprecated in PDF 2.0.<span class="new-tooltiptext">Issue #4</span></span></td>
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
    (<i>Required if <b>Action</b> is Include or Exclude</i>) An array of text strings containing <span class="new-text">fully qualified<span class="new-tooltiptext">Issue #33</span></span>
    field names <span class="new-text">(see 12.7.4.2 "Field names")<span class="new-tooltiptext">Issue #33</span></span>.
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
    <th>adbe.x509.rsa_sha1 <sup>a</sup> <span class="new-text"><sup>c</sup><span class="new-tooltiptext">Issue #4</span></span></th>
  </tr>
  <tr>
    <td>...</td>
    <td>...</td>
    <td>...</td>
    <td>...</td>
  </tr>
  <tr>
    <td colspan="4">...<br/>
    <sup>c</sup> The values <i>adbe.x509.rsa_sha1</i> and <i>adbe.pkcs7.sha1</i> have been deprecated with PDF 2.0.<br/>
    ...</td>
  </tr>
</table>


</div>


<br/><hr>
<p class="footnote">Last modified: 16 February 2021</p>

</body>
</html>
