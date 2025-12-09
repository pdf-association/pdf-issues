---
isodoc: ISO 32001:2022
title: 5. Digital signature enhancements
last_modified_date: 10 November 2024
parent: 'ISO TS 32001: PDF 2.0 Hash Algorithm extensions'
nav_order: 5
---

<ul>
 <li>5.1 Support for secure hash algorithm 3 (SHA-3) hash family
  <ul>
   <li><a href="#H5.1.3"><del onMouseEnter="mouseEnter(this)" data-issue="236" data-iso="approved">5.1.3 Changes to ISO 32000-2:2020, Table 256 — Entries in a signature reference dictionary</del></a>
   </li>
   <li><a href="#H5.1.4">5.1.4 Changes to ISO 32000-2:2020, Table 260 — SubFilter value algorithm support</a>
   </li>
  </ul>
 </li>
</ul>
<hr>

<div class="isostyle">
<div class="fixedpopup" id="issuelink">
  Issue #xxxx
</div>


<p class="fake-h1">{{ page.title }}</p>

<h2 id="H5.1">5.1 Support for secure hash algorithm 3 (SHA-3) hash family</h2>

<p class="location">Delete all of clause 5.1.3 as follows:</p>

<h3 id="H5.1.3"><del onMouseEnter="mouseEnter(this)" data-issue="236" data-iso="approved">5.1.3 Changes to ISO 32000-2:2020, Table 256 — Entries in a signature reference dictionary</del></h3>

<p>
<del onMouseEnter="mouseEnter(this)" data-issue="236" data-iso="approved">
In ISO 32000-2:2020, Table 256 (“Entries in a signature reference dictionary”; 12.8.1, “General”), the following text is added to the end of the current <b>DigestMethod</b> value text:
</del>
</p>

<p>
<del onMouseEnter="mouseEnter(this)" data-issue="236" data-iso="approved">
(PDF 2.x) In addition to those values previously defined, this value may be one of SHA3-256, SHA3-384, SHA3-512 or SHAKE256. Default value for PDF 2.0: SHA256 (PDF 2.0).
</del>
</p>


<h3 id="H5.1.4">5.1.4 Changes to ISO 32000-2:2020, Table 260 — SubFilter value algorithm support</h3>

<p class="location">Change the last bullet point of the bullted list as follows:</p>

<ul>
  <li>...</li>
  <li>SHAKE256 (PDF 2.x). When SHAKE256 is 
  <del onMouseEnter="mouseEnter(this)" data-issue="404">specified, the message digest algorithm identified by the id-shake256 object identifier (OID) in section 2.3 of RFC 8419 shall be used</del>
  <ins onMouseEnter="mouseEnter(this)" data-issue="404">used, the applicable stipulations on algorithm identifiers in RFC 8702, 3.1 and RFC 8419, 3.1, 3.2 shall be followed</ins>.
  </li>
</ul>

</div>
