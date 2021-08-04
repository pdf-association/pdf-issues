---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 7
title: Syntax
modified: 30 July 2021
---

<link rel="stylesheet" href="../assets/iso-style.css">
<div class="isostyle">

<h1>{{ page.clause }}. {{ page.title }}</h1>


<h4 id="H7.3.8.2">7.3.8.2 Stream extent</h4>


<table>
  <caption id="Table5">Table 5 - Entries common to all stream dictionaries</caption>
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
    shall be ignored. However, the <b>Length</b> entry <span class="deleted-text">should<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/10" target="_blank">Issue #10</a></span></span>
    <span class="new-text">shall<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/10" target="_blank">Issue #10</a></span></span> still specify the
    number of those bytes (usually, there are no bytes and <b>Length</b> is 0). The filters that are applied to the file data shall be specified by
    <b>FFilter</b> and the filter parameters shall be specified by <b>FDecodeParms</b>.
    </p></td>
  </tr>
</table>

<h3 id="H7.4.3">7.4.3 ASCII85Decode filter</h3>

<p>...</p>

<p>The following conditions shall never occur in a correctly encoded byte sequence:</p>
<li>
    <ul>The value represented by a group of 5 characters is greater than <span class="deleted-text">232<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/98" target="_blank">Issue #98</a></span></span><span class="new-text">2<sup>32</sup><span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/98" target="_blank">Issue #98</a></span></span> - 1.</ul>
    <ul>A <i>z</i> character occurs in the middle of a group.</ul>
    <ul>A final partial group contains only one character.</ul>
</li>

<h3 id="H7.4.9">7.4.9 JPXDecode filter</h3>

<p>...</p>

<p>
Data used in PDF image XObjects shall be limited to the JPX baseline set of features, <span class="deleted-text">except for<span class="deleted-tooltiptext">
Issue #29</span></span>
<span class="new-text">excluding<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/29" target="_blank">Issue #29</a></span></span> enumerated colour space 19 (CIEJab).
In addition, enumerated colour space 12 (CMYK), which is part of JPX but not JPX baseline, shall be supported in a PDF file. JPX file
structures used in PDF files shall conform to the JPEG 2000 specification.
</p>

<p>...</p>

<h2 id="H7.5">7.5 File structure</h2>

<p>...</p>

<table>
  <caption id="Table15">Table 15 - Entries in the file trailer dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Prev</b></td>
    <td>integer</td>
    <td><p>
    (<i>Optional; present only if the file has more than one cross-reference section; shall be a direct object</i>)
    The byte offset from the beginning of the PDF file to the beginning of the previous cross-reference
    <span class="deleted-text">stream<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/101" target="_blank">Issue #101</a></span></span>
    <span class="new-text">section<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/101" target="_blank">Issue #101</a></span></span>.
    </p></td>
  </tr>
</table>

<h3 id="H7.5.4">7.5.4 Cross reference table</h3>

<p>...</p>

<p><span class="new-text">EXAMPLE 2 The cross-reference table sub-section line should have just a single SPACE between "0" and "6".<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/109" target="_blank">Issue #109</a></span></span></p>

<p><span class="new-text">EXAMPLE 3 The cross-reference table first sub-section line should have just a single SPACE between "0" and "1". The typeface of this example should be all monospaced and with single SPACEs between all cross-reference fields, and thus all fields vertically aligned.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/109" target="_blank">Issue #109</a></span></span></p>


<h3 id="H7.6.3">7.6.3 General encryption algorithm</h3>

<h4 id="H7.6.3.1">7.6.3.1 General</h4>

<p>...</p>

<p>NOTE 1 The name RC4™ is a registered trademark of RSA Security Inc. and cannot be used by third parties creating implementations of the algorithm. Proprietary implementations of the RC4 encryption algorithm are available under license from RSA Security Inc. For licensing information, contact: <span class="deleted-text">RSA Security Inc. 2955 Campus Drive, Suite 400, San Mateo, CA 94403-2507, USA, or<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/95" target="_blank">Issue #95</a></span></span> <a href="http://www.rsasecurity.com/">http://www.rsasecurity.com/</a>.</p>

<p>...</p>

<h3 id="H7.6.4">7.6.4 Standard security handler</h3>

<h4 id="H7.6.4.1">7.6.4.1 General</h4>

<p>...</p>

<p>
If a security handler of revision 4 or 5 is specified, the standard security handler shall support crypt filters (see 7.6.6, "Crypt filters").
The support shall be limited to the <b>Identity</b> crypt filter (see "Table 26 - Standard crypt filter names") and
<span class="deleted-text">crypt filters<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/89" target="_blank">Issue #89</a></span></span><span class="new-text">a crypt filter<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/89" target="_blank">Issue #89</a></span></span>named <b>StdCF</b> whose dictionaries contain an <b>AuthEvent</b> value of <i>DocOpen</i>. For revision 4, the filter <b>CFM</b> value shall be <i>V2</i> (RC4) or <i>AESV2</i> (AES-128). For revision 6, the filter <b>CFM</b> value shall be <i>AESV3</i> (AES-256). Public-Key security handlers in this case shall use <span class="deleted-text">crypt filters<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/89" target="_blank">Issue #89</a></span></span><span class="new-text">a crypt filter<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/89" target="_blank">Issue #89</a></span></span> named <b>DefaultCryptFilter</b> when all document content is encrypted, and shall use <span class="deleted-text">crypt filters<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/89" target="_blank">Issue #89</a></span></span><span class="new-text">a crypt filter<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/89" target="_blank">Issue #89</a></span></span> named <b>DefEmbeddedFile</b> when file attachments only are encrypted in place of <b>StdCF</b> name. This nomenclature shall not be used as an indicator of the type of the security handler or encryption. Use of security handler revisions 1, 2, 3, 4 and 5 is deprecated in PDF 2.0.
</p>

<p>...</p>

<h5 id="H7.6.4.3.3">7.6.4.3.3 Algorithm 2.A: Retrieving the file encryption key from an encrypted document in order to decrypt it (revision 6 and later)</h5>

<ol type="a" start="6">
<li>
Decrypt the 16-byte <b>Perms</b> string using AES-256 in ECB mode <span class="deleted-text">with an initialization vector of zero
<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/24" target="_blank">Issue #24</a></span></span> and the file encryption key as the key. ...
</li>
</ol>

<h5 id="H7.6.4.4.9">7.6.4.4.9 Algorithm 10: Computing the encryption dictionary's Perms (permissions) value (Security handlers of revision 6)</h5>

<ol type="a" start="6">
<li>
Encrypt the 16-byte block using AES-256 in ECB mode <span class="deleted-text">with an initialization vector of zero
<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/24" target="_blank">Issue #24</a></span></span>, using the file encryption key as the key.
The result (16 bytes) is stored as the <b>Perms</b> string, and checked for validity when the file is opened.
</li>
</ol>

<h5 id="H7.6.4.4.12">7.6.4.4.12 Algorithm 13: Validating the permissions (Security handlers of revision 6)</h5>

<ol type="a" start="1">
<li>
Decrypt the 16 byte <b>Perms</b> string using AES-256 in ECB mode <span class="deleted-text">with an initialization vector of zero
<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/24" target="_blank">Issue #24</a></span></span> and the file encryption key as the key. ...
</li>
</ol>

<h4 id="H7.6.5.3">7.6.5.3 Public-key encryption algorithms</h4>

<p><i>New notes added at the end of sub-clause 7.6.5.3:</i></p>

<div class="new-text">
<p>NOTE 1: This means that step c) only applies when both of the following conditions are met:</p>

<ul>
<li>the key is being generated for the crypt filter named <i>DefaultCryptFilter</i> (i.e. the crypt filter used as the value for <b>StmF</b> in the encryption dictionary);</li>
<li>the <b>EncryptMetadata</b> entry of the associated crypt filter dictionary is set to <i>false</i>.</li>
</ul>

<p>NOTE 2: Since crypt filters are not supported when <b>SubFilter</b> is set to <i>adbe.pkcs7.s3</i> or <i>adbe.pkcs7.s4</i> in the encryption dictionary,
there is no way to specify that metadata is to be left unencrypted in these cases. In particular, step c) is always skipped for these <b>SubFilter</b> values.</p>
<span class="new-tooltiptext">Issue #25</span>
</div>


<h3 id="H7.6.6">7.6.6 Crypt filters</h3>

<p>PDF 1.5 introduces crypt filters, which provide finer granularity control of encryption within a PDF file. The use of crypt filters involves the following structures:</p>

<ul>
  <li>The encryption dictionary (see "Table 20 - Entries common to all encryption dictionaries") contains entries that enumerate the crypt filters in the document (<b>CF</b>) and specify which ones are used by default to decrypt all the streams (<b>StmF</b>) and strings (<b>StrF</b>) in the document. In addition, the value of the V entry shall be 4 <span class="new-text">or 5<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/74" target="_blank">Issue #74</a></span></span> to use crypt filters.
  </li>
</ul>

<p>...</p>

<table>
  <caption id="Table27">Table 27 - Additional crypt filter dictionary entries for public-key security handlers</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Recipients</b></td>
    <td><span class="new-text">byte<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/16" target="_blank">Issue #16</a></span></span> string or array</td>
    <td>
    <p>(<i>Required</i>) If the crypt filter is referenced from <b>StmF</b> or <b>StrF</b> in the encryption dictionary, this entry shall be an array of byte strings,
    where each <span class="new-text">byte<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/16" target="_blank">Issue #16</a></span></span> string shall be a binary-encoded CMS object that shall ...</p>
    <p>...</p>
    <p>If the crypt filter is referenced from a <b>Crypt</b> filter decode parameter dictionary (see "Table 14 - Optional parameters for Crypt filters"),
    this entry shall be a <span class="new-text">byte<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/16" target="_blank">Issue #16</a></span></span> string that shall be a binary-encoded CMS object that shall ...</p>
    </td>
  </tr>
</table>


<h4 id="H7.7.3.3">7.7.3.3 Page objects</h4>


<table>
  <caption id="Table31">Table 31 - Entries in a page object</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Contents</b></td>
    <td>stream or array</td>
    <td>
    <p>(<i>Optional</i>) A content stream (see 7.8.2, "Content streams") that shall describe the contents of this page. If this entry is absent, the page shall be empty.</p>
    <p><span class="new-text">NOTE: if the <b>Contents</b> key is not present, a <b>Resources</b> dictionary must still be present, either directly or through
    inheritance, in the pages tree.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/81" target="_blank">Issue #81</a></span></span></p>
    <p>...</p>
    </td>
  </tr>
</table>


<h3 id="H7.8.3">7.8.3 Resource dictionaries</h3>

<p>...</p>

<ul>
<li>
For a content stream that is the value of a page's <b>Contents</b> entry <span class="deleted-text">(or is an element of an
array that is the value of that entry)<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/9" target="_blank">Issue #9</a></span></span>, the resource dictionary shall
be designated by the page dictionary's <b>Resources</b> entry or is inherited, as described under 7.7.3.4, "Inheritance of page
attributes" from some ancestor node of the page object. ...
</li>
</ul>


<p>...</p>

<h4 id="H7.9.2.2">7.9.2.2 Text string type</h4>

<h5 id="H7.9.2.2.1">7.9.2.2.1 General</h5>

<p>...</p>

<p>EXAMPLE 1 A PDF dictionary containing key ‘Key’ with the value that is the text string "text‰" will look like</p>

<code>
<span class="deleted-text">&lt;&lt;/Key(text?)&gt;&gt;<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/96" target="_blank">Issue #96</a></span></span><br/>
<span class="new-text">&lt;&lt;/Key (text\213) &gt;&gt;<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/96" target="_blank">Issue #96</a></span></span>
</code>

<p>where <span class="deleted-text">the character '?' after the 'text' is represented by the hex code 8B<span class="new-text">h<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/75" target="_blank">Issue #75</a></span></span> (<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/96" target="_blank">Issue #96</a></span></span>octal code 213 <span class="deleted-text">- that<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/96" target="_blank">Issue #96</a></span></span> is according to "D.2 Latin character set and encodings"<span class="deleted-text">)<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/96" target="_blank">Issue #96</a></span></span>.</p>

<p>...</p>

<p>EXAMPLE 2 A PDF dictionary containing key ‘Key’ with the value that is the text string "тест" (that is what the word in Russian with the translation to English as ‘test’) will look like</p>

<code>
<span class="deleted-text">&lt;&lt;/Key(??????????)&gt;&gt;<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/96" target="_blank">Issue #96</a></span></span><br/>
<span class="new-text">&lt;&lt;/Key &lt;FEFF0442043504410442&gt; &gt;&gt;<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/96" target="_blank">Issue #96</a></span></span>
</code>

<p><span class="deleted-text">where the characters in parentheses is the sequence of bytes with hex codes FE, FF, 04, 42, 04, 35, 04, 41, 04, 42.<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/96" target="_blank">Issue #96</a></span></span></p>

<p>...</p>

<p><span class="deleted-text">NOTE 5  It is important not to confuse UTF-16BE with UCS2 (i.e. wchar_t). UTF-16 is not a fixed width encoding scheme.<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/96" target="_blank">Issue #96</a></span></span></p>


<h3 id="H7.10.3">7.10.3 Type 2 (exponential interpolation) functions</h3>


<p>...</p>

<p>Values of <b>Domain</b> shall constrain <i>x</i> in such a way that<span class="new-text">: <span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/30" target="_blank">Issue #30</a></span></span></p>

<ul>
    <li><span class="new-text">if <b>N</b> is not an integer, all values of <i>x</i> will be non-negative; and<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/30" target="_blank">Issue #30</a></span></span></li>
    <li><span class="new-text">if <b>N</b> is negative, no value of <i>x</i> will be zero.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/30" target="_blank">Issue #30</a></span></span></li>
</ul>

<p>Typically, <b>Domain</b> is declared as [0.0 1.0], and <b>N</b> is a positive number. To clip the output to a specified range the <b>Range</b> attribute shall be used.</p>


<p>...</p>


<h3 id="H7.11.6">7.11.6 Collection items</h3>


<table>
  <caption id="Table47">Table 47 - Entries in a collection subitem dictionary</caption>
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
    The type of data shall match the data type identified by the corresponding collection field dictionary. <span class="deleted-text">Default: <i>none</i>.<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/37" target="_blank">Issue #37</a></span></span>
    </p></td>
  </tr>
  <tr>
    <td><b>P</b></td>
    <td>text string</td>
    <td><p>
    (<i>Optional</i>) A prefix string that shall be concatenated with the text string presented to the user. This entry is ignored when an interactive PDF
    processor sorts the items in the collection. <span class="deleted-text">Default: <i>none</i>.<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/37" target="_blank">Issue #37</a></span></span>
    </p></td>
  </tr>
</table>


<h3 id="H7.12.2">7.12.2 Extensions dictionary</h3>

<table>
  <caption id="Table48">Table 48 - Entries in an extensions dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Type</b></td>
    <td>name</td>
    <td>
    (<i>Optional, shall be a direct <span class="deleted-text">objectif<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/109" target="_blank">Issue #109</a></span></span> <span class="new-text">object if<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/109" target="_blank">Issue #109</a></span></span> present</i>) The type of PDF object that this dictionary describes; if present, shall be <i>Extensions</i>.
    </td>
  </tr>
</table>

</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
