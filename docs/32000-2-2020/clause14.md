---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 14
title: Document interchange
---

{% include iso-style.html %}
<div class="isostyle">


<h1>{{ page.clause }}. {{ page.title }}</h1>


<h2>14.5 Page-piece dictionaries</h2>

<p>
As "Table 350 - Entries in a page-piece dictionary" shows, a page-piece dictionary may contain any number of entries,
each <span class="deleted-text">keyed by<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/69">Issue #69</a></span></span>
<span class="new-text">key should be a second-class name, or<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/69">Issue #69</a></span></span>
the name of a distinct PDF processor, or of a well-known data type recognised by a family of PDF processors.
</p>

<table>
  <caption>Table 350 - Entries in a page-piece dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td>any valid second-class name <span class="new-text">(<i>recommended</i>), any conforming product name or well known data type<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/69">Issue #69</a></span></span></td>
    <td>dictionary</td>
    <td>A data dictionary (see "Table 351 - Entries in a data dictionary").
    </td>
  </tr>
</table>

<p><span class="new-text">
NOTE: the definition of page-piece dictionary keys was updated to also support the same definition as in ISO 32000-1:2008 to allow easier document
upgrades to PDF 2.0, however second-class names are strongly recommend.
<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/69">Issue #69</a></span></span>
</p>

<h3>14.7.2 Structure hierarchy</h3>

<p>...</p>

<table>
  <caption>Table 355 - Entries in a structure element dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td>R</td>
    <td>integer</td>
    <td>(<i>Optional<span class="new-text">; deprecated in PDF 2.0<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/93">Issue #93</a></span></span></i>) The current revision number of this structure element (see 14.7.6.3, "Attribute revision numbers"). The value shall be a non-negative integer. Default value: 0.
    </td>
  </tr>
</table>


<h5>14.8.4.7.2 General inline level structure types</h5>


<table>
  <caption>Table 368 - General inline level structure types</caption>
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
    that <span class="deleted-text">the user is intended to read first<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/84">Issue #84</a></span></span>
    <span class="new-text">is more important<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/84">Issue #84</a></span></span>:
    </p>
    <p>...</p>
    </td>
  </tr>
</table>


<h5>14.8.4.8.3 Table structure types</h5>


<table>
  <caption>Table 371 - Table standard structure types</caption>
  <tr>
    <th>Structure Type</th>
    <th>Category</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><b>TR</b></td>
    <td>Internal to a <b>Table</b> structure</td>
    <td>
    A row of table header cells (<b>TH</b>) or table data cells (<b>TD</b>)<span class="new-text">or both<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/71">Issue #71</a></span></span> in a table.
    </td>
  </tr>
</table>


<h5>14.8.4.8.4 Caption structure types</h5>


<table>
  <caption>Table 372 - Standard structure type Caption</caption>
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
    <p>NOTE <span class="new-text">1<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/35">Issue #35</a></span></span> In principle, captions can appear in a nested fashion. For example, several smaller images belonging to a group of images can each
    be accompanied by a caption, and the group of these images as a whole is accompanied by a caption as well.</p>
    <p><span class="new-text">NOTE 2 If an <b>Artifact</b> structure element is present, and needs to be associated with a <b>Caption</b>, then the <b>Artifact</b>
    structure element needs to be a descendent of the <b>Caption</b>.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/35">Issue #35</a></span></span></p>
    </td>
  </tr>
</table>


<h4>14.8.6.1 Namespaces for standard structure types and attributes</h4>

<p>...</p>

<p>The term <i>standard structure namespaces</i> refers to either of the two namespaces defined above.</p>

<p><span class="new-text">
NOTE: Namespaces are designed to provide greater interchange of PDFs including logical structure, providing a means to identify the custom
namespace for each element, if appropriate. However, structure elements types in undefined namespaces continue to be permitted.
<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/8">Issue #8</a></span></span></p>


<h4>14.8.6.2 Role maps and namespaces</h4>

<p>...</p>

<div class="new-text">
<p>EXAMPLE:</p>
<code>
17 0 obj<br/>
<<<br/>
&nbsp;&nbsp;&nbsp;&nbsp;/Type /StructElem<br/>
&nbsp;&nbsp;&nbsp;&nbsp;/S /section<br/>
&nbsp;&nbsp;&nbsp;&nbsp;/P 5 0 R<br/>
&nbsp;&nbsp;&nbsp;&nbsp;/NS 15 0 R<br/>
>><br/>
endobj<br/>
<br/>
15 0 obj<br/>
<<<br/>
&nbsp;&nbsp;&nbsp;&nbsp;/Type /Namespace<br/>
&nbsp;&nbsp;&nbsp;&nbsp;/NS (urn:uuid:A63861E-9F7-4FCB-9B27-C3BC8D9BFB06)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;/RoleMapNS 16 0 R<br/>
>><br/>
endobj<br/>
<br/>
16 0 obj<br/>
<< <br/>
&nbsp;&nbsp;&nbsp;&nbsp;/section [/H1 11 0 R]<br/>
&nbsp;&nbsp;&nbsp;&nbsp;...<br/>
>><br/>
endobj<br/>
</code>
<span class="new-tooltiptext">Issue #65</span>
</div>


<h4>14.8.6.3 Other namespaces</h4>

<p>...</p>

<p>NOTE 1 MathML is the only domain-specific namespace defined in PDF 2.0.</p>

<p>
<span class="deleted-text">When including mathematics structured as MathML 3.0, the math structure element type as defined in MathML 3.0 shall be used, and shall have its namespace explicitly defined (see 14.7.4.2, "Namespace dictionary").<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/72">Issue #72</a></span></span>
<span class="new-text">When including mathematics structured as MathML 3.0, the <b>math</b> structure element type, as defined in MathML 3.0, shall be used to enclose the formula under the <b>Formula</b> structure element type. All MathML structure element types and their attributes shall have the MathML 3.0 namespace explicitly defined (see 14.7.4.2, "Namespace dictionary").<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/72">Issue #72</a></span></span>
</p>

<p>...</p>


<h4>14.12.4.2 Document part metadata</h4>

<p>...</p>

<p>
The values of keys present in the DPM dictionary, or of any dictionary or array object present in the DPM dictionary, shall only be of type text string, date string,
<span class="new-text">name,<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/86">Issue #86</a></span></span>
array, dictionary, boolean, integer or real as defined in 7.3, "Objects".
<span class="new-text">All key values that are PDF name objects, after expansion of character sequences escaped with a NUMBER SIGN (23h), if any, shall be valid UTF-8 character sequences.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/86">Issue #86</a></span></span>
Other PDF value types shall not be used.
</p>


<h3>14.13.5 Associated files linked to graphics objects</h3>


<p>...</p>

<p>
The property list associated with the marked-content shall specify an array of file specification dictionaries to which
the content is associated. The named resource in the <span class="deleted-text"><b>Property List</b><span class="deleted-tooltiptext">
Issue #14</span></span> <span class="new-text"><i>property list</i><span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14">Issue #14</a></span></span>
(see 14.6.2, "Property lists") shall specify an array of file specification dictionaries to which the content is associated.
The relationship that the associated files have to the PDF content is supplied by the AFRelationship key in each file specification dictionary.
</p>

<p>...</p>


</div>


<hr>
<p class="footnote">Last modified: 30 July 2021</p>
