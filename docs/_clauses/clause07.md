---
number: 7
title: Syntax
---

<style>
  .iso32000 {
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


<div class="iso32000">


# 7. Syntax


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


</div>

