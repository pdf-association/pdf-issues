---
isodoc: ISO 32005:2023
title: 7. Parent-child relationships between the standard structure elements in the standard structure namespace for PDF 2.0 and PDF 1.7
last_modified_date: 11 July 2024
parent: 'ISO TS 32005: PDF 1.7 and 2.0 inclusion rules in PDF 2.0'
nav_order: 7
---

<ul>
 <li><a href="#H7.2">7.2 Hierarchical inclusion rules</a>
 </li>
</ul>
<hr>

<div class="isostyle">
<div class="fixedpopup" id="issuelink">
  Issue #xxxx
</div>

<p class="fake-h1">{{ page.title }}</p>

<h2 id="H7.2">7.2 Hierarchical inclusion rules</h2>

<p class="location">Change Table 5 as follows:</p>

<p class="editornote">EDITOR NOTE: the corrected hierarchical inclusion rules in Table 5 are also <a href="https://pdfa.org/resource/iso-ts-32005-hierarchical-inclusion-rules/" target="_blank">available as a spreadsheet</a> that was not included in the ISO/TS 32005:2023 publication.
</p>

<p class="editornote">EDITOR NOTE: as a result of <a href="https://github.com/pdf-association/pdf-issues/issues/440">Errata #440</a> modify Table Table 5 such that where Structure Type is <b>WP</b> and Child is <b>Figure</b> and where Structure Type is <b>Figure</b> and Parent is <b>WP</b> the undefined cell value <del onMouseEnter="mouseEnter(this)" data-issue="440" data-iso="approved">"c"</del> 
is corrected to be a <ins onMouseEnter="mouseEnter(this)" data-issue="440" data-iso="approved">"0..<i>n</i>"</ins> relationship.
The embedded spreadsheet data is also corrected.
</p>

<table>
  <caption id="Table35">Table 5 - Parent-child relationships between the PDF 1.7 elements and PDF 2.0 elements</caption>
  <tr>
    <th>Structure Type</th>
    <th style="width:40%;">Children<br/>Occ. Structure Type</th>
    <th style="width:40%;">Parents<br/>Occ. Structure Type</th>
  </tr>
  <tr style="vertical-align: top;">
    <td>Sub</td>
    <td>
      <table cellspacing="0" cellpadding="0" style="border-style: hidden;">
        <tr><td>0..n</td><td>NonStruct</td></tr>
        <tr><td>0..n</td><td>Private</td></tr>
        <tr><td>0..n</td><td>Note</td></tr>
        <tr><td>0..n</td><td>Code</td></tr>
        <tr><td>0..n</td><td>Lbl</td></tr>
        <tr><td>0..n</td><td>Em</td></tr>
        <tr><td>0..n</td><td>Strong</td></tr>
        <tr><td>0..n</td><td>Span</td></tr>
        <tr><td>0..n</td><td>Quote</td></tr>
        <tr><td>0..n</td><td>Link</td></tr>
        <tr><td>0..n</td><td>Reference</td></tr>
        <tr><td>0..n</td><td>Annot</td></tr>
        <tr><td>0..n</td><td>Form</td></tr>
        <tr><td>0..n</td><td>Ruby</td></tr>
        <tr><td>0..n</td><td>Warichu</td></tr>
        <tr><td>0..n</td><td>FENote</td></tr>
        <tr><td>0..n</td><td>L</td></tr>
        <tr><td>0..n</td><td>BibEntry</td></tr>
        <tr><td>0..n</td><td>Figure</td></tr>
        <tr><td>0..n</td><td>Formula</td></tr>
        <tr><td>0..n</td><td>Artifact</td></tr>
        <tr><td>0..n</td><td>content item</td></tr>
      </table>
    </td>
    <td>
      <table cellspacing="0" cellpadding="0"  style="border-style: hidden;">
        <tr><td>&Dagger;</td><td>Part</td></tr>
        <tr><td>&Dagger;</td><td>Div</td></tr>
        <tr><td>&Dagger;</td><td>NonStruct</td></tr>
        <tr>
          <td><ins onMouseEnter="mouseEnter(this)" data-issue="336">0..n</ins></td>
          <td><ins onMouseEnter="mouseEnter(this)" data-issue="336">Code</ins></td>
        </tr>
        <tr><td>0..n</td><td>Private</td></tr>
        <tr><td>0..n</td><td>P</td></tr>
        <tr><td>0..n</td><td>Note</td></tr>
        <tr><td>0..n</td><td>Hn</td></tr>
        <tr><td>0..n</td><td>H</td></tr>
        <tr><td>0..n</td><td>Lbl</td></tr>
        <tr><td>0..n</td><td>Em</td></tr>
        <tr><td>0..n</td><td>Strong</td></tr>
        <tr><td>0..n</td><td>Span</td></tr>
        <tr><td>0..n</td><td>Quote</td></tr>
        <tr><td>0..n</td><td>Link</td></tr>
        <tr><td>0..n</td><td>Annot</td></tr>
        <tr><td>0..n</td><td>RB</td></tr>
        <tr><td>0..n</td><td>RT</td></tr>
        <tr><td>0..n</td><td>RP</td></tr>
        <tr><td>0..n</td><td>WT</td></tr>
        <tr><td>0..n</td><td>WP</td></tr>
        <tr><td>0..n</td><td>FENote</td></tr>
        <tr><td>0..n</td><td>LBody</td></tr>
        <tr><td>0..n</td><td>Caption</td></tr>
        <tr><td>&#x2205;*</td><td>Figure</td></tr>
        <tr><td>0..n</td><td>Formula</td></tr>
        <tr><td>0..n</td><td>Artifact</td></tr>
      </table>
    </td>
  </tr>
  <tr>
    <td>...</td>
    <td>...</td>
    <td>...</td>
  </tr>
  <tr style="vertical-align: top;">
    <td>Code</td>
    <td>
      <table cellspacing="0" cellpadding="0" style="border-style: hidden;">
        <tr><td>&#x2205;*</td><td>DocumentFragment</td></tr>
        <tr><td>0..n</td><td>Part</td></tr>
        <tr><td>0..n</td><td>Div</td></tr>
        <tr><td>0..n</td><td>NonStruct</td></tr>
        <tr><td>0..n</td><td>Private</td></tr>
        <tr><td>0..n</td><td>Note</td></tr>
        <tr><td>0..n</td><td>Em</td></tr>
        <tr><td>0..n</td><td>Strong</td></tr>
        <tr><td>0..n</td><td>Span</td></tr>
        <tr>
          <td><ins onMouseEnter="mouseEnter(this)" data-issue="336">0..n</ins></td>
          <td><ins onMouseEnter="mouseEnter(this)" data-issue="336">Sub</ins></td>
        </tr>
        <tr><td>0..n</td><td>Link</td></tr>
        <tr><td>0..n</td><td>Reference</td></tr>
        <tr><td>0..n</td><td>Annot</td></tr>
        <tr><td>0..n</td><td>FENote</td></tr>
        <tr><td>0..n</td><td>BibEntry</td></tr>
        <tr><td>0..n</td><td>Artifact</td></tr>
        <tr><td>0..n</td><td>content item</td></tr>
      </table>
    </td>
    <td>
      <table cellspacing="0" cellpadding="0" style="border-style: hidden;">
        <tr><td>0..n</td><td>Document</td></tr>
        <tr><td>0..n</td><td>DocumentFragment</td></tr>
        <tr><td>&Dagger;</td><td>Part</td></tr>
        <tr><td>&Dagger;</td><td>Div</td></tr>
        <tr><td>0..n</td><td>Art</td></tr>
        <tr><td>0..n</td><td>Sect</td></tr>
        <tr><td>0..n</td><td>Aside</td></tr>
        <tr><td>0..n</td><td>BlockQuote</td></tr>
        <tr><td>&Dagger;</td><td>NonStruct</td></tr>
        <tr><td>0..n</td><td>Private</td></tr>
        <tr><td>0..n</td><td>Title</td></tr>
        <tr><td>0..n</td><td>Sub</td></tr>
        <tr><td>0..n</td><td>P</td></tr>
        <tr><td>0..n</td><td>Note</td></tr>
        <tr><td>0..n</td><td>Hn</td></tr>
        <tr><td>0..n</td><td>H</td></tr>
        <tr><td>0..n</td><td>Lbl</td></tr>
        <tr><td>0..n</td><td>Em</td></tr>
        <tr><td>0..n</td><td>Strong</td></tr>
        <tr><td>0..n</td><td>Span</td></tr>
        <tr><td>0..n</td><td>Quote</td></tr>
        <tr><td>0..n</td><td>Link</td></tr>
        <tr><td>0..n</td><td>Annot</td></tr>
        <tr><td>&#x2205;*</td><td>Form</td></tr>
        <tr><td>0..n</td><td>FENote</td></tr>
        <tr><td>0..n</td><td>LBody</td></tr>
        <tr><td>0..n</td><td>TH</td></tr>
        <tr><td>0..n</td><td>TD</td></tr>
        <tr><td>0..n</td><td>Caption</td></tr>
        <tr><td>0..n</td><td>Figure</td></tr>
        <tr><td>0..n</td><td>Formula</td></tr>
        <tr><td>0..n</td><td>Artifact</td></tr>
      </table>
    </td>
  </tr>
  <tr>
    <td>...</td>
    <td>...</td>
    <td>...</td>
  </tr>
  <tr style="vertical-align: top;">
    <td>WP</td>
    <td>
      <table cellspacing="0" cellpadding="0" style="border-style: hidden;">
        <tr><td>0..n</td><td>NonStruct</td></tr>
        <tr><td>0..n</td><td>Private</td></tr>
        <tr><td>0..n</td><td>Sub</td></tr>
        <tr><td>0..n</td><td>Em</td></tr>
        <tr><td>0..n</td><td>String</td></tr>
        <tr><td>0..n</td><td>Span</td></tr>
        <tr><td>0..n</td><td>Quote</td></tr>
        <tr><td>0..n</td><td>Link</td></tr>
        <tr><td>0..n</td><td>Reference</td></tr>
        <tr><td>0..n</td><td>Annot</td></tr>
        <tr><td>0..n</td><td>Form</td></tr>
        <tr>
          <td><del onMouseEnter="mouseEnter(this)" data-issue="440" data-iso="approved">c</del>
              <ins onMouseEnter="mouseEnter(this)" data-issue="440" data-iso="approved">0..n</ins></td>
          <td>Figure</td>
        </tr>
        <tr><td>0..n</td><td>Artifact</td></tr>
        <tr><td>&Dagger;</td><td>content item</td></tr>
      </table>
    </td>
    <td>
      <table cellspacing="0" cellpadding="0" style="border-style: hidden;">
        <tr><td>&Dagger;</td><td>Div</td></tr>
        <tr><td>&Dagger;</td><td>NonStruct</td></tr>
        <tr><td>0..n</td><td>Private</td></tr>
        <tr><td>[b]</td><td>Warichu</td></tr>
        <tr><td>0..n</td><td>Artifact</td></tr>
      </table>
    </td>
  </tr>
  <tr>
    <td>...</td>
    <td>...</td>
    <td>...</td>
  </tr>
  <tr style="vertical-align: top;">
    <td>Figure</td>
    <td>
      <table cellspacing="0" cellpadding="0" style="border-style: hidden;">
        <tr><td>...</td><td>...</td></tr>
      </table>
    </td>
    <td>
      <table cellspacing="0" cellpadding="0" style="border-style: hidden;">
        <tr><td>...</td><td>...</td></tr>
        <tr>
          <td><del onMouseEnter="mouseEnter(this)" data-issue="440" data-iso="approved">c</del>
              <ins onMouseEnter="mouseEnter(this)" data-issue="440" data-iso="approved">0..n</ins></td>
          <td>Figure</td>
        </tr>
        <tr><td>...</td><td>...</td></tr>
      </table>
    </td>
  </tr>
</table>

</div>
