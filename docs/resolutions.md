---
---

<style>
  body {
    font-family: Cambria, Georgia, serif;
  }
  .new-text {
    background-color: lightyellow;
    color: green;
    position: relative;
    display: inline-block;
  }
  .new-tooltiptext {
    font-family: Arial, Helvetica, sans-serif;
    visibility: hidden;
    color: green;
    background-color: lightyellow;
    border-radius: 6px;
    padding: 5px 0;
    text-align: center;
    min-width: 80px;
    border: 3px solid green;
    /* Position the tooltip */
    position: absolute;
    z-index: 1;
    bottom: 100%;
    left: 50%;
    margin-left: -50%;
  }

  .new-text .new-tooltiptext::after {
    content: "";
  }

  .new-text:hover .new-tooltiptext {
    visibility: visible;
    opacity: 1;
  }

  .deleted-text {
    background-color: seashell;
    color: red;
    text-decoration: line-through;
    text-decoration-color: red;
    position: relative;
    display: inline-block;
  }

  .deleted-tooltiptext {
    font-family: Arial, Helvetica, sans-serif;
    visibility: hidden;
    background-color: seashell;
    color: red;
    min-width: 80px;
    text-align: center;
    border-radius: 6px;
    border: 3px solid red;
    padding: 5px 0;
    /* Position the tooltip */
    position: absolute;
    z-index: 1;
    bottom: 100%;
    left: 50%;
    margin-left: -50%;
  }
  .deleted-text .deleted-tooltiptext::after {
    content: "";
  }
  .deleted-text:hover .deleted-tooltiptext {
    visibility: visible;
    opacity: 1;
  }

  table {
    margin-left: auto;
    margin-right: auto;
    border-collapse: collapse;
    border: 1px solid black;
  }
  caption {
    font-weight: bold;
  }
  th {
    text-align: left;
    border-collapse: collapse;
    border: 1px solid black;
    border-top: solid thick;
    border-bottom: solid thick;
  }
  td {
    text-align: left;
    min-width: 50px;
    max-width: 500px;
    border-collapse: collapse;
    border: 1px solid black;
  }
</style>


#### 7.3.8.2 Stream extent


<table>
  <caption>Table 5 - Entries common to all stream dictionaries</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>F</b></td>
    <td>file specification</td>
    <td>
    (<i>Optional; PDF 1.2</i>) The file containing the stream data. If this entry is present, the bytes between <b>stream</b> and <b>endstream</b>
    shall be ignored. However, the <b>Length</b> entry <span class="deleted-text">should<span class="deleted-tooltiptext">Issue #10</span></span>
    <span class="new-text">shall<span class="new-tooltiptext">Issue #10</span></span> still specify the
    number of those bytes (usually, there are no bytes and <b>Length</b> is 0). The filters that are applied to the file data shall be specified by
    <b>FFilter</b> and the filter parameters shall be specified by <b>FDecodeParms</b>.
    </td>
  </tr>
</table>


### 7.4.9 JPXDecode filter


...<br/>


Data used in PDF image XObjects shall be limited to the JPX baseline set of features,  <span class="deleted-text">except for<span class="deleted-tooltiptext">
Issue #29</span></span>
<span class="new-text">excluding<span class="new-tooltiptext">Issue #29</span></span> enumerated colour space 19 (CIEJab).
In addition, enumerated colour space 12 (CMYK), which is part of JPX but not JPX baseline, shall be supported in a PDF file. JPX file
structures used in PDF files shall conform to the JPEG 2000 specification.



##### 7.6.4.3.3 Algorithm 2.A: Retrieving the file encryption key from an encrypted document in order to decrypt it (revision 6 and later)


f) Decrypt the 16-byte <b>Perms</b> string using AES-256 in ECB mode <span class="deleted-text">with an initialization vector of zero
<span class="deleted-tooltiptext">Issue #24</span></span> and the file encryption key as the key. ...


##### 7.6.4.4.9 Algorithm 10: Computing the encryption dictionary's Perms (permissions) value (Security handlers of revision 6)


f) Encrypt the 16-byte block using AES-256 in ECB mode <span class="deleted-text">with an initialization vector of zero
<span class="deleted-tooltiptext">Issue #24</span></span>, using the file encryption key as the key.
The result (16 bytes) is stored as the <b>Perms</b> string, and checked for validity when the file is opened.


##### 7.6.4.4.12 Algorithm 13: Validating the permissions (Security handlers of revision 6)


a) Decrypt the 16 byte <b>Perms</b> string using AES-256 in ECB mode <span class="deleted-text">with an initialization vector of zero
<span class="deleted-tooltiptext">Issue #24</span></span> and the file encryption key as the key. ...


### 7.6.6 Crypt filters


<table>
  <caption>Table 27 - Additional crypt filter dictionary entries for public-key security handlers</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Recipients</b></td>
    <td><span class="new-text">byte<span class="new-tooltiptext">Issue #16</span></span> string or array</td>
    <td>
    (<i>Required</i>) If the crypt filter is referenced from <b>StmF</b> or <b>StrF</b> in the encryption dictionary, this entry shall be an array of byte strings,
    where each <span class="new-text">byte<span class="new-tooltiptext">Issue #16</span></span> string shall be a binary-encoded CMS object that shall ...
    <br/>...<br/>
    If the crypt filter is referenced from a <b>Crypt</b> filter decode parameter dictionary (see "Table 14 - Optional parameters for Crypt filters"),
    this entry shall be a <span class="new-text">byte<span class="new-tooltiptext">Issue #16</span></span> string that shall be a binary-encoded CMS object that shall ...
    </td>
  </tr>
</table>


### 7.8.3 Resource dictionaries


...<br/>


<ul>
<li>
For a content stream that is the value of a page's <b>Contents</b> entry <span class="deleted-text">(or is an element of an
array that is the value of that entry)<span class="deleted-tooltiptext">Issue #9</span></span>, the resource dictionary shall
be designated by the page dictionary's <b>Resources</b> entry or is inherited, as described under 7.7.3.4, "Inheritance of page
attributes" from some ancestor node of the page object. ...
</li>
</ul>


...<br/>


### 8.9.5 Image dictionaries


#### 8.9.5.1. General


<table>
  <caption>Table 87 - Additional entries specific to an image dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Intent</b></td>
    <td>name</td>
    <td>...<br/><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext">Issue #13</span></span></td>
  </tr>
  <tr>
    <td><b>ImageMask</b></td>
    <td>boolean</td>
    <td>(<i>Optional</i>) A flag indicating whether the image shall be treated as an image mask (see 8.9.6, "Masked images"). If this flag is <i>true</i>,
    the value of <b>BitsPerComponent</b>, if present, shall be 1 and <span class="deleted-text">Mask<span class="deleted-tooltiptext">Issue #14</span></span>
    <span class="new-text"><b>Mask</b><span class="new-tooltiptext">Issue #14</span></span> and <b>ColorSpace</b> shall not be specified; unmasked areas shall be
    painted using the current nonstroking colour. Default value: <i>false</i>.
    </td>
  </tr>
  <tr>
    <td><b>Alternates</b></td>
    <td>array</td>
    <td>...<br/><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext">Issue #13</span></span></td>
  </tr>
  <tr>
    <td><b>SMask</b></td>
    <td>stream</td>
    <td>...<br/><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext">Issue #13</span></span></td>
  </tr>
  <tr>
    <td><b>Name</b></td>
    <td>name</td>
    <td>...<br/><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext">Issue #13</span></span></td>
  </tr>
  <tr>
    <td><b>StructParent</b></td>
    <td>integer</td>
    <td>...<br/><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext">Issue #13</span></span></td>
  </tr>
  <tr>
    <td><b>ID</b></td>
    <td>byte string</td>
    <td>...<br/><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext">Issue #13</span></span></td>
  </tr>
</table>


### 8.9.7 Inline images


...<br/>


Inline image objects shall not be nested; that is, two <b>BI</b> operators shall not appear without an intervening <b>EI</b> to close the first object.
Similarly, an <b>ID</b> operator shall only appear between a <b>BI</b> and its balancing <b>EI</b>. Unless the image uses <b>ASCIIHexDecode</b> or
<b>ASCII85Decode</b> as <span class="deleted-text">one of its filters<span class="deleted-tooltiptext">Issue #20</span></span>
<span class="new-text">its final or only filter<span class="new-tooltiptext">Issue #20</span></span>, the <b>ID</b> operator shall be followed by a
single white-space character, and the next character shall be interpreted as the first byte of image data.


The key-value pairs appearing between the <b>BI</b> and <b>ID</b> operators (as listed in "Table 91 - Entries in an inline
image object") are analogous to their respective key-value pairs in an image XObject dictionary (see "Table 87 - Additional
entries specific to an image dictionary") or a stream dictionary (see "Table 5 - Entries common to all stream dictionaries").
For convenience, the abbreviations shown in "Table 91 - Entries in an inline image object" and "Table 92 - Additional
abbreviations in an inline image object" may be used in place of the full names. <span class="new-text">In the situation where
both an abbreviated key name and the corresponding full key name from Table 91 are present, the abbreviated key name shall take
precedence.<span class="new-tooltiptext">Issue #3</span></span> Entries other than those listed shall be ignored.


...<br/>


<span class="deleted-text">NOTE 3 The names <b>DeviceGray</b>, <b>DeviceRGB</b>, and <b>DeviceCMYK</b> (as well as their abbreviations <b>G</b>, <b>RGB</b>, and <b>CMYK</b>) always
identify the corresponding colour spaces directly; they never refer to resources in the <b>ColorSpace</b> subdictionary.<span class="deleted-tooltiptext">Issue #19</span></span>


<span class="new-text">The names <b>DeviceGray</b>, <b>DeviceRGB</b>, and <b>DeviceCMYK</b> (as well as their abbreviations <b>G</b>, <b>RGB</b>, and <b>CMYK</b>) never refer to
resources in the <b>ColorSpace</b> subdictionary; they always identify the corresponding colour spaces either directly or via a default colour space (see
8.6.5.6 "Default colour spaces").<span class="new-tooltiptext">Issue #19</span></span>


...<br/>


## 9.8 Font descriptors


### 9.8.1 General


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
    The PostScript name of the font. This name shall be the same as the value of <b>BaseFont</b> in the font or CIDFont dictionary
    that refers to this font descriptor.
    </td>
  </tr>
</table>


#### 9.8.3.3 FD


...<br/>


The key for each entry in an <b>FD</b> dictionary shall be the name of a class of glyphs - that is, a particular subset of the CIDFont's
character collection. The entry's value shall be a font descriptor whose contents shall <span class="new-text">be a subset of the keys defined
in "Table 120 - Entries common to all font descriptors" that<span class="new-tooltiptext">Issue #5</span></span> override the font-wide attributes for that
class only. This font descriptor <span class="deleted-text">shall contain<span class="deleted-tooltiptext">Issue #5</span></span><span class="new-text">contains<span
class="new-tooltiptext">Issue #5</span></span> entries for metric information only; it shall not include <b>FontFile</b>, <b>FontFile2</b>,
<b>FontFile3</b>, or any of the entries listed in <span class="deleted-text">"Table 120 - Entries common to all font descriptors"
<span class="deleted-tooltiptext">Issue #5</span></span><span class="new-text">"Table 122 - Additional font descriptor entries for CIDFonts"
<span class="new-tooltiptext">Issue #5</span></span>.


#### 10.6.5.6 Type 5 halftones


<table>
  <caption>Table 132 - Entries in a Type 5 halftone dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Default</b></td>
    <td>dictionary or<br/>stream</td>
    <td>
    (<i>Required</i>) A halftone that shall be used for any colourant or colour component that does not have an entry of its own.
    <span class="deleted-text">The value shall not be 5.<span class="deleted-tooltiptext">Issue #12</span></span>
    <span class="new-text">The halftone shall not be a Type 5 halftone.<span class="new-tooltiptext">Issue #12</span></span>
    If there are any nonprimary colourants, the default halftone shall have a transfer function.
    </td>
  </tr>
</table>


## 12.2 Viewer preferences


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


### 12.5.2 Annotation dictionaries


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


#### 12.7.5.5 Signature Fields


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


### 12.8.1 Signature Fields


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


#### 12.8.2.4 FieldMDP


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


### 12.8.3 Signature interoperability


#### 12.8.3.1 General


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


### 13.6.3 3D streams

### 13.3.6.1 General


<table>
  <caption>Table 311 - Entries in a 3d stream dictionary</caption>
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
    <span class="new-text">If the name is <b>DeviceRGB</b> and the page where the annotation referencing the 3D stream is used has a <b>DefaultRGB</b> color space,
    then the <b>DefaultRGB</b> color space shall be used (see 8.6.5.6 Default colour spaces).<span class="new-tooltiptext">Issue #18</span></span>
    If this key is not present, the colour space for the 3D artwork colour values  <span class="deleted-text">are<span class="deleted-tooltiptext">Issue #18</span></span>
    <span class="new-text">is<span class="new-tooltiptext">Issue #18</span></span> considered undefined and a PDF processor may choose any appropriate
    RGB-based colour space, such as sRGB.
    </td>
  </tr>
</table>


### 14.13.5 Associated files linked to graphics objects


...<br/>


The property list associated with the marked-content shall specify an array of file specification dictionaries to which
the content is associated. The named resource in the <span class="deleted-text"><b>Property List</b><span class="deleted-tooltiptext">
Issue #14</span></span> <span class="new-text"><i>property list</i><span class="new-tooltiptext">Issue #14</span></span>
(see 14.6.2, "Property lists") shall specify an array of file specification dictionaries to which the content is associated.
The relationship that the associated files have to the PDF content is supplied by the AFRelationship key in each file specification dictionary.


...<br/>


