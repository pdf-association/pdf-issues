---
subset: PDF/A-4
isodoc: ISO 19005-4:2020
title: 6. Technical requirements
last_modified_date: 14 February 2022
parent: ISO 19005-4:2020 PDF/A-4
nav_order: 6
---

<nav class="subclauses">
<ul class="noprint">
  <li>6 Technical requirements
   <ul>
    <li>6.2 Graphics
        <ul>
            <li><a href="#H6.2.9">6.2.9 Transparency</a>
            </li>
        </ul>
        <ul>
          <li>6.2.10 Fonts
            <ul>
              <li>6.2.10.3 Composite Fonts
                <ul>
                  <li><a href="#H6.2.10.3.1">6.2.10.3.1 General</a>
                  </li>
                </ul>
              </li>
            </ul>
          </li>
        </ul>
    </li>
    <li>6.7 Metadata
     <ul>
      <li><a href="#H6.7.3">6.7.3 Version identification</a>
      </li>
     </ul>
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

<h2 id="H6.2">6.2 Graphics</h2>

<h3 id="H6.2.9">6.2.9 Transparency</h3>

<p class="location">Change the second paragraph as follows:</p>

<p class="hangingindent">
NOTE <ins onMouseEnter="mouseEnter(this)" data-issue="104" data-iso="approved">1</ins>
This requirement ensures that there is always an explicitly defined transparency blending space specified for any content which has associated transparency.
</p>

<p class="location">Insert a new NOTE 2 after the existing NOTE (renumbered) as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="104" data-iso="approved">Note 2 Page transparency can be determined as defined in ISO 32000-2:2020, Annex Q.</ins>
</p>

<p>...</p>

<h3 id="H6.2.10">6.2.10 Fonts</h3>

<h4 id="H6.2.10.3">6.2.10.3 Composite fonts</h4>

<h5 id="H6.2.10.3.1">6.2.10.3.1 General</h5>

<p class="location">Change the last bullet as follows:</p>

<ul>
  <li>...</li>
  <li>
  Otherwise the corresponding values of the <b>Registry</b> and <b>Ordering</b> keys in both CIDSystemInfo dictionaries shall be identical, and the value of the <b>Supplement</b> key in the CIDSystemInfo dictionary of the CIDFont shall be <del onMouseEnter="mouseEnter(this)" data-issue="77">greater</del> <ins onMouseEnter="mouseEnter(this)" data-issue="77">less</ins> than or equal to the value of the <b>Supplement</b> key in the CIDSystemInfo dictionary of the CMap.
  </li>
</ul>


<h2 id="H6.7">6.7 Metadata</h2>

<h3 id="H6.7.3">6.7.3 Version identification</h3>

<p class="location">Add a new NOTE before Table 2 as follows:</p>

<p>The PDF/A identification schema defined in Table 2 uses the namespace URI http<del onMouseEnter="mouseEnter(this)" data-issue="123" data-iso="approved">s</del>://www.aiim.org/pdfa/ns/id/. The required schema namespace prefix is <b>pdfaid</b>.
</p>

<p><ins onMouseEnter="mouseEnter(this)" data-issue="123" data-iso="approved">
NOTE there was an error in a previous edition of this document and implementations may choose to accept "https" in addition to "http" for the namespace URI.
</ins></p>

<p class="location">Change Table 2 as follows:</p>

<table>
  <caption id="Table2">Table 2 - PDF/A identification schema</caption>
  <tr>
    <th>Property</th>
    <th>Value type</th>
    <th>Category</th>
    <th>Explanation</th>
  </tr>
  <tr>
    <td><b>pdfa<ins onMouseEnter="mouseEnter(this)" data-issue="123" data-iso="approved">id</ins>:conformance</b></td>
    <td>Closed choice of Text</td>
    <td>Internal</td>
    <td>(Optional) PDF/A conformance level: E or F</td>
  </tr>
</table>

</div>
