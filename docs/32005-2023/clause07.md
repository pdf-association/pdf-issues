---
isodoc: ISO 32005:2023
clause: 7
title: Parent-child relationships between the standard structure elements in the standard structure namespace for PDF 2.0 and PDF 1.7
modified: 15 October 2023
---

<ul>
 <li><a href="#H7.2">7.2 Hierarchical inclusion rules</a>
 </li>
</ul>
<hr>

<link rel="stylesheet" href="../assets/iso-style.css">
<div class="isostyle">
<div class="fixedpopup" id="issuelink">
	Issue #xxxx
</div>


<p class="fake-h1">{{ page.clause }}. {{ page.title }}</p>

<h2 id="H7.2">7.2 Hierarchical inclusion rules</h2>

<p class="location">Change Table 5 as follows:</p>

<p class="editornote">EDITOR NOTE: the corrected hierarchical inclusion rules in Table 5 are also <a href="https://pdfa.org/resource/iso-ts-32005-hierarchical-inclusion-rules/" target="_blank">available as a spreadsheet</a> that was not included in the ISO/TS 32005:2023 publication.
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
</table>

</div>

<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
