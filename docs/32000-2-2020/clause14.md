---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 14
title: Document interchange
modified: 30 July 2021
---

<ul>
 <li><a href="#H14.5">14.5 Page-piece dictionaries</a>
 </li>
 <li>14.7 Logical structure
  <ul>
   <li><a href="#H14.7.2">14.7.2 Structure hierarchy</a>
   </li>
  </ul>
 </li>
 <li>14.8 Tagged PDF
  <ul>
   <li>14.8.4 Standard structure types
    <ul>
     <li>14.8.4.7 Inline level structure types
      <ul>
       <li><a href="#H14.8.4.7.2">14.8.4.7.2 General inline level structure types</a>
       </li>
      </ul>
     </li>
     <li>14.8.4.8 Other structure types
      <ul>
       <li><a href="#H14.8.4.8.3">14.8.4.8.3 Table structure types</a>
       </li>
       <li><a href="#H14.8.4.8.4">14.8.4.8.4 Caption structure types</a>
       </li>
      </ul>
     </li>
    </ul>
   </li>
   <li>14.8.6 Standard structure namespaces
    <ul>
     <li><a href="#H14.8.6.1">14.8.6.1 Namespaces for standard structure types and attributes</a>
     </li>
     <li><a href="#H14.8.6.2">14.8.6.2 Role maps and namespaces</a>
     </li>
     <li><a href="#H14.8.6.3">14.8.6.3 Other namespaces</a>
     </li>
    </ul>
   </li>
  </ul>
 </li>
 <li>14.12 Document parts
  <ul>
   <li>14.12.4 Data structures
    <ul>
     <li><a href="#H14.12.4.2">14.12.4.2 Document part metadata</a>
     </li>
    </ul>
   </li>
  </ul>
 </li>
 <li>14.13 Associated files
  <ul>
   <li><a href="#H14.13.5">14.13.5 Associated files linked to graphics objects</a>
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

<h2 id="H14.5">14.5 Page-piece dictionaries</h2>

<p>
As "Table 350 - Entries in a page-piece dictionary" shows, a page-piece dictionary may contain any number of entries,
each <del onMouseEnter="mouseEnter(this)" data-issue="69">keyed by</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="69">key should be a second-class name, or</ins>
the name of a distinct PDF processor, or of a well-known data type recognised by a family of PDF processors.
</p>

<table>
  <caption id="Table350">Table 350 - Entries in a page-piece dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td>any valid second-class name <ins onMouseEnter="mouseEnter(this)" data-issue="69">(<i>recommended</i>), any conforming product name or well known data type</ins></td>
    <td>dictionary</td>
    <td>A data dictionary (see "Table 351 - Entries in a data dictionary").
    </td>
  </tr>
</table>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="69"> NOTE: the definition of page-piece dictionary keys was updated to also support the same definition as in ISO 32000-1:2008 to allow easier document upgrades to PDF 2.0, however second-class names are strongly recommend.</ins>
</p>

<h3 id="H14.7.2">14.7.2 Structure hierarchy</h3>

<p>...</p>

<table>
  <caption id="Table355">Table 355 - Entries in a structure element dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td>R</td>
    <td>integer</td>
    <td>(<i>Optional<ins onMouseEnter="mouseEnter(this)" data-issue="93">; deprecated in PDF 2.0</ins></i>) The current revision number of this structure element (see 14.7.6.3, "Attribute revision numbers"). The value shall be a non-negative integer. Default value: 0.
    </td>
  </tr>
</table>


<h5 id="H14.8.4.7.2">14.8.4.7.2 General inline level structure types</h5>


<table>
  <caption id="Table368">Table 368 - General inline level structure types</caption>
  <tr>
    <th>Structure Type</th>
    <th>Category</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><b>Strong</b></td>
    <td>Inline</td>
    <td>
    <p>(<i>PDF 2.0</i>) Encloses content for the purpose of strong importance, seriousness or urgency for its contents.</p>
    <p>EXAMPLE 3 In this example the <b>Strong</b> element is used to denote the content
    that <del onMouseEnter="mouseEnter(this)" data-issue="84">the user is intended to read first</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="84">is more important</ins>:
    </p>
    <p>...</p>
    </td>
  </tr>
</table>


<h5 id="H14.8.4.8.3">14.8.4.8.3 Table structure types</h5>


<table>
  <caption id="Table371">Table 371 - Table standard structure types</caption>
  <tr>
    <th>Structure Type</th>
    <th>Category</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><b>TR</b></td>
    <td>Internal to a <b>Table</b> structure</td>
    <td>
    A row of table header cells (<b>TH</b>) or table data cells (<b>TD</b>)<ins onMouseEnter="mouseEnter(this)" data-issue="71">or both</ins> in a table.
    </td>
  </tr>
</table>


<h5 id="H14.8.4.8.4">14.8.4.8.4 Caption structure types</h5>


<table>
  <caption id="Table372">Table 372 - Standard structure type Caption</caption>
  <tr>
    <th>Structure Type</th>
    <th>Category</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><b>Caption</b></td>
    <td>Grouping or Block</td>
    <td>
    <p>...</p>
    <p>A structure element is understood to be "captioned" when a <b>Caption</b> structure element exists as an immediate child of that structure element.
    The <b>Caption</b> shall be the first or the last structure element inside its parent structure element. The number of captions cannot exceed 1.
    </p>
    <p>While captions are often used with figures or formulas, they may be associated with any type of content.</p>
    <p class="hangingindent">NOTE <ins onMouseEnter="mouseEnter(this)" data-issue="35">1</ins> In principle, captions can appear in a nested fashion. For example, several smaller images belonging to a group of images can each
    be accompanied by a caption, and the group of these images as a whole is accompanied by a caption as well.</p>
    <p class="hangingindent">
    <ins onMouseEnter="mouseEnter(this)" data-issue="35">NOTE 2 If an <b>Artifact</b> structure element is present, and needs to be associated with a <b>Caption</b>, then the <b>Artifact</b> structure element needs to be a descendent of the <b>Caption</b>.</ins>
    </p>
    </td>
  </tr>
</table>


<h4 id="H14.8.6.1">14.8.6.1 Namespaces for standard structure types and attributes</h4>

<p>...</p>

<p>The term <i>standard structure namespaces</i> refers to either of the two namespaces defined above.</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="8"> NOTE: Namespaces are designed to provide greater interchange of PDFs including logical structure, providing a means to identify the custom namespace for each element, if appropriate. However, structure elements types in undefined namespaces continue to be permitted. </ins>
</p>


<h4 id="H14.8.6.2">14.8.6.2 Role maps and namespaces</h4>

<p>...</p>

<ins onMouseEnter="mouseEnter(this)" data-issue="65">
<p>EXAMPLE:</p>
<code>
17 0 obj
<<
   /Type /StructElem
   /S /section
   /P 5 0 R
   /NS 15 0 R
>>
endobj

15 0 obj
<<
   /Type /Namespace
   /NS (urn:uuid:A63861E-9F7-4FCB-9B27-C3BC8D9BFB06)
   /RoleMapNS 16 0 R
>>
endobj

16 0 obj
<<
   /section [/H1 11 0 R]
   ...
>>
endobj
</code>
</ins>


<h4 id="H14.8.6.3">14.8.6.3 Other namespaces</h4>

<p>...</p>

<p class="hangingindent">NOTE 1 MathML is the only domain-specific namespace defined in PDF 2.0.</p>

<p>
<del onMouseEnter="mouseEnter(this)" data-issue="72">When including mathematics structured as MathML 3.0, the math structure element type as defined in MathML 3.0 shall be used, and shall have its namespace explicitly defined (see 14.7.4.2, "Namespace dictionary").</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="72">When including mathematics structured as MathML 3.0, the <b>math</b> structure element type, as defined in MathML 3.0, shall be used to enclose the formula under the <b>Formula</b> structure element type. All MathML structure element types and their attributes shall have the MathML 3.0 namespace explicitly defined (see 14.7.4.2, "Namespace dictionary").</ins>
</p>

<p>...</p>


<h4 id="H14.12.4.2">14.12.4.2 Document part metadata</h4>

<p>...</p>

<p>
The values of keys present in the DPM dictionary, or of any dictionary or array object present in the DPM dictionary, shall only be of type text string, date string,
<ins onMouseEnter="mouseEnter(this)" data-issue="86">name,</ins>
array, dictionary, boolean, integer or real as defined in 7.3, "Objects".
<ins onMouseEnter="mouseEnter(this)" data-issue="86">All key values that are PDF name objects, after expansion of character sequences escaped with a NUMBER SIGN (23h), if any, shall be valid UTF-8 character sequences.</ins>
Other PDF value types shall not be used.
</p>


<h3 id="H14.13.5">14.13.5 Associated files linked to graphics objects</h3>


<p>...</p>

<p>
The property list associated with the marked-content shall specify an array of file specification dictionaries to which
the content is associated. The named resource in the
<del onMouseEnter="mouseEnter(this)" data-issue="14"><b>Property List</b></del>
<ins onMouseEnter="mouseEnter(this)" data-issue="14"><i>property list</i></ins>
(see 14.6.2, "Property lists") shall specify an array of file specification dictionaries to which the content is associated.
The relationship that the associated files have to the PDF content is supplied by the AFRelationship key in each file specification dictionary.
</p>

<p>...</p>


</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
