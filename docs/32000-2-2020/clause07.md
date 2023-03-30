---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 7
title: Syntax
modified: 13 March 2023
---

<ul class="noprint">
  <li>7.2 Lexical conventions
   <ul>
   <li><a href="#H7.2.2">7.2.2 Representation</a>
   </li>
   </ul>
  </li>
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
    <li><a href="#H7.5.5">7.5.5 File trailer</a>
    </li>
    <li><a href="#H7.5.7">7.5.7 Object streams</a>
    </li>
    <li>7.5.8 Cross-reference streams
     <ul>
      <li><a href="#H7.5.8.2">7.5.8.2 Cross-reference stream dictionary</a>
      </li>
      <li><a href="#H7.5.8.4">7.5.8.4 Compatibility with applications that do not support compressed reference streams</a>
      </li>
     </ul>
    </li>
   </ul>
  </li>
  <li>7.6 Encryption
   <ul>
    <li><a href="#H7.6.2">7.6.2 Application of encryption</a>
    </li>
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
      <li>7.6.5.1 General
      </li>
      <li><a href="#H7.6.5.2">7.6.5.2 Public-key encryption dictionary</a>
      </li>
      <li><a href="#H7.6.5.3"><ins onMouseEnter="mouseEnter(this)" data-issue="196" data-iso="submitted">7.6.5.3 Public-key encryption permissions</ins></a>
      </li>
      <li><a href="#H7.6.5.4"><del onMouseEnter="mouseEnter(this)" data-issue="196" data-iso="submitted">7.6.5.3</del><ins onMouseEnter="mouseEnter(this)" data-issue="196" data-iso="submitted">7.6.5.4</ins> Public-key encryption algorithms</a>
      </li>
     </ul>
    </li>
    <li><a href="#H7.6.6">7.6.6 Crypt filters</a>
    </li>
   </ul>
  </li>
  <li>7.7 Document structure
   <ul>
    <li><a href="#H7.7.1">7.7.1 General</a>
    </li>
    <li><a href="#H7.7.2">7.7.2 Document catalog dictionary</a>
    </li>
    <li>7.7.3 Page tree
     <ul>
      <li><a href="#H7.7.3.3">7.7.3.3 Page objects</a>
      </li>
     </ul>
    </li>
    <li><a href="#H7.7.4">7.7.4 Name dictionary</a>
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
    <li><a href="#H7.9.6">7.9.6 Name trees</a>
    </li>
   </ul>
  </li>
  <li>7.10 Functions
   <ul>
    <li><a href="#H7.10.3">7.10.3 Type 2 (exponential interpolation) functions</a>
    </li>
    <li>7.10.5 Type 4 (PostScript calculator) functions
     <ul>
      <li><a href="#H7.10.5.2">7.10.5.2 Operators and operands</a>
      </li>
     </ul>
    </li>
   </ul>
  </li>
  <li>7.11 File specifications
   <ul>
    <li>7.11.4 Embedded file streams
     <ul>
      <li><a href="#H7.11.4.1">7.11.4.1 General</a>
      </li>
     </ul>
    </li>
    <li><a href="#H7.11.6">7.11.6 Collection items</a>
    </li>
   </ul>
  </li>
  <li>7.12 Extensions dictionary
   <ul>
    <li><a href="#H7.12.2">7.12.2 Extensions dictionary</a>
    </li>
    <li><a href="#H7.12.5">7.12.5 ExtensionLevel</a>
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

<h2 id="H7.2">7.2 Lexical conventions</h2>

<h3 id="H7.2.2">7.2.2 Representation</h3>

<p class="location">Change the first paragraph and the 3rd (last) bullet in the subsequent list as follows:</p>

<p>
<del onMouseEnter="mouseEnter(this)" data-issue="193" data-iso="submitted">A non-encrypted PDF file can be entirely represented using byte values corresponding to the visible
printable subset of the ASCII character set defined in INCITS 4-1986 (R2017), plus white-space characters.
However, a</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="193" data-iso="submitted">A</ins> PDF file is not restricted to the ASCII character set; it may contain arbitrary bytes, subject to the following considerations:
</p>

<ul>
 <li>...</li>
 <li>...</li>
 <li>A PDF file <del onMouseEnter="mouseEnter(this)" data-issue="193" data-iso="submitted">containing binary data</del> shall be transported as a binary file rather than as a text file to ensure that all bytes of the file are faithfully preserved.</li>
</ul>

<p>...</p>

<h2 id="H7.3">7.3 Objects</h2>

<h3 id="H7.3.4">7.3.4 String objects</h3>

<h4 id="H7.3.4.2">7.3.4.2 Literal strings</h4>

<p class="location">Change first paragraph as follows:</p>

<p>A <i>literal string</i> shall be written as an arbitrary number of characters enclosed in parentheses (LEFT PAREN<ins onMouseEnter="mouseEnter(this)" data-issue="143" data-iso="approved">T</ins>HESIS (28h) and RIGHT PARENTHESIS (29h)). Any characters may appear in a string except unbalanced parentheses and the backslash (REVERSE SOLIDUS (5Ch)), which shall be treated specially as described in this subclause. Balanced pairs of parentheses within a string require no special treatment.
</p>

<p>...</p>

<h4 id="H7.3.8.2">7.3.8.2 Stream extent</h4>

<p class="location">Change Table 5 as follows:</p>

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
    shall be ignored. However, the <b>Length</b> entry <del onMouseEnter="mouseEnter(this)" data-issue="10" data-iso="approved">should</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="10" data-iso="approved">shall</ins> still specify the
    number of those bytes (usually, there are no bytes and <b>Length</b> is 0). The filters that are applied to the file data shall be specified by
    <b>FFilter</b> and the filter parameters shall be specified by <b>FDecodeParms</b>.
    </p></td>
  </tr>
</table>

<h3 id="H7.4.3">7.4.3 ASCII85Decode filter</h3>

<p class="location">Change last bulleted list follows:</p>

<p>The following conditions shall never occur in a correctly encoded byte sequence:</p>
<ul>
    <li>The value represented by a group of 5 characters is greater than <del onMouseEnter="mouseEnter(this)" data-issue="98" data-iso="approved">232</del><ins onMouseEnter="mouseEnter(this)" data-issue="98" data-iso="approved">2<sup>32</sup></ins> - 1.</li>
    <li>A <i>z</i> character occurs in the middle of a group.</li>
    <li>A final partial group contains only one character.</li>
</ul>

<h3 id="H7.4.9">7.4.9 JPXDecode filter</h3>

<p class="location">Change paragraph below NOTE 5 as follows:</p>

<p>
Data used in PDF image XObjects shall be limited to the JPX baseline set of features,
<del onMouseEnter="mouseEnter(this)" data-issue="29" data-iso="approved">except for</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="29" data-iso="approved">excluding</ins>
enumerated colour space 19 (CIEJab).
In addition, enumerated colour space 12 (CMYK), which is part of JPX but not JPX baseline, shall be supported in a PDF file. JPX file
structures used in PDF files shall conform to the JPEG 2000 specification.
</p>

<p>...</p>

<h2 id="H7.5">7.5 File structure</h2>

<h3 id="H7.5.4">7.5.4 Cross reference table</h3>

<p class="location">Change NOTE 3 as follows:</p>

<p class="hangingindent">
NOTE 3 The subsection structure is useful for incremental updates, since it allows a new cross-reference section to be added to the PDF file, containing entries only for objects that have been added, modified or deleted. <del onMouseEnter="mouseEnter(this)" data-issue="147" data-iso="submitted">This also means that cross reference subsections of incremental updates can never have an object number of zero.</del>
</p>

<p class="location">Change paragraph below NOTE 3 as follows:</p>

<p>
Each cross-reference subsection shall contain entries for a contiguous range of object numbers.
<del onMouseEnter="mouseEnter(this)" data-issue="113" data-iso="approved">Each cross-reference subsection shall contain entries for a contiguous range of object numbers.</del>
The subsection shall begin with a line containing only two <ins onMouseEnter="mouseEnter(this)" data-issue="147" data-iso="submitted">non-negative</ins> integers separated by a single SPACE (20h) and terminated by an end-of-line marker (see 7.2.3, "Character set"). The two <ins onMouseEnter="mouseEnter(this)" data-issue="147" data-iso="submitted">non-negative</ins> integers denote (respectively) the object number of the first object in this subsection and the number of entries in the subsection.
</p>

<p class="location">Change various paragraphs below EXAMPLE 1 as follows:</p>

<p>...</p>
<p>where:</p>

<p><i>nnnnnnnnnn</i> shall be a 10-digit byte offset in the <del onMouseEnter="mouseEnter(this)" data-issue="101" data-iso="approved">decoded stream</del> <ins onMouseEnter="mouseEnter(this)" data-issue="101" data-iso="approved">PDF file</ins></p>

<p>...</p>

<p>The byte offset in the <del onMouseEnter="mouseEnter(this)" data-issue="101" data-iso="approved">decoded stream</del> <ins onMouseEnter="mouseEnter(this)" data-issue="101" data-iso="approved">PDF file</ins> shall be a 10-digit number, padded with leading zeros if necessary, giving the number of bytes from the beginning of the PDF file to the beginning of the object. ... </p>

<p class="location">Change EXAMPLE 2 as follows:</p>

<p><ins onMouseEnter="mouseEnter(this)" data-issue="109" data-iso="approved">EXAMPLE 2 The cross-reference table sub-section line requires a single SPACE between "0" and "6".</ins></p>

<p class="location">Change EXAMPLE 3 as follows:</p>

<p><ins onMouseEnter="mouseEnter(this)" data-issue="109" data-iso="approved">EXAMPLE 3 The cross-reference table first sub-section line requires a single SPACE between "0" and "1".</ins></p>
<p class="editornote">EDITOR NOTE: The typeface of Example 3 should be all monospaced and with single SPACEs between all cross-reference fields, and thus all cross-reference data fields vertically aligned.</p>


<h3 id="H7.5.5">7.5.5 File trailer</h3>

<p class="location">Change first paragraph as follows:</p>

<p>
The trailer of a PDF file enables a PDF processor to quickly find the cross-reference table and certain
special objects. PDF processors should read a PDF file from its end. The last line of the file shall contain
only the end-of-file marker, %%EOF. The two preceding lines shall contain, one per line and in order,
the keyword <b>startxref</b> and the byte offset
<del onMouseEnter="mouseEnter(this)" data-issue="101" data-iso="approved">in the decoded stream</del> from the beginning of the PDF file to
the beginning of the <b>xref</b> keyword in the last cross-reference section
<ins onMouseEnter="mouseEnter(this)" data-issue="101" data-iso="approved">or the beginning of the previous cross-reference stream
(see 7.5.8, "Cross-reference streams")</ins>. The <b>startxref</b> line shall be
preceded by the trailer dictionary, consisting of the keyword trailer followed by a series of key-value
pairs enclosed in double angle brackets (&lt;&lt;...&gt;&gt;) (using LESS-THAN SIGNs (3Ch) and GREATER-THAN
SIGNs (3Eh)). Thus, the trailer has the following overall structure:
</p>

<p class="location">Change Table 15 as follows:</p>

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
    <del onMouseEnter="mouseEnter(this)" data-issue="101" data-iso="approved">stream</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="101" data-iso="approved">section</ins>.
    </p></td>
  </tr>
  <tr>
    <td><b>Info</b></td>
    <td>dictionary</td>
    <td><p>
    (<i>Optional<del onMouseEnter="mouseEnter(this)" data-issue="106" data-iso="submitted">; shall be an indirect reference</del></i>) ...
    </p></td>
  </tr>
</table>

<h3 id="H7.5.7">7.5.7 Object streams</h3>

<p class="location">Append the following paragraph after the bulleted list as follows:</p>

<p>The following objects shall not be stored in an object stream:</p>

<ul>
  <li>...</li>
</ul>

<p>
<ins onMouseEnter="mouseEnter(this)" data-issue="114" data-iso="approved">Any entry's value in an <b>ObjStm</b> dictionary shall be either a direct object or an indirect uncompressed object.</ins>
</p>

<p class="hangingindent">
NOTE 3 Indirect references to objects inside object streams use the normal syntax: for example, 14 0 R. Access to these objects requires a different way of storing cross-reference information; see 7.5.8, "Cross-reference streams". Use of compressed objects requires a PDF 1.5 PDF reader. However, compressed objects can be stored in a manner that a PDF 1.4 PDF reader can ignore.
</p>

<p class="location">Insert the following new NOTE 4 after NOTE 3 as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="110" data-iso="approved">NOTE 4: Including the document catalog in an object stream has interoperability implications, particularly for encrypted documents. If the catalog dictionary is part of an object stream, a PDF processor reading the document must first process that object stream before it can access potentially relevant document metadata, including the declared PDF version, developer extensions and XMP metadata.</ins>
</p>

<p>...</p>

<h3 id="H7.5.8">7.5.8 Cross-reference streams</h3>

<h4 id="H7.5.8.2">7.5.8.2 Cross-reference stream dictionary</h4>

<p>...</p>

<p class="location">Change the first bullet point as follows:</p>
<ul>
<li>
The values of all entries shown in "Table 17 - Additional entries specific to a cross-reference
stream dictionary" shall be direct objects; indirect references shall not be permitted. For arrays
(the <b>Index</b> and <b>W</b> entries), all of their elements shall be direct objects as well. 
<del onMouseEnter="mouseEnter(this)" data-issue="246">If the stream is encoded, the <b>Filter</b> and <b>DecodeParms</b> 
entries in "Table 5 - Entries common to all stream dictionaries" shall also be direct objects.</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="246">The values of all entries shown in "Table 5 - Entries common to 
all stream dictionaries" shall also be direct objects. For arrays, all array elements shall be direct objects and for 
dictionaries, all key values shall be direct objects as well. The <b>F</b> entry defined in Table 5 shall not be used.</ins> 
</li>
<li>...</li>
</ul>


<h4 id="H7.5.8.4">7.5.8.4 Compatibility with applications that do not support compressed reference streams</h4>

<p class="location">Change Table 19 as follows:</p>

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
    <del onMouseEnter="mouseEnter(this)" data-issue="146" data-iso="submitted">in the decoded stream from the beginning of the PDF file of a cross-reference stream.</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="146" data-iso="submitted">to the cross-reference stream, calculated from the beginning of the PDF file.</ins>
    </p></td>
  </tr>
</table>

<p>...</p>

<h3 id="H7.6.2">7.6.2 Application of encryption</h3>

<h3 id="H7.6.3">7.6.3 General encryption algorithm</h3>

<p class="location">Add new NOTE 1 after the 4th bullet in the first bulleted list below the first paragraph as follows:</p>

<p>Encryption applies to all strings and streams in the document's PDF file, with the following exceptions:</p>

<ul>
<li>...</li>
<li>Any hexadecimal strings representing the value of the Contents key in a Signature dictionary</li>
</ul>

<p class="hangingindent" style="margin-left: 40px"><ins onMouseEnter="mouseEnter(this)" data-issue="211" data-iso="submitted">NOTE 1 For the signature schemes enumerated in ISO 32000-1 and in this document,
the value of the <b>Contents</b> key in a Signature dictionary is always a hexadecimal string (see "Table 255 — Entries in a signature dictionary").</ins></p>

<p>Encryption is not applied to other object types such as integers and boolean values, which are used primarily to convey information about the document's structure rather than its contents. ...</p>

<p>...</p>

<h4 id="H7.6.3.1">7.6.3.1 General</h4>

<p class="location">Change NOTE 1 as follows:</p>

<p class="hangingindent">NOTE 1 The name RC4&trade; is a registered trademark of RSA Security Inc. and cannot be used by third parties creating implementations of the algorithm. Proprietary implementations of the RC4 encryption algorithm are available under license from RSA Security Inc. For licensing information, contact: <del onMouseEnter="mouseEnter(this)" data-issue="95" data-iso="approved">RSA Security Inc. 2955 Campus Drive, Suite 400, San Mateo, CA 94403-2507, USA, or</del> <a href="http://www.rsasecurity.com/">http://www.rsasecurity.com/</a>.</p>

<p>...</p>

<h3 id="H7.6.4">7.6.4 Standard security handler</h3>

<h4 id="H7.6.4.1">7.6.4.1 General</h4>

<p class="location">Change the second paragraph above NOTE 2 as follows:</p>

<p>
If a security handler of revision 4 or 5 is specified, the standard security handler shall support crypt filters (see 7.6.6, "Crypt filters").
The support shall be limited to the <b>Identity</b> crypt filter (see "Table 26 - Standard crypt filter names") and
<del onMouseEnter="mouseEnter(this)" data-issue="89" data-iso="approved">crypt filters</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="89" data-iso="approved">a crypt filter</ins>
named <b>StdCF</b> whose dictionaries contain an <b>AuthEvent</b> value of <i>DocOpen</i>. For revision 4, the filter <b>CFM</b> value shall be <i>V2</i> (RC4) or <i>AESV2</i> (AES-128). For revision 6, the filter <b>CFM</b> value shall be <i>AESV3</i> (AES-256). Public-Key security handlers in this case shall use
<del onMouseEnter="mouseEnter(this)" data-issue="89" data-iso="approved">crypt filters</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="89" data-iso="approved">a crypt filter</ins>
named <b>DefaultCryptFilter</b> when all document content is encrypted, and shall use
<del onMouseEnter="mouseEnter(this)" data-issue="89" data-iso="approved">crypt filters</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="89" data-iso="approved">a crypt filter</ins>
named <b>DefEmbeddedFile</b> when file attachments only are encrypted in place of <b>StdCF</b> name. This nomenclature shall not be used as an indicator of the type of the security handler or encryption. Use of security handler revisions 1, 2, 3, 4 and 5 is deprecated in PDF 2.0.
</p>

<p>...</p>

<h5 id="H7.6.4.3.2">7.6.4.3.2 Algorithm 2: Computing a file encryption key in order to encrypt a document (revision 4 and earlier)</h5>

<p class="location">Change NOTE 2 as follows:</p>

<p class="hangingindent">NOTE 2  The first element of the ID array, as used in 7.6.4.3.2, "Algorithm 2: Computing a file encryption key in order to encrypt a document (revision 4 and earlier)", step e, generally remains unchanged across revisions of a given document. However, since this is not guaranteed, use of the ID in computation of the file encryption key, as required when using <del onMouseEnter="mouseEnter(this)" data-issue="53" data-iso="approved">7.6.4.3.3, "Algorithm 2.A: Retrieving the file encryption key from an encrypted document in order to decrypt it (revision 6 and later)</del>Algorithm 2: Computing a file encryption key in order to encrypt a document (revision 4 and earlier)", can complicate updates to the document. For this reason, security handlers are encouraged to use Algorithm 2.A or higher, which do not use the ID in file encryption key computation. <del onMouseEnter="mouseEnter(this)" data-issue="53" data-iso="approved">This algorithm, when applied to the user password string, produces the file encryption key used to encrypt or decrypt string and stream data according to 7.6.3.2, "Algorithm 1: Encryption of data using the RC4 or AES algorithms". Parts of this algorithm are also used in the algorithms described below.</del>
</p>

<p class="location">Insert new NOTE 3 immediately below NOTE 2 as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="53" data-iso="approved">NOTE 3  This algorithm, when applied to the user password string, produces the file encryption key used to encrypt or decrypt string and stream data according to 7.6.3.2, "Algorithm 1: Encryption of data using the RC4 or AES algorithms". Parts of this algorithm are also used in the algorithms described in 7.6.4.4, "Password algorithms".</ins>
</p>

<h5 id="H7.6.4.3.3">7.6.4.3.3 Algorithm 2.A: Retrieving the file encryption key from an encrypted document in order to decrypt it (revision 6 and later)</h5>

<p class="location">Insert new NOTE below bullet (f) as follows:</p>

<ol type="a" start="6">
<li>
Decrypt the 16-byte <b>Perms</b> string using AES-256 in ECB mode <del onMouseEnter="mouseEnter(this)" data-issue="24" data-iso="approved">with an initialization vector of zero</del>
and the file encryption key as the key. ...
</li>
</ol>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="53" data-iso="approved">NOTE This algorithm, when applied to the user password string, produces the file encryption key used to encrypt or decrypt string and stream data according to 7.6.3.3, "Algorithm 1.A: Encryption of data using the AES algorithms". Parts of this algorithm are also used in the algorithms described in 7.6.4.4, "Password algorithms".</ins>
</p>

<h5 id="H7.6.4.4.9">7.6.4.4.9 Algorithm 10: Computing the encryption dictionary's Perms (permissions) value (Security handlers of revision 6)</h5>

<p class="location">Change bullet (f) as follows:</p>

<ol type="a" start="6">
<li>
Encrypt the 16-byte block using AES-256 in ECB mode <del onMouseEnter="mouseEnter(this)" data-issue="24" data-iso="approved">with an initialization vector of zero</del>,
using the file encryption key as the key. The result (16 bytes) is stored as the <b>Perms</b> string, and checked for validity when the file is opened.
</li>
</ol>

<h5 id="H7.6.4.4.12">7.6.4.4.12 Algorithm 13: Validating the permissions (Security handlers of revision 6)</h5>

<p class="location">Change bullet (a) as follows:</p>

<ol type="a" start="1">
<li>
Decrypt the 16 byte <b>Perms</b> string using AES-256 in ECB mode <del onMouseEnter="mouseEnter(this)" data-issue="24" data-iso="approved">with an initialization vector of zero</del>
and the file encryption key as the key. ...
</li>
</ol>

<h3 id="H7.6.5">7.6.5 Public-key security handlers</h3>

<h4 id="H7.6.5.1">7.6.5.1 General</h4>

<p>...</p>

<h4 id="H7.6.5.2">7.6.5.2 Public-key security dictionary</h4>

<p>...</p>

<p class="location">Change the paragraph below the NOTE as follows:</p>

<p>
Permitted values of the <b>SubFilter</b> entry for use with conforming public-key security handlers are <i>adbe.pkcs7.s3</i><ins onMouseEnter="mouseEnter(this)" data-issue="219" data-iso="submitted"> (PDF 1.3)</ins>, <i>adbe.pkcs7.s4</i><ins onMouseEnter="mouseEnter(this)" data-issue="219" data-iso="submitted"> (PDF 1.4)</ins>, which shall be used when not using crypt filters (see 7.6.6, "Crypt filters") and <i>adbe.pkcs7.s5</i><ins onMouseEnter="mouseEnter(this)" data-issue="219" data-iso="submitted"> (PDF 1.5)</ins>, which shall be used when using crypt filters.
</p>

<p>...</p>

<p class="location">Insert a new subclause heading immediately below the NOTE below Table 23 as follows:</p>

<h4 id="H7.6.5.3"><ins onMouseEnter="mouseEnter(this)" data-issue="196" data-iso="submitted">7.6.5.3 Public-key security permissions</ins></h4>

<p class="editornote">EDITOR NOTE: current text and Table 24 remain unchanged.</p>

<p class="location">Renumber the next clause appropriately:</p>

<h4 id="H7.6.5.4"><del onMouseEnter="mouseEnter(this)" data-issue="196" data-iso="submitted">7.6.5.3</del><ins onMouseEnter="mouseEnter(this)" data-issue="196" data-iso="submitted">7.6.5.4</ins> Public-key encryption algorithms</h4>

<p class="location">Change the second bullet as follows:</p>

<ul>
 <li>...</li>
 <li>A 4-byte value defining the permissions, most significant byte first. See <ins onMouseEnter="mouseEnter(this)" data-issue="196" data-iso="submitted">7.6.5.3, "Public-key security permissions" and</ins> "Table 24 — Public-key security handler user access permissions" for the possible permission values.</li>
 <li>...</li>
</ul>

<p class="location">Add two new notes at the very end of the sub-clause as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="25" data-iso="approved">NOTE 1: This means that step c) only applies when both of the following conditions are met:</ins></p>

<ul>
<li><ins onMouseEnter="mouseEnter(this)" data-issue="25" data-iso="approved">the key is being generated for the crypt filter named <i>DefaultCryptFilter</i> (i.e. the crypt filter used as the value for <b>StmF</b> in the encryption dictionary);</ins></li>
<li><ins onMouseEnter="mouseEnter(this)" data-issue="25" data-iso="approved">the <b>EncryptMetadata</b> entry of the associated crypt filter dictionary is set to <i>false</i>.</ins></li>
</ul>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="25" data-iso="approved">
NOTE 2: Since crypt filters are not supported when <b>SubFilter</b> is set to <i>adbe.pkcs7.s3</i> or <i>adbe.pkcs7.s4</i> in the encryption dictionary,
there is no way to specify that metadata is to be left unencrypted in these cases. In particular, step c) is always skipped for these <b>SubFilter</b> values.
</ins></p>

<h3 id="H7.6.6">7.6.6 Crypt filters</h3>

<p class="location">Change the first bullet in the sub-clause as follows:</p>

<p>PDF 1.5 introduces crypt filters, which provide finer granularity control of encryption within a PDF file. The use of crypt filters involves the following structures:</p>

<ul>
  <li>The encryption dictionary (see "Table 20 - Entries common to all encryption dictionaries") contains entries that enumerate the crypt filters in the document (<b>CF</b>) and specify which ones are used by default to decrypt all the streams (<b>StmF</b>) and strings (<b>StrF</b>) in the document. In addition, the value of the V entry shall be 4 <ins onMouseEnter="mouseEnter(this)" data-issue="74" data-iso="approved">or 5</ins> to use crypt filters.
  </li>
</ul>

<p>...</p>

<p class="location">Change Table 25 as follows:</p>

<table>
  <caption id="Table25">Table 25 - Entries common to all crypt filter dictionaries</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Length</b></td>
    <td>integer</td>
    <td>
    <p>(<i>Required; deprecated in PDF 2.0</i>) ...</p>
    <p>
      When <b>CFM</b> is <i>AESV2</i>, the <b>Length</b> key shall have the value of 128<ins onMouseEnter="mouseEnter(this)" data-issue="184" data-iso="submitted"> for public-key security handlers, and 16 for the standard security handler</ins>.
      When <b>CFM</b> is <i>AESV3</i>, the <b>Length</b> key shall have a value of 256<ins onMouseEnter="mouseEnter(this)" data-issue="184" data-iso="submitted"> for public-key security handlers, and 32 for the standard security handler</ins>.
    </p>
    </td>
  </tr>
</table>

<p>...</p>

<p class="location">Change Table 27 as follows:</p>

<table>
  <caption id="Table27">Table 27 - Additional crypt filter dictionary entries for public-key security handlers</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Recipients</b></td>
    <td><ins onMouseEnter="mouseEnter(this)" data-issue="16" data-iso="approved">byte</ins> string or array</td>
    <td>
    <p>(<i>Required</i>) If the crypt filter is referenced from <b>StmF</b> or <b>StrF</b> in the encryption dictionary, this entry shall be an array of byte strings,
    where each <ins onMouseEnter="mouseEnter(this)" data-issue="16" data-iso="approved">byte</ins> string shall be a binary-encoded CMS object that shall ...</p>
    <p>...</p>
    <p>If the crypt filter is referenced from a <b>Crypt</b> filter decode parameter dictionary (see "Table 14 - Optional parameters for Crypt filters"),
    this entry shall be a <ins onMouseEnter="mouseEnter(this)" data-issue="16" data-iso="approved">byte</ins> string that shall be a binary-encoded CMS object that shall ...</p>
    </td>
  </tr>
</table>

<h2 id="H7.7">7.7 Document structure</h2>

<h3 id="H7.7.1">7.7.1 General</h3>

<p class="location">Move Figure 5 from subclause 7.7.2 to after the first paragraph, and update Figure 5 as follows:</p>

<ins onMouseEnter="mouseEnter(this)" data-issue="261"> 
  <figure>
    <img src="../assets/figure5-document-structure.svg" alt="Updated Figure 5 - Structure of a PDF document, additionally showing Document Part in PDF DOM">
    <figcaption>Figure 5 - Structure of a PDF document</figcaption>
  </figure>
</ins>

<h3 id="H7.7.2">7.7.2 Document catalog dictionary</h3>

<p>...</p>

<p class="location">Move Figure 5 - Structure of a PDF document from here to subclause 7.7.1:</p>

<del onMouseEnter="mouseEnter(this)" data-issue="261"> 
  <figure>
    <figcaption>Figure 5 - Structure of a PDF document</figcaption>
  </figure>
</del>

<p class="location">Change Table 29 as follows:</p>

<table>
  <caption id="Table29">Table 29 - Entries in the catalog dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Extensions</b></td>
    <td>dictionary</td>
    <td>
    (<i>Optional; <ins onMouseEnter="mouseEnter(this)" data-issue="242" data-iso="submitted">shall be a direct object;</ins> ISO 32000-1</i>) ...
    </td>
  </tr>
  <tr>
    <td><b>Dests</b></td>
    <td>dictionary</td>
    <td>
    (<i>Optional; PDF 1.1<del onMouseEnter="mouseEnter(this)" data-issue="106" data-iso="submitted">; shall be an indirect reference</del></i>) ...
    </td>
  </tr>
  <tr>
    <td><b>Outlines</b></td>
    <td>dictionary</td>
    <td>
    (<i>Optional<del onMouseEnter="mouseEnter(this)" data-issue="106" data-iso="submitted">; shall be an indirect reference</del></i>) ...
    </td>
  </tr>
  <tr>
    <td><b>Threads</b></td>
    <td>array</td>
    <td>
    (<i>Optional; PDF 1.1<del onMouseEnter="mouseEnter(this)" data-issue="106" data-iso="submitted">; shall be an indirect reference</del></i>) ...
    </td>
  </tr>
  <tr>
    <td><b>Lang</b></td>
    <td>text string</td>
    <td>
    <p>(<i>Optional; PDF 1.4</i>) A language identifier that shall specify the natural language for all text in the document except where overridden by language specifications for structure elements or marked-content (see 14.9.2, "Natural language specification"). If this entry is absent
    <ins onMouseEnter="mouseEnter(this)" data-issue="105" data-iso="approved"> or invalid (see 14.9.2, "Natural language specification")</ins>, the language shall be considered unknown.
    </p>
    <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="135" data-iso="submitted">NOTE All text in a document includes PDF text strings (see 7.9.2.2 "Text string type") as well as textual content.</ins>
    </p>
    </td>
  </tr>
</table>

<h3 id="H7.7.3">7.7.3 Page tree</h3>

<h4 id="H7.7.3.3">7.7.3.3 Page objects</h4>

<p class="location">Change Table 31 as follows:</p>

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
    <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="81" data-iso="approved">NOTE If the <b>Contents</b> key is not present, a <b>Resources</b> dictionary must still be present, either directly or through inheritance, in the pages tree.</ins></p>
    <p>...</p>
    </td>
  </tr>
  <tr>
    <td><b>ID</b></td>
    <td>byte string</td>
    <td>
    (<i>Optional; PDF 1.3<del onMouseEnter="mouseEnter(this)" data-issue="106" data-iso="submitted">; indirect reference preferred</del></i>) ...
    </td>
  </tr>
</table>


<h3 id="H7.7.4">7.7.4 Name dictionary</h3>

<p>...</p>

<p class="location">Change all occurrences of "name string" to "string" in Table 32 as follows:</p>

<table>
  <caption id="Table32">Table 32 - Entries in the name dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Dests</b></td>
    <td>name tree</td>
    <td>
    <p>(<i>Optional; PDF 1.2</i>) name tree mapping <del onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="submitted">name</del> strings to destinations (see 12.3.2.4, "Named destinations").</p>
    </td>
  </tr>
  <tr>
    <td><b>AP</b></td>
    <td>name tree</td>
    <td>
    <p>(<i>Optional; PDF 1.3</i>) name tree mapping <del onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="submitted">name</del> strings to annotation appearance streams (see 12.5.5, "Appearance streams").</p>
    </td>
  </tr>
  <tr>
    <td><b>JavaScript</b></td>
    <td>name tree</td>
    <td>
    <p>(<i>Optional; PDF 1.3</i>) name tree mapping <del onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="submitted">name</del> strings to document-level
       ECMAScript actions (see 12.6.4.17, "ECMAScript actions").</p>
    </td>
  </tr>
  <tr>
    <td><b>Pages</b></td>
    <td>name tree</td>
    <td>
    <p>(<i>Optional; PDF 1.3</i>) name tree mapping <del onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="submitted">name</del> strings to visible
       pages for use in interactive forms (see 12.7.7, "Named pages").</p>
    </td>
  </tr>
  <tr>
    <td><b>Templates</b></td>
    <td>name tree</td>
    <td>
    <p>(<i>Optional; PDF 1.3</i>) name tree mapping <del onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="submitted">name</del> strings to invisible
       (template) pages for use in interactive forms (see 12.7.7, "Named pages").</p>
    </td>
  </tr>
  <tr>
    <td><b>EmbeddedFiles</b></td>
    <td>name tree</td>
    <td>
    <p>(<i>Optional; PDF 1.4</i>) name tree mapping <del onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="submitted">name</del> strings to file
       specifications for embedded file streams (see 7.11.4, "Embedded file streams"). ...</p>
    <p>(<i>PDF 2.0</i>) For unencrypted wrapper documents for an encrypted payload document (see 7.6.7, "Unencrypted wrapper document") the
       <del onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="submitted">name</del> strings provided in this tree shall not contain or be derived from
       the encrypted payload document’s actual file name. ...</p>
    </td>
  </tr>  
  <tr>
    <td><b>AlternatePresentations</b></td>
    <td>name tree</td>
    <td>
    <p>(<i>Optional; PDF 1.4</i>) name tree mapping <del onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="submitted">name</del> strings to alternate presentations (see 13.5, "Alternate presentations").</p>
    </td>
  </tr>
  <tr>
    <td><b>Renditions</b></td>
    <td>name tree</td>
    <td>
    <p>(<i>Optional; PDF 1.5</i>) A name tree mapping <del onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="submitted">name</del> strings
       (which shall have <del onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="submitted">Unicode</del>
       <ins onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="submitted">a UTF-16BE</ins> encoding) to rendition objects (see 13.2.3, "Renditions").</p>
    </td>
  </tr>
</table>


<h3 id="H7.8.3">7.8.3 Resource dictionaries</h3>

<p class="location">Change the first bullet in the first bulleted list as follows:</p>

<p>A resource dictionary shall be associated with a content stream in one of the following ways:</p>

<ul>
<li>
For a content stream that is the value of a page's <b>Contents</b> entry
<del onMouseEnter="mouseEnter(this)" data-issue="9" data-iso="approved">(or is an element of an array that is the value of that entry)</del>, the resource dictionary shall
be designated by the page dictionary's <b>Resources</b> entry or is inherited, as described under 7.7.3.4, "Inheritance of page
attributes" from some ancestor node of the page object. ...
</li>
</ul>

<p>...</p>

<h2 id="H7.9">7.9 Common data structures</h2>
<h3 id="H7.9.2">7.9.2 String object types</h3>
<h4 id="H7.9.2.2">7.9.2.2 Text string type</h4>

<h5 id="H7.9.2.2.1">7.9.2.2.1 General</h5>

<p class="location">Change EXAMPLE 1 as follows:</p>

<p>EXAMPLE 1 A PDF dictionary containing key 'Key' with the value that is the text string "text&permil;" will look like</p>

<code>
 <del onMouseEnter="mouseEnter(this)" data-issue="96" data-iso="approved">&lt;&lt;/Key(text?)&gt;&gt;</del>
 <ins onMouseEnter="mouseEnter(this)" data-issue="96" data-iso="approved">&lt;&lt;/Key (text\213) &gt;&gt;</ins>
</code>

<p>where <del onMouseEnter="mouseEnter(this)" data-issue="96" data-iso="approved">the character '?' after the 'text' is represented by the hex code 8Bh (</del>octal code 213 <del onMouseEnter="mouseEnter(this)" data-issue="96" data-iso="approved">- that</del> is according to "D.2 Latin character set and encodings".</p>

<p>...</p>

<p class="location">Change EXAMPLE 2 as follows:</p>

<p>EXAMPLE 2 A PDF dictionary containing key 'Key' with the value that is the text string "&#x442;&#x435;&#x441;&#x442;" (that is what the word in Russian with the translation to English as 'test') will look like</p>

<code>
 <del onMouseEnter="mouseEnter(this)" data-issue="96" data-iso="approved">&lt;&lt;/Key(??????????)&gt;&gt;</del>
 <ins onMouseEnter="mouseEnter(this)" data-issue="96" data-iso="approved">&lt;&lt;/Key &lt;FEFF0442043504410442&gt; &gt;&gt;</ins>
</code>

<p><del onMouseEnter="mouseEnter(this)" data-issue="96" data-iso="approved">where the characters in parentheses is the sequence of bytes with hex codes FE, FF, 04, 42, 04, 35, 04, 41, 04, 42.</del></p>

<p>...</p>

<p class="location">Change NOTE 4 as follows:</p>

<p class="hangingindent">NOTE 4 This mechanism precludes beginning a string using <b>PDFDocEncoding</b>
with the three characters <del onMouseEnter="mouseEnter(this)" data-issue="161" data-iso="submitted">dieresis</del><ins onMouseEnter="mouseEnter(this)" data-issue="161" data-iso="submitted">idieresis</ins>,
guillemotright, questiondown, which is unlikely to be a meaningful beginning of a word or phrase.</p>

<p class="location">Delete NOTE 5 as follows:</p>

<p class="hangingindent"><del onMouseEnter="mouseEnter(this)" data-issue="96" data-iso="approved">NOTE 5  It is important not to confuse UTF-16BE with UCS2 (i.e. wchar_t). UTF-16 is not a fixed width encoding scheme.</del></p>


<h3 id="H7.9.6">7.9.6 Name trees</h3>

<p>...</p>

<p class="location">Change Table 36 as follows:</p>

<table>
  <caption id="Table36">Table 36 - Entries in a name tree node dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Names</b></td>
    <td>array</td>
    <td>
    <p>(<i>Root and leaf nodes only; required in leaf nodes; present in the root node if and only if <b>Kids</b> is not present</i>) Shall be an array of the form</p>
    <p>[<i>key<sub>1</sub> value<sub>1</sub> key<sub>2</sub> value<sub>2</sub> ...key<sub>n</sub> value<sub>n</sub></i>]</p>
    <p>where each <i>key<sub>i</sub></i> shall be a string and the corresponding <i>value<sub>i</sub></i> shall be the
      object associated with that key. The keys shall be sorted <del onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="submitted">in lexical order</del>, as described below.</p>
    </td>
  </tr>
</table>


<p class="location">Change the paragraph below Table 36 as follows:</p>

<p>The <b>Kids</b> entries in the root and intermediate nodes define the tree’s structure by identifying the immediate children of each node.
The <b>Names</b> entries in the leaf (or root) nodes shall contain the tree’s keys and their associated values, arranged in key-value pairs and shall be sorted
<del onMouseEnter="mouseEnter(this)" data-issue="214" data-iso="submitted">lexically</del> in ascending order by key. Shorter keys shall appear before longer ones beginning with the same byte sequence.
Any encoding of the keys may be used as long as it is self-consistent; keys shall be compared for equality on a simple byte-by-byte basis.
</p>

<p>...</p>

<h2 id="H7.10">7.10 Functions</h2>
<h3 id="H7.10.3">7.10.3 Type 2 (exponential interpolation) functions</h3>

<p class="location">Change the paragraph below Table 40 as follows:</p>

<p>Values of <b>Domain</b> shall constrain <i>x</i> in such a way that<ins onMouseEnter="mouseEnter(this)" data-issue="30" data-iso="approved">: </ins></p>

<ul>
    <li><ins onMouseEnter="mouseEnter(this)" data-issue="30" data-iso="approved">if <b>N</b> is not an integer, all values of <i>x</i> will be non-negative; and</ins></li>
    <li><ins onMouseEnter="mouseEnter(this)" data-issue="30" data-iso="approved">if <b>N</b> is negative, no value of <i>x</i> will be zero.</ins></li>
</ul>

<p>Typically, <b>Domain</b> is declared as [0.0 1.0], and <b>N</b> is a positive number. To clip the output to a specified range the <b>Range</b> attribute shall be used.</p>

<p>...</p>

<h3 id="H7.10.5">7.10.5 Type 4 (PostScript calculator) functions</h3>

<h4 id="H7.10.5.2">7.10.5 Operators and operands</h4>

<p class="location">Change Table 42 as follows:</p>

<table>
  <caption id="Table42">Table 42 - Operators in Type 4 functions</caption>
  <tr>
    <th>Operator Type</th>
    <th>Operators</th>
  </tr>
  <tr>
    <td>Conditional operators</td>
    <td>
      <del onMouseEnter="mouseEnter(this)" data-issue="269"><code>If</code></del> 
      <ins onMouseEnter="mouseEnter(this)" data-issue="269"><code>if</code></ins> 
      <code>ifelse</code>
    </td>
  </tr>
</table>

<h3 id="H7.11.4">7.11.4 Embedded file streams</h3>

<h4 id="H7.11.4.1">7.11.4.1 General</h4>

<p class="location">Change Table 44 as follows:</p>

<table>
  <caption id="Table44">Table 44 - Additional entries in an embedded file stream dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Subtype</b></td>
    <td>name</td>
    <td>
    <p>
    (<i>Optional, required in the case of an embedded file stream used as an associated file
    <ins onMouseEnter="mouseEnter(this)" data-issue="156" data-iso="submitted">(see 14.13 "Associated files") or as an asset of a RichMedia annotation (see "13.7 Rich media")</ins></i>) ...
    </p>
    </td>
  </tr>
</table>

<h3 id="H7.11.6">7.11.6 Collection items</h3>

<p class="location">Change Table 47 as follows:</p>

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
    The type of data shall match the data type identified by the corresponding collection field dictionary. <del onMouseEnter="mouseEnter(this)" data-issue="37" data-iso="approved">Default: <i>none</i>.</del>
    </p></td>
  </tr>
  <tr>
    <td><b>P</b></td>
    <td>text string</td>
    <td><p>
    (<i>Optional</i>) A prefix string that shall be concatenated with the text string presented to the user. This entry is ignored when an interactive PDF
    processor sorts the items in the collection. <del onMouseEnter="mouseEnter(this)" data-issue="37" data-iso="approved">Default: <i>none</i>.</del>
    </p></td>
  </tr>
</table>


<h3 id="H7.12.2">7.12.2 Extensions dictionary</h3>

<p class="location">Change Table 48 as follows:</p>

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
    (<i>Optional, shall be a direct <del onMouseEnter="mouseEnter(this)" data-issue="109" data-iso="approved">objectif</del> <ins onMouseEnter="mouseEnter(this)" data-issue="109" data-iso="approved">object if</ins> present</i>) The type of PDF object that this dictionary describes; if present, shall be <i>Extensions</i>.
    </td>
  </tr>
</table>

<h3 id="H7.12.5">7.12.5 ExtensionLevel</h3>

<p class="location">Change the paragraph as follows:</p>

<p>The value of the <b>ExtensionLevel</b> entry shall be an integer, which shall be interpreted with respect to the <b>BaseVersion</b> value.
If a developer has released multiple extensions against the same <b>BaseVersion</b> value, they <del onMouseEnter="mouseEnter(this)" data-issue="239" data-iso="submitted">shall</del><ins onMouseEnter="mouseEnter(this)" data-issue="239" data-iso="submitted">should</ins> be ordered over time and the <b>ExtensionLevel</b> numbers <del onMouseEnter="mouseEnter(this)" data-issue="239" data-iso="submitted">shall be a monotonically increasing sequence</del><ins onMouseEnter="mouseEnter(this)" data-issue="239" data-iso="submitted">should increase</ins> over time.
</p>

</div>

<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
