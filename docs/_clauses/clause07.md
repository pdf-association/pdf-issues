---
number: 7
title: Syntax
---


<html>
<head>
<title>ISO 32000-2:2020 Clause 7: Syntax</title>
</head>
<body>


{% include iso-style.html %}


<div class="iso32000">


<h1>7. Syntax</h1>


<h4>7.3.8.2 Stream extent</h4>


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


<h3>7.4.9 JPXDecode filter</h3>


...<br/>


Data used in PDF image XObjects shall be limited to the JPX baseline set of features,  <span class="deleted-text">except for<span class="deleted-tooltiptext">
Issue #29</span></span>
<span class="new-text">excluding<span class="new-tooltiptext">Issue #29</span></span> enumerated colour space 19 (CIEJab).
In addition, enumerated colour space 12 (CMYK), which is part of JPX but not JPX baseline, shall be supported in a PDF file. JPX file
structures used in PDF files shall conform to the JPEG 2000 specification.



<h5>7.6.4.3.3 Algorithm 2.A: Retrieving the file encryption key from an encrypted document in order to decrypt it (revision 6 and later)</h5>


f) Decrypt the 16-byte <b>Perms</b> string using AES-256 in ECB mode <span class="deleted-text">with an initialization vector of zero
<span class="deleted-tooltiptext">Issue #24</span></span> and the file encryption key as the key. ...


<h5>7.6.4.4.9 Algorithm 10: Computing the encryption dictionary's Perms (permissions) value (Security handlers of revision 6)</h5>


f) Encrypt the 16-byte block using AES-256 in ECB mode <span class="deleted-text">with an initialization vector of zero
<span class="deleted-tooltiptext">Issue #24</span></span>, using the file encryption key as the key.
The result (16 bytes) is stored as the <b>Perms</b> string, and checked for validity when the file is opened.


<h5>7.6.4.4.12 Algorithm 13: Validating the permissions (Security handlers of revision 6)</h5>


a) Decrypt the 16 byte <b>Perms</b> string using AES-256 in ECB mode <span class="deleted-text">with an initialization vector of zero
<span class="deleted-tooltiptext">Issue #24</span></span> and the file encryption key as the key. ...


<h3>7.6.6 Crypt filters</h3>


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


<h3>7.8.3 Resource dictionaries</h3>


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


</div>


<br/><hr>
<p style="text-align:center">Last modified: 16 February 2021</p>

</body>
</html>
