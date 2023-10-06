---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 14
title: Document interchange
modified: 6 October 2023
---

<ul class="noprint">
 <li>14.3 Metadata
  <ul>
   <li><a href="#H14.3.2">14.3.2 Metadata streams</a>
   </li>
  </ul>
 </li>
 <li><a href="#H14.5">14.5 Page-piece dictionaries</a>
 </li>
 <li>14.6 Marked content
  <ul>
   <li><a href="#H14.6.1">14.6.1 General</a>
   </li>
  </ul>
 </li>
 <li>14.7 Logical structure
  <ul>
   <li><a href="#H14.7.2">14.7.2 Structure hierarchy</a>
   </li>
   <li><a href="#H14.7.3">14.7.3 Structure types</a>
   </li>
   <li>14.7.5 Structure content
    <ul>
     <li><a href="#H14.7.5.3">14.7.5.3 PDF objects as content items</a>
     </li>
    </ul>
   </li>
   <li>14.7.6 Structure attributes
    <ul>
     <li><a href="#H14.7.6.1">14.7.6.1 General</a>
     </li>
     <li><a href="#H14.7.6.2">14.7.6.2 Attribute classes</a>
     </li>
    </ul>
   </li>
  </ul>
 </li>
 <li>14.8 Tagged PDF
  <ul>
   <li>14.8.3 Basic layout model
    <ul>
     <li><a href="#H14.8.3.3">14.8.3.3 Progression direction</a>
     </li>
    </ul>
   </li>
   <li>14.8.4 Standard structure types
    <ul>
     <li><a href="#H14.8.4.4">14.8.4.4 Grouping level structure types</a>
     </li>
     <li>14.8.4.7 Inline level structure types
      <ul>
       <li><a href="#H14.8.4.7.2">14.8.4.7.2 General inline level structure types</a>
       </li>
       <li><a href="#H14.8.4.7.3"><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">14.8.4.7.3 Link elements</ins></a>
       </li>
       <li><a href="#H14.8.4.7.4">14.8.4.7.<del onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">3</del><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">4</ins> Ruby and warichu elements</a>
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
   <li>14.8.5 Standard structure attributes
    <ul>
     <li><a href="#H14.8.5.1">14.8.5.1 General</a>
     </li>
     <li><a href="#H14.8.5.2">14.8.5.2 Standard <ins onMouseEnter="mouseEnter(this)" data-issue="224" data-iso="submitted">structure</ins> attribute owners</a>
     </li>
     <li><a href="#H14.8.5.3">14.8.5.3 Attribute values and inheritance</a>
     </li>
     <li>14.8.5.4 Layout attributes
      <ul>
       <li><a href="#H14.8.5.4.1">14.8.5.4.1 General</a>
       </li>
       <li><a href="#H14.8.5.4.2">14.8.5.4.2 General layout attributes</a>
       </li>
       <li><a href="#H14.8.5.4.4">14.8.5.4.4 Layout Attributes for ILSEs</a>
       </li>
      </ul>
     </li>
     <li><a href="#H14.8.5.5">14.8.5.5 List attributes</a>
     </li>
     <li><a href="#H14.8.5.8">14.8.5.8 Artifact attributes</a>
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
 <li>14.9 Repurposing and accessibility support
  <ul>
   <li>><a href="#H14.9.4">14.9.4 Replacement text</a>
   </li>
  </ul>
 </li>
 <li>14.10 Web capture
  <ul>
   <li>14.10.5 Source information
    <ul>
     <li><a href="#H14.10.5.3">14.10.5.3 Command dictionaries</a>
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

<h2 id="H14.3">14.3 Metadata</h2>

<h3 id="H14.3.2">14.3.2 Metadata streams</h3>

<p class="location">Change the paragraph below Table 347 as follows:</p>

<p>
The contents of a metadata stream shall be the metadata represented in Extensible Markup Language (XML) and the grammar of the XML representing the metadata shall be defined according to the extensible metadata platform specification (ISO 16684-1). 
<ins onMouseEnter="mouseEnter(this)" data-issue="296">All XMP metadata in PDF shall be encoded as UTF-8.</ins>
</p>


<h2 id="H14.5">14.5 Page-piece dictionaries</h2>

<p class="location">Change the paragraph above Table 350 as follows:</p>

<p>
As "Table 350 - Entries in a page-piece dictionary" shows, a page-piece dictionary may contain any number of entries,
each <del onMouseEnter="mouseEnter(this)" data-issue="69" data-iso="approved">keyed by</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="69" data-iso="approved">key should be a second-class name, or</ins>
the name of a distinct PDF processor, or of a well-known data type recognised by a family of PDF processors.
The value associated with each key shall be a data dictionary containing the private data that shall be used by the PDF processor.
The <b>Private</b> entry may have a value of any data type, but typically it is a dictionary containing all of the private
data needed by the PDF processor other than the actual content of the document, page, or form.
</p>

<p class="location">Change Table 350 as follows:</p>

<table>
  <caption id="Table350">Table 350 - Entries in a page-piece dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td>any valid second-class name <ins onMouseEnter="mouseEnter(this)" data-issue="69" data-iso="approved">(<i>recommended</i>), any conforming product name or well known data type</ins></td>
    <td>dictionary</td>
    <td>A data dictionary (see "Table 351 - Entries in a data dictionary").
    </td>
  </tr>
</table>

<p class="location">Insert new NOTE below Table 350 as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="69" data-iso="approved">NOTE: the definition of page-piece dictionary keys was updated to also support the same definition as in ISO 32000-1:2008 to allow easier document upgrades to PDF 2.0, however second-class names are strongly recommend.</ins>
</p>

<h2 id="H14.6">14.6 Marked content</h2>

<h3 id="H14.6.1">14.6.1 General</h3>

<p class="location">Delete NOTE 1 as follows:</p>

<p class="hangingindent">
<del onMouseEnter="mouseEnter(this)" data-issue="303">NOTE 1 This is a sequence not simply of bytes in the content stream but of complete graphics objects. Each object is fully qualified by the parameters of the graphics state in which it is rendered.</del>
</p>

<p class="editornote">EDITOR NOTE: notes in subclause 14.6.1 will be renumbered.</p>

<p>...</p>

<p class="location">Change NOTE 3 as follows:</p>

<p class="hangingindent">
NOTE 3 The tag operand of marked-content operators have no relationship to Tagged PDF (see 14.8 "Tagged PDF") and thus is not 
<del onMouseEnter="mouseEnter(this)" data-issue="126" data-iso="approved">rolemapped</del><ins onMouseEnter="mouseEnter(this)" data-issue="126" data-iso="approved">role mapped</ins>.
</p>

<p>...</p>

<p class="location">Change Table 352 as follows:</p>

<table>
  <caption id="Table352">Table 352 -Marked content operators</caption>
  <tr>
    <th>Operands</th>
    <th>Operator</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><del onMouseEnter="mouseEnter(this)" data-issue="301"><i>Tag</i></del><ins onMouseEnter="mouseEnter(this)" data-issue="301"><i>tag</i></ins></td>
    <td><b>BMC</b></td>
    <td>Begin a marked-content sequence terminated by a balancing <b>EMC</b> operator. <i>tag</i> shall be a name object indicating the role or significance of the sequence.</td>
  </tr>
</table>



<p class="location">Change the paragraph below Table 352 as follows:</p>

<p>
When the marked-content operators <b>BMC</b>, <b>BDC</b>, and <b>EMC</b> are combined with the text object operators <b>BT</b> and <b>ET</b>
(see 9.4, "Text objects")
<ins onMouseEnter="mouseEnter(this)" data-issue="302">; the compatibility operators <b>BX</b> and <b>EX</b> (see "Table 33 - Compatibility operators");
or the graphics state save and restore operators <b>q</b> and <b>Q</b> (see "Table 56 - Graphics state operators")</ins>, each pair of matching
operators (<b>BMC</b>…<b>EMC</b>, <b>BDC</b>…<b>EMC</b>, <del onMouseEnter="mouseEnter(this)" data-issue="302">or </del><b>BT</b>…<b>ET</b><ins onMouseEnter="mouseEnter(this)" data-issue="302">, <b>BX</b>…<b>EX</b> or <b>q</b>…<b>Q</b></ins>) shall be properly (separately) nested. ...
</p>


<h2 id="H14.7">14.7 Logical structure</h2>

<h3 id="H14.7.2">14.7.2 Structure hierarchy</h3>

<p class="location">Change Table 355 as follows:</p>

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
    <td>(<i>Optional<ins onMouseEnter="mouseEnter(this)" data-issue="93" data-iso="approved">; deprecated in PDF 2.0</ins></i>) The current revision number of this structure element (see 14.7.6.3, "Attribute revision numbers"). The value shall be a non-negative integer. Default value: 0.
    </td>
  </tr>
</table>

<h3 id="H14.7.3">14.7.3 Structure types</h3>

<p class="location">Change the third paragraph as follows:</p>

<p>
The <b>RoleMap</b> dictionary shall be comprised of a set of keys representing structure element types <del onMouseEnter="mouseEnter(this)" data-issue="126" data-iso="approved">rolemapped</del><ins onMouseEnter="mouseEnter(this)" data-issue="126" data-iso="approved">role mapped</ins> to other structure element types. The corresponding value for each of these keys shall be a single name identifying the target structure element type.
</p>

<p>...</p>


<h3 id="H14.7.5">14.7.5 Structure content</h3>

<h4 id="H14.7.5.3">14.7.5.3 PDF objects as content items</h4>

<p class="location">Change Table 358 as follows:</p>

<table>
  <caption id="Table358">Table 358 - Entries in an object reference dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Pg</b></td>
    <td>Dictionary</td>
    <td>
      <i>(Optional; shall be an indirect reference)</i> The page object of the page on which the object shall be rendered. This entry overrides any <b>Pg</b> entry in the structure element containing the object reference; it shall be 
      <del onMouseEnter="mouseEnter(this)" data-issue="339">used</del>
      <ins onMouseEnter="mouseEnter(this)" data-issue="339">required</ins> 
      if the structure element has no such entry.
    </td>
  </tr>
</table>

<h3 id="H14.7.6">14.7.6 Structure attributes</h3>

<h4 id="H14.7.6.1">14.7.6.1 General</h4>

<p class="location">Change the first paragraph as follows:</p>

<p>
A PDF processor that processes logical structure may attach additional information, called attributes, to any structure element. The attribute
information shall be held in one or more attribute objects associated with the structure element. An attribute object shall be a dictionary or
stream that includes an <b>O</b> entry (see "Table 360 — Entries common to all attribute object dictionaries") identifying the
<del onMouseEnter="mouseEnter(this)" data-issue="354">conforming product that owns</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="354">owner of</ins> the attribute information. 
Other entries, except the <b>NS</b> entry, shall represent the attributes: the keys shall be attribute names, and values shall be the corresponding
attribute values. To facilitate the interchange of content among conforming products, PDF defines a set of standard structure attributes identified
by specific standard owners; see 14.8.5, "Standard structure attributes". In addition, attributes may be used to represent user properties (see 
14.7.6.4, "User properties").
</p>

<p class="location">Change Table 360 as follows:</p>

<table>
  <caption id="Table360">Table 360- Entries common to all attribute object dictionaries</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>O</b></td>
    <td>name</td>
    <td>
    (<i>Required</i>) The name of the 
    <del onMouseEnter="mouseEnter(this)" data-issue="354">PDF processor creating</del> 
    <ins onMouseEnter="mouseEnter(this)" data-issue="354">owner of</ins> 
    the attribute data. The value shall either be 
    <del onMouseEnter="mouseEnter(this)" data-issue="354">a</del> <i>NSO</i>, <i>UserProperties</i> (see "Table 361 — Additional entries in an attribute object dictionary for user properties"), one of the values from 14.8.5, "Standard structure attributes", or conform to the guidelines described in Annex E, "Extending PDF".
    <p>If the value for the <b>O</b> entry is <i>NSO</i> then the <b>NS</b> entry shall be present, and shall identify the owner of the attribute object.</p>
    </td>
  </tr>
</table>


<h4 id="H14.7.6.2">14.7.6.2 Attribute classes</h4>

<p class="location">Change the last paragraph as follows:</p>

<p>
The <b>C</b> entry in a structure element dictionary (see "Table 355 — Entries in a structure element dictionary") shall contain a class name or
an array of class names 
(<del onMouseEnter="mouseEnter(this)" data-issue="305">typically</del><ins onMouseEnter="mouseEnter(this)" data-issue="305">possibly</ins> accompanied by revision numbers as well <ins onMouseEnter="mouseEnter(this)" data-issue="305"></i>(deprecated in PDF 2.0)</i></ins>; see 14.7.6.3, "Attribute revision numbers"). For each class named in
the <b>C</b> entry, the corresponding attribute object or objects shall be considered to be attached to the given structure element, along with
those identified in the element’s <b>A</b> entry. 
<ins onMouseEnter="mouseEnter(this)" data-issue="289">Attribute objects included through a class and through an array of classes within the <b>C</b>
entry may have the value of <b>O</b> and <b>NS</b> repeated. If a given attribute is specified more than once across the attribute objects, the later
(in array order) shall take precedence.</ins>
If both the <b>A</b> and <b>C</b> entries are present and a given attribute is specified by both, the one specified by the <b>A</b> entry shall take precedence.
</p>

<p class="location">Add a new NOTE after the last paragraph as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="254">NOTE If a class identified through the <b>C</b> entry is not present in the <b>ClassMap</b>, 
it is an empty class, which defines no additional attributes.</ins>
<p>

<h2 id="H14.8">14.8 Tagged PDF</h2>

<h2>14.8.3 Basic layout model</h2>

<h3 id="H14.8.3.3">14.8.3.3 Progression direction</h3>

<p class="location">Change first paragraph as follows:</p>

<p>
The meaning of the terms block-progression direction and inline-progression direction depends on the writing system in use, as specified by the standard <ins onMouseEnter="mouseEnter(this)" data-issue="224" data-iso="submitted">structure</ins> attribute <b>WritingMode</b> (see 14.8.5.4.2, "General Layout Attributes"). In Western writing systems, the block direction is from top to bottom and the inline direction is from left to right. Other writing systems use different directions for laying out content.
</p>

<p>...</p>

<h3 id="H14.8.4">14.8.4 Standard structure types</h3>

<h4 id="H14.8.4.4">14.8.4.4 Grouping level structure types</h4>

<p class="location">Change Table 365 as follows:</p>

<table>
  <caption id="Table365">Table 365 - Grouping level structure types</caption>
  <tr>
    <th>Structure Type</th>
    <th>Category</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><b>Part</b></td>
    <td>Grouping</td>
    <td>
    <p>Encloses a grouping of structure elements without consideration for their hierarchy.</p>
    <p class="hangingindent">
    NOTE 1 <del onMouseEnter="mouseEnter(this)" data-issue="141" data-iso="submitted"><b>Part</b> is the semantic equivalent of <b>Div</b></del> <ins onMouseEnter="mouseEnter(this)" data-issue="141" data-iso="submitted">The non-hierarchical aspect of <b>Part</b> is similar to <b>Div</b>. However, unlike <b>Div</b>, the grouping of elements enclosed in a <b>Part</b> structure element has semantic value</ins>.
    </p>
    <p>A structure element with the type of <b>Part</b> shall inherit the containment requirements and limitations of its parent element. Where the parent element is itself a structure element of type <b>Part</b>, then the inheritance shall recurse to the first parent element whose type is not <b>Part</b>.</p>
    <p class="hangingindent">
    <ins onMouseEnter="mouseEnter(this)" data-issue="141" data-iso="submitted">NOTE 2 The semantic value of a structure element of type <b>Part</b> is determined by the elements enclosed within, in addition to the grouping nature of <b>Part</b>.</ins>
    </p>
    <p>...</p>
    </td>
  </tr>
</table>

<h4 id="H14.8.4.7">14.8.4.7 Inline level structure types</h4>

<h5 id="H14.8.4.7.2">14.8.4.7.2 General inline level structure types</h5>

<p class="location">Change Table 368 as follows:</p>

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
    that <del onMouseEnter="mouseEnter(this)" data-issue="84" data-iso="approved">the user is intended to read first</del>
    <ins onMouseEnter="mouseEnter(this)" data-issue="84" data-iso="approved">is more important</ins>:
    </p>
    <p>...</p>
    </td>
  </tr>
</table>

<p class="location">Insert a new clause heading below NOTE 1 and modify text as follows:</p>

<h5 id="H14.8.4.7.3"><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">14.8.4.7.3 Link elements</ins></h5>

<p>Tagged PDF link elements (standard structure type Link) use PDF's logical structure facilities to establish the association between content items and link annotations, providing functionality comparable to HTML hypertext links. The following items may be children of a link element:</p>

<ul>
<li>One or more content items or other ILSEs (except other links) <del onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">if <b>A</b>, <b>Dest</b> and <b>PA</b> keys of all of them have identical values</del></li>
<li>Object references (see 14.7.5.3, "PDF objects as content items") to one <ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">or more</ins> link <del onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">annotation</del> <ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">annotations</ins> associated with the content</li>
</ul>

<p class="hangingindent">NOTE <del onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">2</del><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">1</ins> An <b>SD</b> entry in the <b>GoTo</b> or <b>GoToR</b> action in a <b>Link</b> annotation facilitates linking directly to a target structure element as opposed to just targeting an area on a page.</p>

<p><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">
When a <b>Link</b> structure element describes a span of text to be associated with a link annotation and that span
wraps from the end of one line to the beginning of another, the <b>Link</b> structure element shall include a single
object reference that associates the span with the associated link annotation. Further, the link annotation shall
use the <b>QuadPoint</b> entry to denote the active areas on the page.</ins></p>

<p><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">
EXAMPLE 1 The <b>Link</b> structure element references a link annotation that includes a <b>QuadPoint</b> entry that boxes the
strings "with a" and "link". That is, the <b>QuadPoint</b> entry contains 16 numbers: the first 8 numbers describe
a quadrilateral for "with a", and the next 8 describe a quadrilateral for "link".
</ins></p>

<p style="padding-left:40px;"><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">
Here is some text <span style="color:blue;text-decoration:underline;">with a</span><br/>
<span style="color:blue;text-decoration:underline;">link</span> inside.
</ins></p>

<p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">
NOTE 2 Beginning with PDF 1.7, use of the <b>Link</b> structure element to enclose multiple link annotations on a single page is deprecated.
</ins></p>

<p><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">EXAMPLE 2 Consider the following fragment of HTML code, which produces a line of text containing a hypertext link:</ins></p>

<div><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">
<code>&lt;html&gt;
    &lt;body&gt;
        &lt;p&gt;
            Here is some text &lt;a href="https://www.pdfa.org"&gt;with a link&lt;/a&gt; inside.
        &lt;/p&gt;
    &lt;/body&gt;
&lt;/html&gt;
</code></ins></div>

<br/>
<p><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">This code sample shows an equivalent fragment of PDF using a link element, whose text it displays in blue and underlined.</ins></p>

<div><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">
<code>/P &lt;&lt; /MCID 0 &gt;&gt;                     % Marked-content sequence 0 (paragraph)
  BDC                                % Begin marked-content sequence
    BT                               % Begin text object
      /T1_0 1 Tf                     % Set text font and size
      14 0 0 14 10.000 753.976 Tm    % Set text matrix
      0.0 0.0 0.0 rg                 % Set nonstroking colour to black
      (Here is some text ) Tj        % Show text preceding link
    ET                               % End text object
  EMC                                % End marked-content sequence

/Link &lt;&lt; /MCID 1 &gt;&gt;                  % Marked-content sequence 1 (link)
  BDC                                % Begin marked-content sequence
    0.7 w                            % Set line width
    [ ] 0 d                          % Solid dash pattern
    111.094 751.8587 m               % Move to beginning of underline
    174.486 751.8587 l               % Draw underline
    0.0 0.0 1.0 RG                   % Set stroking colour to blue
    S                                % Stroke underline
    BT                               % Begin text object
      14 0 0 14 111.094 753.976 Tm   % Set text matrix
      0.0 0.0 1.0 rg                 % Set nonstroking colour to blue
      (with a link) Tj               % Show text of link
    ET                               % End text object
  EMC                                % End marked-content sequence

/P &lt;&lt; /MCID 2 &gt;&gt;                     % Marked-content sequence 2 (paragraph)
  BDC                                % Begin marked-content sequence
    BT                               % Begin text object
      14 0 0 14 174.486 753.976 Tm   % Set text matrix
      0.0 0.0 0.0 rg                 % Set nonstroking colour to black
      ( inside.) Tj                  % Show text following link
    ET                               % End text object
  EMC                                % End marked-content sequence
</code></ins></div>

<br/>
<p><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">EXAMPLE 3 This example shows an excerpt from the associated logical structure hierarchy.</ins></p>

<div><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">
<code>501 0 obj              % Structure element for paragraph
&lt;&lt;  /Type /StructElem
    /S /P
    ...
    /K [ 0             % Three children: marked-content sequence 0
         502 0 R       % Link
         2             % Marked-content sequence 2
    ]
&gt;&gt;
endobj

502 0 obj              % Structure element for link
&lt;&lt;  /Type /StructElem
    /S /Link
    ...
    /K [ 1             % Two children: marked-content sequence 1
         503 0 R       % Object reference to link annotation
    ]
&gt;&gt;
endobj

503 0 obj              % Object reference to link annotation
&lt;&lt;  /Type /OBJR
    /Obj 600 0 R       % Link annotation (not shown)
&gt;&gt;
endobj
</code></ins></div>
<br/>

<h5 id="H14.8.4.7.4">14.8.4.7.<del onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">3</del><ins onMouseEnter="mouseEnter(this)" data-issue="133" data-iso="submitted">4</ins> Ruby and warichu elements</h5>

<p class="editornote">EDITOR NOTE: Clause is renumbered - existing text is unchanged.</p>


<h5 id="H14.8.4.8.3">14.8.4.8.3 Table structure types</h5>

<p class="location">Change Table 371 as follows:</p>

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
    A row of table header cells (<b>TH</b>) or table data cells (<b>TD</b>)<ins onMouseEnter="mouseEnter(this)" data-issue="45,71" data-iso="approved,approved"> or both</ins> in a table.
    </td>
  </tr>
</table>


<h5 id="H14.8.4.8.4">14.8.4.8.4 Caption structure types</h5>

<p class="location">Change Table 372 as follows:</p>

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
    <p class="hangingindent">NOTE <ins onMouseEnter="mouseEnter(this)" data-issue="35" data-iso="approved">1</ins> In principle, captions can appear in a nested fashion. For example, several smaller images belonging to a group of images can each
    be accompanied by a caption, and the group of these images as a whole is accompanied by a caption as well.</p>
    <p class="hangingindent">
    <ins onMouseEnter="mouseEnter(this)" data-issue="35" data-iso="approved">NOTE 2 If an <b>Artifact</b> structure element is present, and needs to be associated with a <b>Caption</b>, then the <b>Artifact</b> structure element needs to be a descendent of the <b>Caption</b>.</ins>
    </p>
    </td>
  </tr>
</table>


<h3 id="H14.8.5">14.8.5 Standard structure attributes</h3>

<h4 id="H14.8.5.1">14.8.5.1 General</h4>

<p class="location">Change reference to subclause 14.8.5.2 in sixth paragraph as follows:</p>

<p>
In addition to the standard structure attributes described in 14.8.5.2, "Standard <ins onMouseEnter="mouseEnter(this)" data-issue="224" data-iso="submitted">structure</ins> attribute owners" there are several other optional entries – <b>Lang</b>, <b>Alt</b>, <b>ActualText</b>, and <b>E</b> – that are described in 14.9, "Repurposing and accessibility support" but are useful to other PDF consumers as well. They appear in the following places in a PDF file (rather than in attribute dictionaries):
</p>

<ul>
  <li>...</li>
</ul>

<p class="location">Change title of subclause 14.8.5.2 as follows:</p>

<h4 id="H14.8.5.2">14.8.5.2 Standard <ins onMouseEnter="mouseEnter(this)" data-issue="224" data-iso="submitted">structure</ins> attribute owners</h4>

<p class="location">Change first paragraph as follows:</p>

<p>
Each attribute object has an owner, specified by the object's <b>O</b> entry, or, if the value of <b>O</b> is <i>NSO</i>, by the object’s <b>NS</b> entry, which determines the interpretation of the attributes defined in the object's dictionary. Multiple owners may define like-named attributes with different value types or interpretations. Tagged PDF defines a set of standard <ins onMouseEnter="mouseEnter(this)" data-issue="224" data-iso="submitted">structure</ins> attribute owners as shown in "Table 376 — Standard structure attribute owners".
</p>

<p>...</p>

<p class="location">Change Table 376 as follows:</p>

<table>
  <caption id="Table376">Table 376 - Standard structure attribute owners</caption>
  <tr>
    <th>Owner value for the attribute object’s O entry</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><b>CSS-1</b></td>
    <td>Additional attributes governing translation to a format using CSS, <del onMouseEnter="mouseEnter(this)" data-issue="357">version</del><ins onMouseEnter="mouseEnter(this)" data-issue="357">level</ins> 1</td>
  </tr>
  <tr>
    <td><b>CSS-2</b></td>
    <td>Additional attributes governing translation to a format using CSS, <del onMouseEnter="mouseEnter(this)" data-issue="357">version 2.1</del><ins onMouseEnter="mouseEnter(this)" data-issue="357">level 2, revision 1</ins></td>
  </tr>
  <tr>
    <td><b>CSS-3</b></td>
    <td>Additional attributes governing translation to a format using CSS, <del onMouseEnter="mouseEnter(this)" data-issue="357">version</del><ins onMouseEnter="mouseEnter(this)" data-issue="357">level</ins> 3</td>
  </tr>
</table>


<p class="location">Add a new NOTE after the current note below Table 376 as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="286">NOTE The attribute owner, defined through the <b>O</b> and <b>NS</b> entries in the attribute object, define an owner for each attribute, but do not provide information on transformation of those attributes into other formats. When considering formats such as HTML and MathML, attributes would be transformed to meet the syntactic requirements of those formats.</ins>
<p>

<p>...</p>

<h4 id="H14.8.5.3">14.8.5.3 Attribute values and inheritance</h4>

<p>...</p>

<p class="location">Change NOTE 1 as follows:</p>

<p class="hangingindent">
NOTE 1 The description of each of the standard <ins onMouseEnter="mouseEnter(this)" data-issue="224" data-iso="submitted">structure</ins> attributes in this subclause specifies whether their values are inheritable
</p>

<p>...</p>

<h4 id="H14.8.5.4">14.8.5.4 Layout attributes</h4>

<h5 id="H14.8.5.4.1">14.8.5.4.1 General</h5>

<p class="location">Change Table 377 as follows:</p>

<table>
  <caption id="Table377">Table 377 - Standard layout attributes</caption>
  <tr>
    <th>Structure Elements</th>
    <th>Attributes</th>
    <th>Inheritable</th>
  </tr>
  <tr>
    <td><b><del onMouseEnter="mouseEnter(this)" data-issue="223" data-iso="submitted">Vertical text</del>
        <ins onMouseEnter="mouseEnter(this)" data-issue="223" data-iso="submitted">Any structure element containing text whose inline-progression direction is top to bottom or bottom to top.</ins>
    </b></td>
    <td>...</td>
    <td>...</td>
  </tr>
  <tr>
    <td><b><ins onMouseEnter="mouseEnter(this)" data-issue="223" data-iso="submitted">RB, RT, EP (</ins>Ruby text<ins onMouseEnter="mouseEnter(this)" data-issue="223" data-iso="submitted">)</ins>
    </b></td>
    <td>...</td>
    <td>...</td>
  </tr>
</table>

<p>...</p>

<h5 id="H14.8.5.4.2">14.8.5.4.2 General layout attributes</h5>

<p class="location">Change Table 378 as follows:</p>

<table>
  <caption id="Table378">Table 378 - Standard layout attributes common to all standard structure types</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Placement</b></td>
    <td>name</td>
    <td>
    <p>
     (<i>Optional; not inheritable</i>) The positioning of the element with respect to the enclosing reference area and other content
     <ins onMouseEnter="mouseEnter(this)" data-issue="189" data-iso="submitted">(see 14.8.3.3, "Progression direction")</ins>. The value shall be one of the following:
    </p>
    <p>...</p>
    <p>Default value: <i>Block</i> for BLSEs, <i>Inline</i> for ILSEs.</p>
    <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="188" data-iso="submitted">
    NOTE The default value depends on the context in which the structure element is used (see 14.8.4.1, "General").
    </ins></p>
    <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="188" data-iso="submitted">
    EXAMPLE 1 A <b>Figure</b> structure element occurring within a <b>P</b> structure element is an ILSE, and therefore has a default value of <i>Inline</i>.
    </ins></p>
    <p class="hangingindent"><ins onMouseEnter="mouseEnter(this)" data-issue="188" data-iso="submitted">
    EXAMPLE 2 A <b>Figure</b> structure element occurring within a <b>Sect</b> structure element is an BLSE, and therefore has a default value of <i>Block</i>.
    </ins></p>
    </td>
  </tr>
  <tr>
    <td><b>WritingMode</b></td>
    <td>name</td>
    <td>
     <p>
     (<i>Optional; inheritable</i>) Indicates the directions of layout progression inside Block Level Structure Elements (BLSEs) (inline progression)
     and regarding the sequence of BLSEs (block progression)
     <ins onMouseEnter="mouseEnter(this)" data-issue="189" data-iso="submitted">(see 14.8.3.3, "Progression direction")</ins>.
     <b>WritingMode</b> may be used as an attribute for any structure element. The value shall be one of the following:
     </p>
     <p>...</p>
    </td>
  </tr>
</table>


<h5 id="H14.8.5.4.4">14.8.5.4.4 Layout Attributes for ILSEs</h5>

<p class="location">Change Table 380 as follows:</p>

<table>
  <caption id="Table380">Table 380 - Standard layout attributes specific to inline-level structure elements</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>GlyphOrientationVertical</b></td>
    <td><del onMouseEnter="mouseEnter(this)" data-issue="152" data-iso="submitted">number</del><ins onMouseEnter="mouseEnter(this)" data-issue="152" data-iso="submitted">integer</ins> or name</td>
    <td>
    <p>...</p>
    </td>
  </tr>
</table>

<h4 id="H14.8.5.5">14.8.5.5 List attributes</h4>

<p class="location">Change Table 382 as follows:</p>

<table>
  <caption id="Table382">Table 382 - Standard list attributes</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>ContinuedList</b></td>
    <td>boolean</td>
    <td>
    (<i>Optional; <ins onMouseEnter="mouseEnter(this)" data-issue="346">not inheritable;</ins> PDF 2.0</i>) ...
    </td>
  </tr>
  <tr>
    <td><b>ContinuedFrom</b></td>
    <td>ID (byte string)</td>
    <td>
    (<i>Optional; <ins onMouseEnter="mouseEnter(this)" data-issue="346">not inheritable;</ins> PDF 2.0</i>) ...
    </td>
  </tr>
</table>


<h4 id="H14.8.5.8">14.8.5.8 Attribute attributes</h4>

<p class="location">Change Table 385 as follows:</p>

<table>
  <caption id="Table385">Table 385 - Standard artifact attributes</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Type</b></td>
    <td>name</td>
    <td>
    (<i>Optional; <ins onMouseEnter="mouseEnter(this)" data-issue="347">not inheritable; PDF 2.0</ins></i>) ...
    </td>
  </tr>
  <tr>
    <td><b>BBox</b></td>
    <td>rectangle</td>
    <td>
    (<i>Optional; <ins onMouseEnter="mouseEnter(this)" data-issue="347">not inheritable; PDF 2.0</ins></i>) ...
    </td>
  </tr>
  <tr>
    <td><b>Subtype</b></td>
    <td>name</td>
    <td>
    (<i>Optional; <del onMouseEnter="mouseEnter(this)" data-issue="347">PDF 1.7</del><ins onMouseEnter="mouseEnter(this)" data-issue="347">not inheritable; PDF 2.0</ins></i>) ...
    </td>
  </tr>
</table>

<p class="location">Insert a new NOTE below Table 385 as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="347">NOTE: the meaning of the keys <b>Type</b> and <b>Subtype</b> in "Table 382 - Standard artifact attributes" do not follow the documented conventions described in 7.3.7, "Dictionary objects". This is due to alignment of "Table 382 - Standard artifact attributes" (<i>PDF 2.0</i>) with the previously existing "Table 363 - Property list entries for artifacts".</ins>
</p>



<h3 id="H14.8.6">14.8.6 Standard structure namespaces</h3>

<h4 id="H14.8.6.1">14.8.6.1 Namespaces for standard structure types and attributes</h4>

<p class="location">Modify the paragraph above the current NOTE as follows:</p>

<p>
To facilitate conversion of documents created against versions of the PDF standard earlier than PDF 2.0, the
<i>default standard structure namespace</i> shall be "http://iso.org/pdf/ssn".
<del onMouseEnter="mouseEnter(this)" data-issue="151" data-iso="approved">When a namespace is not explicitly specified for a given structure element or attribute, it shall be assumed to be within this default standard structure namespace.</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="151" data-iso="approved">When a structure element does not have a specified namespace, after transitively applying any role map present (see 14.8.6.2, "Role maps and namespaces"), the final element type shall be considered to be within the default standard structure namespace and shall be one of the standard structure types defined in the default standard structure namespace.</ins>
</p>

<p class="location">Add a new NOTE 1 above the current NOTE as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="106" data-iso="approved">NOTE 1 The original structure type is still considered to be in an undefined namespace, which means it is exempt from restrictions on role mapping within the same namespace.</ins>
</p>

<p class="editornote">EDITOR NOTE: the current note is renumbered as NOTE 2.</p>

<p class="location">Insert a new NOTE 3 after the last paragraph as follows:</p>

<p>The term <i>standard structure namespaces</i> refers to either of the two namespaces defined above.</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="8" data-iso="approved">NOTE 3 Namespaces are designed to provide greater interchange of PDFs including logical structure, providing a means to identify the custom namespace for each element, if appropriate. However, structure elements types in undefined namespaces continue to be permitted. </ins>
</p>


<h4 id="H14.8.6.2">14.8.6.2 Role maps and namespaces</h4>

<p>...</p>

<p class="location">Modify the 2nd bullet in the bulleted list as follows:</p>

<p>In a tagged PDF, all structure elements shall be in at least one of the standard structure namespaces or in a namespace identified in 14.8.6.3, “Other namespaces”. An element shall be considered to be in one of these namespaces if:</p>

<ul>
<li>they directly identify one of these namespaces through their NS entry;</li>
<li>they are in the default standard structure namespace <ins onMouseEnter="mouseEnter(this)" data-issue="151" data-iso="approved">(after any role mapping)</ins>;</li>
<li>...</li>
</ul>

<p class="location">Insert a new EXAMPLE 1 at the end of the subclause as follows:</p>

<div><ins onMouseEnter="mouseEnter(this)" data-issue="65" data-iso="approved">
<p>EXAMPLE 1: use of namespaces</p>
<code>
17 0 obj
&lt;&lt;
   /Type /StructElem
   /S /section
   /P 5 0 R
   /NS 15 0 R
&gt;&gt;
endobj

15 0 obj
&lt;&lt;
   /Type /Namespace
   /NS (urn:uuid:A63861E-9F7-4FCB-9B27-C3BC8D9BFB06)
   /RoleMapNS 16 0 R
&gt;&gt;
endobj

16 0 obj
&lt;&lt;
   /section [/H1 11 0 R]
   ...
&gt;&gt;
endobj
</code></ins></div>

<p class="location">Insert a new EXAMPLE 2 at the end of the subclause as follows:</p>

<div><ins onMouseEnter="mouseEnter(this)" data-issue="151" data-iso="approved">
<p>EXAMPLE 2: Role mapping of structure elements with no explicitly identified namespace</p>
<code>
13 0 obj % A structure tree with a role map for elements within an undefined namespace
&lt;&lt;
   /Type /StructTreeRoot
   /RoleMap &lt;&lt; % The "Global" role map is applied to elements in an undefined namespace.
     /Foo /Bar % The element type "Foo" in an undefined namespace maps to "Bar".
     /Bar /P   % The "Bar" element in an undefined namespace maps to P, which is defined in
               % the default standard structure namespace. This means that elements of
               % type "Foo" transitively map to "P" through the "Bar" element type.
   &gt;&gt;
   ...
&gt;&gt;
endobj

14 0 obj % A structure element with an undefined namespace of structure type "Foo"
&lt;&lt;
    /Type /StructElem % Structure Element with no defined namespace.
    /S /Foo           % The "Foo" element has an undefined namespace and isn't defined in either
                      % the PDF 1.7 or PDF 2.0 namespaces.
    ...
&gt;&gt;
endobj
</code></ins></div>

<h4 id="H14.8.6.3">14.8.6.3 Other namespaces</h4>

<p class="location">Replace the paragraph below NOTE 1 as follows:</p>

<p class="hangingindent">NOTE 1 MathML is the only domain-specific namespace defined in PDF 2.0.</p>

<p>
<del onMouseEnter="mouseEnter(this)" data-issue="72" data-iso="approved">When including mathematics structured as MathML 3.0, the math structure element type as defined in MathML 3.0 shall be used, and shall have its namespace explicitly defined (see 14.7.4.2, "Namespace dictionary").</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="72" data-iso="approved">When including mathematics structured as MathML 3.0, the <b>math</b> structure element type, as defined in MathML 3.0, shall be used to enclose the formula under the <b>Formula</b> structure element type. All MathML structure element types and their attributes shall have the MathML 3.0 namespace explicitly defined (see 14.7.4.2, "Namespace dictionary").</ins>
</p>

<p>...</p>

<h2 id="H14.9">14.9 Repurposing and accessibility support</h2>

<h3 id="H14.9.4">14.9.4 Replacement text</h3>

<p>...</p>

<p class="location">Correct the EXAMPLE as follows:</p>

<code class="hangingindent">
(Dru) Tj
/Span
    &lt;&lt;<del onMouseEnter="mouseEnter(this)" data-issue="356">/Actual Text</del><ins onMouseEnter="mouseEnter(this)" data-issue="356">/ActualText</ins> (c)&gt;&gt;
    BDC
        (k-) Tj
    EMC
(ker) '
</code>

<h2 id="H14.10">14.10 Web capture</h2>
<h3 id="H14.10.5">14.10.5 Source information</h3>
<h4 id="H14.10.5.3">14.10.5.3 Command dictionaries</h4>

<p class="location">Change Table 393 as follows:</p>

<table>
  <caption id="Table393">Table 393 - Entries in a Web Capture command dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>F</b></td>
    <td>integer</td>
    <td>
    <p>(<i>Optional</i>) A set of flags specifying various characteristics of the command (see
        <del onMouseEnter="mouseEnter(this)" data-issue="222" data-iso="submitted">"Table 393 - Entries in a Web Capture command dictionary"</del>
        <ins onMouseEnter="mouseEnter(this)" data-issue="222" data-iso="submitted">"Table 394 - Web Capture command flags"</ins>). Default value: 0.
    </p>
    </td>
  </tr>
</table>


<h2 id="H14.12">14.12 Document parts</h2>
<h3 id="H14.12.4">14.12.4 Data structures</h3>
<h4 id="H14.12.4.2">14.12.4.2 Document part metadata</h4>

<p class="location">Change the last paragraph as follows:</p>

<p>
The values of keys present in the DPM dictionary, or of any dictionary or array object present in the DPM dictionary, shall only be of type text string, date string,
<ins onMouseEnter="mouseEnter(this)" data-issue="86" data-iso="approved">name,</ins>
array, dictionary, boolean, integer or real as defined in 7.3, "Objects".
<ins onMouseEnter="mouseEnter(this)" data-issue="86" data-iso="approved">All key values that are PDF name objects, after expansion of character sequences escaped with a NUMBER SIGN (23h), if any, shall be valid UTF-8 character sequences.</ins>
Other PDF value types shall not be used.
</p>

<h2 id="H14.13">14.13 Associated files</h2>
<h3 id="H14.13.5">14.13.5 Associated files linked to graphics objects</h3>

<p class="location">Change the paragraph below NOTE 3 as follows:</p>

<p>
The property list associated with the marked-content shall specify an array of file specification dictionaries to which
the content is associated. The named resource in the
<del onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved"><b>Property List</b></del>
<ins onMouseEnter="mouseEnter(this)" data-issue="14" data-iso="approved"><i>property list</i></ins>
(see 14.6.2, "Property lists") shall specify an array of file specification dictionaries to which the content is associated.
The relationship that the associated files have to the PDF content is supplied by the AFRelationship key in each file specification dictionary.
</p>

<p>...</p>


</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
