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
    <td><p>
    (<i>Optional; PDF 1.2</i>) The file containing the stream data. If this entry is present, the bytes between <b>stream</b> and <b>endstream</b>
    shall be ignored. However, the <b>Length</b> entry <span class="deleted-text">should<span class="deleted-tooltiptext">Issue #10</span></span>
    <span class="new-text">shall<span class="new-tooltiptext">Issue #10</span></span> still specify the
    number of those bytes (usually, there are no bytes and <b>Length</b> is 0). The filters that are applied to the file data shall be specified by
    <b>FFilter</b> and the filter parameters shall be specified by <b>FDecodeParms</b>.
    </p></td>
  </tr>
</table>


<h3>7.4.9 JPXDecode filter</h3>


...<br/>

<p>
Data used in PDF image XObjects shall be limited to the JPX baseline set of features,  <span class="deleted-text">except for<span class="deleted-tooltiptext">
Issue #29</span></span>
<span class="new-text">excluding<span class="new-tooltiptext">Issue #29</span></span> enumerated colour space 19 (CIEJab).
In addition, enumerated colour space 12 (CMYK), which is part of JPX but not JPX baseline, shall be supported in a PDF file. JPX file
structures used in PDF files shall conform to the JPEG 2000 specification.
</p>


...<br/>

<h3>7.6.4 Standard security handler</h3>

<h5>7.6.4.3.3 Algorithm 2.A: Retrieving the file encryption key from an encrypted document in order to decrypt it (revision 6 and later)</h5>

<ol type="a" start="6">
<li>
Decrypt the 16-byte <b>Perms</b> string using AES-256 in ECB mode <span class="deleted-text">with an initialization vector of zero
<span class="deleted-tooltiptext">Issue #24</span></span> and the file encryption key as the key. ...
</li>
</ol>

<h5>7.6.4.4.9 Algorithm 10: Computing the encryption dictionary's Perms (permissions) value (Security handlers of revision 6)</h5>

<ol type="a" start="6">
<li>
Encrypt the 16-byte block using AES-256 in ECB mode <span class="deleted-text">with an initialization vector of zero
<span class="deleted-tooltiptext">Issue #24</span></span>, using the file encryption key as the key.
The result (16 bytes) is stored as the <b>Perms</b> string, and checked for validity when the file is opened.
</li>
</ol>

<h5>7.6.4.4.12 Algorithm 13: Validating the permissions (Security handlers of revision 6)</h5>

<ol type="a" start="1">
<li>
Decrypt the 16 byte <b>Perms</b> string using AES-256 in ECB mode <span class="deleted-text">with an initialization vector of zero
<span class="deleted-tooltiptext">Issue #24</span></span> and the file encryption key as the key. ...
</li>
</ol>

<h4>7.6.5.3 Public-key encryption algorithms</h4>

<p><i>New notes added at the end of sub-clause 7.6.5.3:</i></p>

<span class="new-text">
<p>NOTE 1: This means that step c) only applies when both of the following conditions are met:</p>

<ul>
<li>the key is being generated for the crypt filter named <i>DefaultCryptFilter</i> (i.e. the crypt filter used as the value for <b>StmF</b> in the encryption dictionary);</li>
<li>the <b>EncryptMetadata</b> entry of the associated crypt filter dictionary is set to <i>false</i>.</li>
</ul>

<p>NOTE 2: Since crypt filters are not supported when <b>SubFilter</b> is set to <i>adbe.pkcs7.s3</i> or <i>adbe.pkcs7.s4</i> in the encryption dictionary,
there is no way to specify that metadata is to be left unencrypted in these cases. In particular, step c) is always skipped for these <b>SubFilter</b> values.</p>
<span class="new-tooltiptext">Issue #25</span>
</span>


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
    <td><p>
    (<i>Required</i>) If the crypt filter is referenced from <b>StmF</b> or <b>StrF</b> in the encryption dictionary, this entry shall be an array of byte strings,
    where each <span class="new-text">byte<span class="new-tooltiptext">Issue #16</span></span> string shall be a binary-encoded CMS object that shall ...
    <br/>...<br/>
    If the crypt filter is referenced from a <b>Crypt</b> filter decode parameter dictionary (see "Table 14 - Optional parameters for Crypt filters"),
    this entry shall be a <span class="new-text">byte<span class="new-tooltiptext">Issue #16</span></span> string that shall be a binary-encoded CMS object that shall ...
    </p></td>
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

<h3>7.10.3 Type 2 (exponential interpolation) functions</h3>


...<br/>

<p>Values of <b>Domain</b> shall constrain <i>x</i> in such a way that<span class="new-text">: <span class="new-tooltiptext">Issue #30</span></span></p>

<ul>
    <li><span class="new-text">if <b>N</b> is not an integer, all values of <i>x</i> will be non-negative; and<span class="new-tooltiptext">Issue #30</span></span></li>
    <li><span class="new-text">if <b>N</b> is negative, no value of <i>x</i> will be zero.<span class="new-tooltiptext">Issue #30</span></span></li>
</ul>

<p>Typically, <b>Domain</b> is declared as [0.0 1.0], and <b>N</b> is a positive number. To clip the output to a specified range the <b>Range</b> attribute shall be used.</p>


...<br/>

<h3>7.11.6 Collection items</h3>


<table>
  <caption>Table 47 - Entries in a collection subitem dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>D</b></td>
    <td>text string, date or number</td>
    <td><p>
    (<i>Optional</i>) The data corresponding to the related entry in the collection field dictionary (see "Table 155 - Entries in a collection field dictionary").
    The type of data shall match the data type identified by the corresponding collection field dictionary. <span class="deleted-text">Default: <i>none</i>.<span class="deleted-tooltiptext">Issue #37</span></span>
    </p></td>
  </tr>
  <tr>
    <td><b>P</b></td>
    <td>text string</td>
    <td><p>
    (<i>Optional</i>) A prefix string that shall be concatenated with the text string presented to the user. This entry is ignored when an interactive PDF
    processor sorts the items in the collection. <span class="deleted-text">Default: <i>none</i>.<span class="deleted-tooltiptext">Issue #37</span></span>
    </p></td>
  </tr>
</table>


</div>


<br/><hr>
<p class="footnote">Last modified: 16 April 2021</p>

</body>
</html>
