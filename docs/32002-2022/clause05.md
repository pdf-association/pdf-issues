---
isodoc: ISO 32002:2022
title: 5. Digital signature enhancements
last_modified_date: 11 Sept 2024
parent: 'ISO TS 32002: PDF 2.0 Digital Signature extensions'
nav_order: 5
---

<nav class="subclauses">
<ul class="noprint">
 <li>5.1 Elliptic curve cryptography
  <ul>
   <li><a href="#H5.1.2">5.1.2 Proposed changes to ISO 32000-2:2020 Table 260 – SubFilter value algorithm support</a>
   </li>
   <li><a href="#H5.1.3">5.1.3 Specification of allowed elliptic curves</a>
   </li>
  </ul>
 </li>
</ul>
</nav>
<hr>

<div class="isostyle">
<div class="fixedpopup" id="issuelink">
  Issue #xxxx
</div>

<p class="fake-h1">{{ page.title }}</p>

<h2 id="H5.1">5.1 Elliptic curve cryptography</h2>

<h3 id="H5.1.2">5.1.2 Proposed changes to ISO 32000-2:2020 Table 260 – SubFilter value algorithm support</h3>

<p class="location">Change Table 2 as follows:</p>

<table>
  <caption id="Table2">Table 2 - Additional permitted SubFilter values for ISO 32000-2:2020, Table 260</caption>
  <tr>
    <th>SubFilter value</th>
    <th>adbe.pkcs7.detached, ETSI.CAdES.detached or ETSI.RFC3161</th>
    <th>adbe.pkcs7.sha1 (c)</th>
    <th>adbe.x509.rsa_sha1 (a)</th>
  </tr>
  <tr>
    <td>EdDSA algorithm support</td>
    <td>IETF RFC 8032, Edwards-curve Digital Signature Algorithm (EdDSA) (PDF 2.x) using the Ed25519 or Ed448 elliptic curves<sup>b</sup></td>
    <td>No</td>
    <td>No</td>
  </tr>
  <tr>
    <td colspan="4">
      <p>b When using the Ed25519 EdDSA elliptic curve algorithm, the message digest shall be computed using the SHA512 message digest algorithm 
      <del onMouseEnter="mouseEnter(this)" data-issue="404">with OID id-sha512 as defined in IETF RFC 8419:2018, 2.3</del>. 
      When using the Ed448 EdDSA elliptic curve algorithm, the message digest shall be computed using the SHAKE256 message digest algorithm
      <del onMouseEnter="mouseEnter(this)" data-issue="404">with OID id-shake256 as defined in IETF RFC 8419:2018, 2.3</del>.
      </p>
    </td>
  </tr>
</table>

<h3 id="H5.1.3">5.1.3 Specification of allowed elliptic curves</h3>

<p class="location">Change Table 4 as follows:</p>

<table>
  <caption id="Table4">Table 4 - Supported EdDSA elliptic curves</caption>
  <tr>
    <th>Elliptic curve name</th>
    <th>Digest algorithms</th>
    <th>Restrictions</th>
  </tr>
  <tr>
    <td>Ed25519</td>
    <td>SHA512</td>
    <td></td>
  </tr>
  <tr>
    <td>Ed448</td>
    <td>SHAKE256</td>
    <td>
       <del onMouseEnter="mouseEnter(this)" data-issue="404">Message digests shall be calculated using the fixed length id-shake256 message digest algorithm in accordance with ISO/TS 32001.</del>
       <ins onMouseEnter="mouseEnter(this)" data-issue="404">The applicable stipulations of RFC 8419, 3.1, 3.2 on algorithm identifiers for SHAKE256 shall be followed.</ins>
    </td>
  </tr>
</table>

</div>
