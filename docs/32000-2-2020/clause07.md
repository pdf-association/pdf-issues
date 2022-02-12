---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 7
title: Syntax
modified: 4 February 2022
---

<ul class="noprint">
  <li>7.3 Objects
   <ul>
    <li>7.3.4 String objects
     <ul>
      <li><a href="#H7.3.4.2">7.3.4.2 Literal strings</a>
      </li>
     </ul>
    </li>
    <li>7.3.8 Stream objects
     <ul>
      <li><a href="#H7.3.8.2">7.3.8.2 Stream extent</a>
      </li>
     </ul>
    </li>
   </ul>
  </li>
  <li>7.4 Filters
   <ul>
    <li><a href="#H7.4.3">7.4.3 ASCII85Decode filter</a>
    </li>
    <li><a href="#H7.4.9">7.4.9 JPXDecode filter</a>
    </li>
   </ul>
  </li>
  <li><a href="#H7.5">7.5 File structure</a>
   <ul>
    <li><a href="#H7.5.4">7.5.4 Cross reference table</a>
    </li>
    <li><a href="#H7.5.7">7.5.7 Object streams</a>
    </li>
    <li>7.5.8 Cross-reference streams</a>
     <ul>
      <li><a href="#H7.5.8.4">7.5.8.4 Compatibility with applications that do not support compressed reference streams</a>
      </li>
     </ul>
    </li>
   </ul>
  </li>
  <li>7.6 Encryption
   <ul>
    <li>7.6.3 General encryption algorithm
     <ul>
      <li><a href="#H7.6.3.1">7.6.3.1 General</a>
      </li>
     </ul>
    </li>
    <li>7.6.4 Standard security handler
     <ul>
      <li><a href="#H7.6.4.1">7.6.4.1 General</a>
       <ul>
        <li><a href="#H7.6.4.3.2">7.6.4.3.2 Algorithm 2: Computing a file encryption key in order to encrypt a document (revision 4 and earlier)</a>
        </li>
        <li><a href="#H7.6.4.3.3">7.6.4.3.3 Algorithm 2.A: Retrieving the file encryption key from an encrypted document in order to decrypt it (revision 6 and later)</a>
        </li>
        <li><a href="#H7.6.4.4.9">7.6.4.4.9 Algorithm 10: Computing the encryption dictionary's Perms (permissions) value (Security handlers of revision 6)</a>
        </li>
        <li><a href="#H7.6.4.4.12">7.6.4.4.12 Algorithm 13: Validating the permissions (Security handlers of revision 6)</a>
        </li>
       </ul>
      </li>
     </ul>
    </li>
    <li>7.6.5 Public-key security handlers
     <ul>
      <li><a href="#H7.6.5.3">7.6.5.3 Public-key encryption algorithms</a>
      </li>
     </ul>
    </li>
    <li><a href="#H7.6.6">7.6.6 Crypt filters</a>
    </li>
   </ul>
  </li>
  <li>7.7 Document structure
   <ul>
    <li><a href="#H7.7.2">7.7.2 Document catalog dictionary</a>
    </li>
    <li>7.7.3 Page tree
     <ul>
      <li><a href="#H7.7.3.3">7.7.3.3 Page objects</a>
      </li>
     </ul>
    </li>
   </ul>
  </li>
  <li>7.8 Content streams and resources
   <ul>
    <li><a href="#H7.8.3">7.8.3 Resource dictionaries</a>
    </li>
   </ul>
  </li>
  <li>7.9 Common data structures
   <ul>
    <li>7.9.2 String object types
     <ul>
      <li>7.9.2.2 Text string type
       <ul>
        <li><a href="#H7.9.2.2.1">7.9.2.2.1 General</a>
        </li>
       </ul>
      </li>
     </ul>
    </li>
   </ul>
  </li>
  <li>7.10 Functions
   <ul>
    <li><a href="#H7.10.3">7.10.3 Type 2 (exponential interpolation) functions</a>
    </li>
   </ul>
  </li>
  <li>7.11 File specifications
   <ul>
    <li><a href="#H7.11.6">7.11.6 Collection items</a>
    </li>
   </ul>
  </li>
  <li>7.12 Extensions dictionary
   <ul>
    <li><a href="#H7.12.2">7.12.2 Extensions dictionary</a>
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

<h2 id="H7.3">7.3 Objects</h2>

<h3 id="H7.3".4>7.3.4 String objects</h3>

<h4 id="H7.3.4.2">7.3.4.2 Literal strings</h4>

<p>A <i>literal string</i> shall be written as an arbitrary number of characters enclosed in parentheses (LEFT PAREN<ins onMouseEnter="mouseEnter(this)" data-issue="143">T</ins>HESIS (28h) and RIGHT PARENTHESIS (29h)). Any characters may appear in a string except unbalanced parentheses and the backslash (REVERSE SOLIDUS (5Ch)), which shall be treated specially as described in this subclause. Balanced pairs of parentheses within a string require no special treatment.
</p>

<p>...</p>

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
    shall be ignored. However, the <b>Length</b> entry <del onMouseEnter="mouseEnter(this)" data-issue="10">should</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="10">shall</ins> still specify the
    number of those bytes (usually, there are no bytes and <b>Length</b> is 0). The filters that are applied to the file data shall be specified by
    <b>FFilter</b> and the filter parameters shall be specified by <b>FDecodeParms</b>.
    </p></td>
  </tr>
</table>

<h3 id="H7.4.3">7.4.3 ASCII85Decode filter</h3>

<p>...</p>

<p>The following conditions shall never occur in a correctly encoded byte sequence:</p>
<ul>
    <li>The value represented by a group of 5 characters is greater than <del onMouseEnter="mouseEnter(this)" data-issue="98">232</del><ins onMouseEnter="mouseEnter(this)" data-issue="98">2<sup>32</sup></ins> - 1.</li>
    <li>A <i>z</i> character occurs in the middle of a group.</li>
    <li>A final partial group contains only one character.</li>
</ul>

<h3 id="H7.4.9">7.4.9 JPXDecode filter</h3>

<p>...</p>

<p>
Data used in PDF image XObjects shall be limited to the JPX baseline set of features,
<del onMouseEnter="mouseEnter(this)" data-issue="29">except for</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="29">excluding</ins>
enumerated colour space 19 (CIEJab).
In addition, enumerated colour space 12 (CMYK), which is part of JPX but not JPX baseline, shall be supported in a PDF file. JPX file
structures used in PDF files shall conform to the JPEG 2000 specification.
</p>

<p>...</p>

<h2 id="H7.5">7.5 File structure</h2>

<p>
The trailer of a PDF file enables a PDF processor to quickly find the cross-reference table and certain
special objects. PDF processors should read a PDF file from its end. The last line of the file shall contain
only the end-of-file marker, %%EOF. The two preceding lines shall contain, one per line and in order,
the keyword <b>startxref</b> and the byte offset
<del onMouseEnter="mouseEnter(this)" data-issue="101">in the decoded stream</del> from the beginning of the PDF file to
the beginning of the <b>xref</b> keyword in the last cross-reference section
<ins onMouseEnter="mouseEnter(this)" data-issue="101">or the beginning of the previous cross-reference streams
(see 7.5.8, "Cross-reference streams")</ins>. The <b>startxref</b> line shall be
preceded by the trailer dictionary, consisting of the keyword trailer followed by a series of key-value
pairs enclosed in double angle brackets (&lt;&lt;...&gt;&gt;) (using LESS-THAN SIGNs (3Ch) and GREATER-THAN
SIGNs (3Eh)). Thus, the trailer has the following overall structure:
</p>

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
    <del onMouseEnter="mouseEnter(this)" data-issue="101">stream</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="101">section</ins>.
    </p></td>
  </tr>
</table>

<h3 id="H7.5.4">7.5.4 Cross reference table</h3>

<p>...</p>

<p class="hangingindent">
NOTE 3 The subsection structure is useful for incremental updates, since it allows a new cross-reference section to be added to the PDF file, containing entries only for objects that have been added, modified or deleted. <del onMouseEnter="mouseEnter(this)" data-issue="147">This also means that cross reference subsections of incremental updates can never have an object number of zero.</del>
<p>

<p>
Each cross-reference subsection shall contain entries for a contiguous range of object numbers.
<del onMouseEnter="mouseEnter(this)" data-issue="113">Each cross-reference subsection shall contain entries for a contiguous range of object numbers.</del>
The subsection shall begin with a line containing only two <ins onMouseEnter="mouseEnter(this)" data-issue="147">non-negative</ins> integers separated by a single SPACE (20h) and terminated by an end-of-line marker (see 7.2.3, "Character set"). The two <ins onMouseEnter="mouseEnter(this)" data-issue="147">non-negative</ins> integers denote (respectively) the object number of the first object in this subsection and the number of entries in the subsection.
</p>

<p>...</p>

<p><ins onMouseEnter="mouseEnter(this)" data-issue="109">EXAMPLE 2 The cross-reference table sub-section line requires a single SPACE between "0" and "6".</ins></p>

<p><ins onMouseEnter="mouseEnter(this)" data-issue="109">EXAMPLE 3 The cross-reference table first sub-section line requires a single SPACE between "0" and "1". The typeface of this example should be all monospaced and with single SPACEs between all cross-reference fields, and thus all fields vertically aligned.</ins></p>


<h3 id="H7.5.7">7.5.7 Object streams</h3>

<p>...</p>


<p>The following objects shall not be stored in an object stream:</p>

<ul>
  <li>...</li>
</ul>

<p>
<ins onMouseEnter="mouseEnter(this)" data-issue="114">Any entry's value in an <b>ObjStm</b> dictionary shall be either a direct object or an indirect uncompressed object.</ins>
</p>

<p class="hangingindent">
NOTE 3 Indirect references to objects inside object streams use the normal syntax: for example, 14 0 R. Access to these objects requires a different way of storing cross-reference information; see 7.5.8, "Cross-reference streams". Use of compressed objects requires a PDF 1.5 PDF reader. However, compressed objects can be stored in a manner that a PDF 1.4 PDF reader can ignore.
</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="110">NOTE 4: Including the document catalog in an object stream has interoperability implications, particularly for encrypted documents. If the catalog dictionary is part of an object stream, a PDF processor reading the document must first process that object stream before it can access potentially relevant document metadata, including the declared PDF version, developer extensions and XMP metadata.</ins>
</p>

<p>...</p>

<h3 id="H7.5.8">7.5.8 Cross-reference streams</h3>

<h4 id="H7.5.8.4">7.5.8.4 Compatibility with applications that do not support compressed reference streams</h4>

<p>...</p>

<table>
  <caption id="Table19">Table 19 - Additional entries in a hybrid-reference file’s trailer dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>XRefStm</b></td>
    <td>integer</td>
    <td><p>
    (<i>Optional</i>) The byte offset
    <del onMouseEnter="mouseEnter(this)" data-issue="146">in the decoded stream from the beginning of the PDF file of a cross-reference stream.</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="146">to the cross-reference stream, calculated from the beginning of the PDF file.</ins>.
    </p></td>
  </tr>
</table>

<p>...</p>

<h3 id="H7.6.3">7.6.3 General encryption algorithm</h3>

<h4 id="H7.6.3.1">7.6.3.1 General</h4>

<p>...</p>

<p class="hangingindent">NOTE 1 The name RC4&trade; is a registered trademark of RSA Security Inc. and cannot be used by third parties creating implementations of the algorithm. Proprietary implementations of the RC4 encryption algorithm are available under license from RSA Security Inc. For licensing information, contact: <del onMouseEnter="mouseEnter(this)" data-issue="95">RSA Security Inc. 2955 Campus Drive, Suite 400, San Mateo, CA 94403-2507, USA, or</del> <a href="http://www.rsasecurity.com/">http://www.rsasecurity.com/</a>.</p>

<p>...</p>

<h3 id="H7.6.4">7.6.4 Standard security handler</h3>

<h4 id="H7.6.4.1">7.6.4.1 General</h4>

<p>...</p>

<p>
If a security handler of revision 4 or 5 is specified, the standard security handler shall support crypt filters (see 7.6.6, "Crypt filters").
The support shall be limited to the <b>Identity</b> crypt filter (see "Table 26 - Standard crypt filter names") and
<del onMouseEnter="mouseEnter(this)" data-issue="89">crypt filters</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="89">a crypt filter</ins>
named <b>StdCF</b> whose dictionaries contain an <b>AuthEvent</b> value of <i>DocOpen</i>. For revision 4, the filter <b>CFM</b> value shall be <i>V2</i> (RC4) or <i>AESV2</i> (AES-128). For revision 6, the filter <b>CFM</b> value shall be <i>AESV3</i> (AES-256). Public-Key security handlers in this case shall use
<del onMouseEnter="mouseEnter(this)" data-issue="89">crypt filters</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="89">a crypt filter</ins>
named <b>DefaultCryptFilter</b> when all document content is encrypted, and shall use
<del onMouseEnter="mouseEnter(this)" data-issue="89">crypt filters</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="89">a crypt filter</ins>
named <b>DefEmbeddedFile</b> when file attachments only are encrypted in place of <b>StdCF</b> name. This nomenclature shall not be used as an indicator of the type of the security handler or encryption. Use of security handler revisions 1, 2, 3, 4 and 5 is deprecated in PDF 2.0.
</p>

<p>...</p>

<h5 id="H7.6.4.3.2">7.6.4.3.2 Algorithm 2: Computing a file encryption key in order to encrypt a document (revision 4 and earlier)</h5>

<p>...</p>

<p class="hangingindent">NOTE 2  The first element of the ID array, as used in 7.6.4.3.2, "Algorithm 2: Computing a file encryption key in order to encrypt a document (revision 4 and earlier)", step e, generally remains unchanged across revisions of a given document. However, since this is not guaranteed, use of the ID in computation of the file encryption key, as required when using <del onMouseEnter="mouseEnter(this)" data-issue="53">7.6.4.3.3, "Algorithm 2.A: Retrieving the file encryption key from an encrypted document in order to decrypt it (revision 6 and later)Algorithm 2: Computing a file encryption key in order to encrypt a document (revision 4 and earlier)"</del> <ins onMouseEnter="mouseEnter(this)" data-issue="53">7.6.4.3.2, "Algorithm 2: Computing a file encryption key in order to encrypt a document (revision 4 and earlier)"</ins>, can complicate updates to the document. For this reason, security handlers are encouraged to use Algorithm 2.A or higher, which do not use the ID in file encryption key computation. <del onMouseEnter="mouseEnter(this)" data-issue="53">This algorithm, when applied to the user password string, produces the file encryption key used to encrypt or decrypt string and stream data according to 7.6.3.2, "Algorithm 1: Encryption of data using the RC4 or AES algorithms". Parts of this algorithm are also used in the algorithms described below.</del>
</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="53">NOTE 3  This algorithm, when applied to the user password string, produces the file encryption key used to encrypt or decrypt string and stream data according to 7.6.3.2, "Algorithm 1: Encryption of data using the RC4 or AES algorithms". Parts of this algorithm are also used in the algorithms described in 7.6.4.4, "Password algorithms".</ins>
</p>

<h5 id="H7.6.4.3.3">7.6.4.3.3 Algorithm 2.A: Retrieving the file encryption key from an encrypted document in order to decrypt it (revision 6 and later)</h5>

<p>...</p>


<ol type="a" start="6">
<li>
Decrypt the 16-byte <b>Perms</b> string using AES-256 in ECB mode <del onMouseEnter="mouseEnter(this)" data-issue="24">with an initialization vector of zero</del>
and the file encryption key as the key. ...
</li>
</ol>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="53">NOTE This algorithm, when applied to the user password string, produces the file encryption key used to encrypt or decrypt string and stream data according to 7.6.3.3, "Algorithm 1.A: Encryption of data using the AES algorithms". Parts of this algorithm are also used in the algorithms described in 7.6.4.4, "Password algorithms".</ins>
</p>

<h5 id="H7.6.4.4.9">7.6.4.4.9 Algorithm 10: Computing the encryption dictionary's Perms (permissions) value (Security handlers of revision 6)</h5>

<ol type="a" start="6">
<li>
Encrypt the 16-byte block using AES-256 in ECB mode <del onMouseEnter="mouseEnter(this)" data-issue="24">with an initialization vector of zero</del>,
using the file encryption key as the key. The result (16 bytes) is stored as the <b>Perms</b> string, and checked for validity when the file is opened.
</li>
</ol>

<h5 id="H7.6.4.4.12">7.6.4.4.12 Algorithm 13: Validating the permissions (Security handlers of revision 6)</h5>

<ol type="a" start="1">
<li>
Decrypt the 16 byte <b>Perms</b> string using AES-256 in ECB mode <del onMouseEnter="mouseEnter(this)" data-issue="24">with an initialization vector of zero</del>
and the file encryption key as the key. ...
</li>
</ol>

<h4 id="H7.6.5.3">7.6.5.3 Public-key encryption algorithms</h4>

<p><i>New notes added at the end of sub-clause 7.6.5.3:</i></p>

<ins onMouseEnter="mouseEnter(this)" data-issue="25">
<p class="hangingindent">NOTE 1: This means that step c) only applies when both of the following conditions are met:</p>

<ul>
<li>the key is being generated for the crypt filter named <i>DefaultCryptFilter</i> (i.e. the crypt filter used as the value for <b>StmF</b> in the encryption dictionary);</li>
<li>the <b>EncryptMetadata</b> entry of the associated crypt filter dictionary is set to <i>false</i>.</li>
</ul>

<p class="hangingindent">
NOTE 2: Since crypt filters are not supported when <b>SubFilter</b> is set to <i>adbe.pkcs7.s3</i> or <i>adbe.pkcs7.s4</i> in the encryption dictionary,
there is no way to specify that metadata is to be left unencrypted in these cases. In particular, step c) is always skipped for these <b>SubFilter</b> values.
</p>
</ins>


<h3 id="H7.6.6">7.6.6 Crypt filters</h3>

<p>PDF 1.5 introduces crypt filters, which provide finer granularity control of encryption within a PDF file. The use of crypt filters involves the following structures:</p>

<ul>
  <li>The encryption dictionary (see "Table 20 - Entries common to all encryption dictionaries") contains entries that enumerate the crypt filters in the document (<b>CF</b>) and specify which ones are used by default to decrypt all the streams (<b>StmF</b>) and strings (<b>StrF</b>) in the document. In addition, the value of the V entry shall be 4 <ins onMouseEnter="mouseEnter(this)" data-issue="74">or 5</ins> to use crypt filters.
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
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="16">byte</ins> string or array</td>
    <td>
    <p>(<i>Required</i>) If the crypt filter is referenced from <b>StmF</b> or <b>StrF</b> in the encryption dictionary, this entry shall be an array of byte strings,
    where each <ins onMouseEnter="mouseEnter(this)" data-issue="16">byte</ins> string shall be a binary-encoded CMS object that shall ...</p>
    <p>...</p>
    <p>If the crypt filter is referenced from a <b>Crypt</b> filter decode parameter dictionary (see "Table 14 - Optional parameters for Crypt filters"),
    this entry shall be a <ins onMouseEnter="mouseEnter(this)" data-issue="16">byte</ins> string that shall be a binary-encoded CMS object that shall ...</p>
    </td>
  </tr>
</table>

<h2 id="H7.7">7.7 Document structure</h2>

<h3 id="H7.7.2">7.7.2 Document catalog dictionary</h3>

<table>
  <caption id="Table29">Table 29 - Entries in the catalog dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Lang</b></td>
    <td>text string</td>
    <td>
    <p>(<i>Optional; PDF 1.4</i>) A language identifier that shall specify the natural language for all text in the document except where overridden by language specifications for structure elements or marked-content (see 14.9.2, "Natural language specification"). If this entry is absent
    <ins onMouseEnter="mouseEnter(this)" data-issue="105"> or invalid (see 14.9.2, "Natural language specification")</ins>, the language shall be considered unknown.
    </p><ins onMouseEnter="mouseEnter(this)" data-issue="135">NOTE All text in a document includes PDF text strings (see 7.9.2.2 "Text string type") as well as textual content.</ins><p>
    </p>
    </td>
  </tr>
</table>

<h3 id="H7.7.3">7.7.3 Page tree</h3>

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
    <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="81">NOTE: if the <b>Contents</b> key is not present, a <b>Resources</b> dictionary must still be present, either directly or through inheritance, in the pages tree.</ins></p>
    <p>...</p>
    </td>
  </tr>
</table>


<h3 id="H7.8.3">7.8.3 Resource dictionaries</h3>

<p>...</p>

<ul>
<li>
For a content stream that is the value of a page's <b>Contents</b> entry
<del onMouseEnter="mouseEnter(this)" data-issue="9">(or is an element of an array that is the value of that entry)</del>, the resource dictionary shall
be designated by the page dictionary's <b>Resources</b> entry or is inherited, as described under 7.7.3.4, "Inheritance of page
attributes" from some ancestor node of the page object. ...
</li>
</ul>


<p>...</p>

<h4 id="H7.9.2.2">7.9.2.2 Text string type</h4>

<h5 id="H7.9.2.2.1">7.9.2.2.1 General</h5>

<p>...</p>

<p>EXAMPLE 1 A PDF dictionary containing key 'Key' with the value that is the text string "text&permil;" will look like</p>

<code>
 <del onMouseEnter="mouseEnter(this)" data-issue="96">&lt;&lt;/Key(text?)&gt;&gt;</del>
 <ins onMouseEnter="mouseEnter(this)" data-issue="96">&lt;&lt;/Key (text\213) &gt;&gt;</ins>
</code>

<p>where <del onMouseEnter="mouseEnter(this)" data-issue="96">the character '?' after the 'text' is represented by the hex code 8Bh (</del>octal code 213 <del onMouseEnter="mouseEnter(this)" data-issue="96">- that</del> is according to "D.2 Latin character set and encodings".</p>

<p>...</p>

<p>EXAMPLE 2 A PDF dictionary containing key 'Key' with the value that is the text string "&#x442;&#x435;&#x441;&#x442;" (that is what the word in Russian with the translation to English as 'test') will look like</p>

<code>
 <del onMouseEnter="mouseEnter(this)" data-issue="96">&lt;&lt;/Key(??????????)&gt;&gt;</del>
 <ins onMouseEnter="mouseEnter(this)" data-issue="96">&lt;&lt;/Key &lt;FEFF0442043504410442&gt; &gt;&gt;</ins>
</code>

<p><del onMouseEnter="mouseEnter(this)" data-issue="96">where the characters in parentheses is the sequence of bytes with hex codes FE, FF, 04, 42, 04, 35, 04, 41, 04, 42.</del></p>

<p>...</p>

<p class="hangingindent"><del onMouseEnter="mouseEnter(this)" data-issue="96">NOTE 5  It is important not to confuse UTF-16BE with UCS2 (i.e. wchar_t). UTF-16 is not a fixed width encoding scheme.</del></p>


<h3 id="H7.10.3">7.10.3 Type 2 (exponential interpolation) functions</h3>


<p>...</p>

<p>Values of <b>Domain</b> shall constrain <i>x</i> in such a way that<ins onMouseEnter="mouseEnter(this)" data-issue="30">: </ins></p>

<ul>
    <li><ins onMouseEnter="mouseEnter(this)" data-issue="30">if <b>N</b> is not an integer, all values of <i>x</i> will be non-negative; and</ins></li>
    <li><ins onMouseEnter="mouseEnter(this)" data-issue="30">if <b>N</b> is negative, no value of <i>x</i> will be zero.</ins></li>
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
    The type of data shall match the data type identified by the corresponding collection field dictionary. <del onMouseEnter="mouseEnter(this)" data-issue="37">Default: <i>none</i>.</del>
    </p></td>
  </tr>
  <tr>
    <td><b>P</b></td>
    <td>text string</td>
    <td><p>
    (<i>Optional</i>) A prefix string that shall be concatenated with the text string presented to the user. This entry is ignored when an interactive PDF
    processor sorts the items in the collection. <del onMouseEnter="mouseEnter(this)" data-issue="37">Default: <i>none</i>.</del>
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
    (<i>Optional, shall be a direct <del onMouseEnter="mouseEnter(this)" data-issue="109">objectif</del> <ins onMouseEnter="mouseEnter(this)" data-issue="109">object if</ins> present</i>) The type of PDF object that this dictionary describes; if present, shall be <i>Extensions</i>.
    </td>
  </tr>
</table>

</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
