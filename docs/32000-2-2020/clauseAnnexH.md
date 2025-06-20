---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: Annex H
title: (informative) Example PDF files
modified: 20 June 2025
---

<ul class="noprint">
  <li><a href="#HH.2">H.2 Minimal PDF file</a>
  </li>
  <li><a href="#HH.3">H.3 Simple text string example</a>
  </li>
  <li>H.7 Updating example
    <ul>
      <li><a href="#HH.7.5">H.7.5 Stage 4: Add three annotations and update metadata</a>
      </li>
    </ul>
  </li>
  <li>H.8 Structure elements examples
    <ul>
      <li><a href="#HH.8.2">H.8.2 Table of Contents</a>
      </li>
      <li><a href="#HH.8.3">H.8.3 Hierarchical lists</a>
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

<p class="editornote">EDITOR NOTE: as a result of <a href="https://github.com/pdf-association/pdf-issues/issues/415">Errata #415</a>, all occurrences of incorrect PDF content stream operator <del onMouseEnter="mouseEnter(this)" data-issue="415" data-iso="approved"><code>/BDC</code></del> need to replaced by <ins onMouseEnter="mouseEnter(this)" data-issue="415" data-iso="approved"><code>BDC</code></ins> (PDF content operators do not have leading SLASH) throughout Annex H.</p>

<h2 id="HH.2">H.2 Minimal PDF file</h2>

<p class="location">Change the example as follows:</p>

<code>...
            &lt;xmpMM:DocumentID&gt;… <del onMouseEnter="mouseEnter(this)" data-issue="402" data-iso="approved"><i>unique GUID of document</i></del> …&lt;/xmpMM:DocumentID&gt;
            &lt;xmpMM:InstanceID&gt;… <del onMouseEnter="mouseEnter(this)" data-issue="402" data-iso="approved"><i>GUID changed for each save</i></del> …&lt;/xmpMM:InstanceID&gt;
...

</code>

<h2 id="HH.3">H.3 Simple text string example</h2>

<p>...</p>

<p class="location">Correct the example as follows:</p>

<code>...
    %Underline "32000-2". Position must be calculated by generator
    %including scaled per-font underline vertical offset

    <ins onMouseEnter="mouseEnter(this)" data-issue="563">1.2 w                            %Set line width suitable for size of text</ins>
    133.3 694.2 m                    %Move to start of line position
    221.4 694.2 l                    %Set path to end of line position
    <del onMouseEnter="mouseEnter(this)" data-issue="563">1.2 w                            %Set line width suitable for size of text</del>
    S                                %Stroke path
...</code>

<p>...</p>

<h2 id="HH.7">H.7 Updating example</h2>

<h3 id="HH.7.5">H.7.5 Stage 4: Add three annotations and update metadata</h3>

<p class="location">Change the example as follows:</p>

<code>...
6 0 obj                                         %Metadata stream<del onMouseEnter="mouseEnter(this)" data-issue="402" data-iso="approved">s</del>
      &lt;&lt;/Type /Metadata
          /Subtype /XML
          /Length … <i>number of bytes in updated metadata</i> …
      &gt;&gt;
stream
<del onMouseEnter="mouseEnter(this)" data-issue="402" data-iso="approved">%In this Metadata, "preserved" items are left unaltered, and not updated to reflect possibly
%different software or a different author. Updating software needs to be able to parse the XMP
%in any valid format and preserve all content which is not to be updated, even that with
%unfamiliar tags. In this example some reordering of tags has taken place. Note further that
%after incremental update there can be multiple XMP packets
&lt;?xpacket begin="… <i>UTF-8 value of U+FEFF (efbbbf)</i> …" id="W5M0MpCehiHzreSzNTczkc9d"?&gt;
&lt;x:xmpmeta xmlns:x="adobe:ns:meta/"&gt;
&lt;rdf:RDF xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"&gt;
&lt;rdf:Description rdf:about="" xmlns:pdf="http://ns.adobe.com/pdf/1.3/"&gt;
&lt;pdf:Producer>… <i>name of software which generated the PDF (preserved)</i> …&lt;/pdf:Producer&gt;
&lt;/rdf:Description&gt;
&lt;rdf:Description rdf:about="" xmlns:dc="http://purl.org/dc/elements/1.1/"&gt;
&lt;dc:format&gt;application/pdf&lt;/dc:format&gt;
&lt;dc:title&gt;&lt;rdf:Alt&gt;
&lt;rdf:li xml:lang="x-default"&gt;… <i>document title (preserved)</i> …&lt;/rdf:li&gt;
&lt;/rdf:Alt&gt;&lt;/dc:title&gt;
&lt;dc:creator&gt;&lt;rdf:Seq&gt;
&lt;rdf:li&gt;… <i>document author’s personal name (preserved)</i> …&lt;/rdf:li&gt;
&lt;/rdf:Seq&gt;&lt;/dc:creator&gt;
&lt;/rdf:Description&gt;
&lt;rdf:Description rdf:about="" xmlns:xmpMM="http://ns.adobe.com/xap/1.0/mm/"&gt;
&lt;xmpMM:DocumentID>… unique GUID of document (preserved) …&lt;/xmpMM:DocumentID&gt;
&lt;xmpMM:InstanceID>… GUID changed for each save (updated) …&lt;/xmpMM:InstanceID&gt;
&lt;/rdf:Description&gt;
&lt;rdf:Description rdf:about="" xmlns:xmp="http://ns.adobe.com/xap/1.0/"&gt;
&lt;xmp:CreatorTool&gt;… <i>name of tool used to create the document (preserved)</i> …&lt;/xmp:CreatorTool&gt;
&lt;xmp:CreateDate&gt;… <i>timestamp, like 2012-12-25T12:34:56Z (preserved)</i> …&lt;/xmp:CreateDate&gt;
&lt;xmp:ModifyDate&gt;… <i>timestamp, like 2012-12-27T14:36:06Z (updated)</i> …&lt;/xmp:ModifyDate&gt;
&lt;/rdf:Description&gt;
&lt;/rdf:RDF&gt;
&lt;/x:xmpmeta&gt;
… <i>white-space padding to permit in-place updating of metadata</i> …
… <i>Note that applications which fully understand PDF updating do not usually update in-place</i> …
&lt;?xpacket end="w"?&gt;</del>
<ins onMouseEnter="mouseEnter(this)" data-issue="402" data-iso="approved">...</ins>
endstream
endobj
...

</code>

<h2 id="HH.8">H.8 Structure elements examples</h2>

<h3 id="HH.8.2">H.8.2 Table of Contents</h3>

<p class="location">Change the first paragraph as follows:</p>

<p>
The structure element’s structure type entry (<b>S</b>) may have values that establish hierarchical relationships between entries in a table of contents. The<b>TOCI</b> value specifies an individual member of a table of contents. The <b>TOC</b> value specifies a list made up of other table of contents items that are individual members of the table of contents and/or lists of table of contents items. (The trailing character in <b>TOCI</b> is an <del onMouseEnter="mouseEnter(this)" data-issue="75" data-iso="approved">upper case</del> <ins onMouseEnter="mouseEnter(this)" data-issue="75" data-iso="approved">uppercase</ins> "i".)
</p>

<p class="location">Insert a new NOTE after the first paragraph as follows:</p>

<p class="hangingindent">
<ins onMouseEnter="mouseEnter(this)" data-issue="62" data-iso="approved">NOTE the following example uses <b>Reference</b>, <b>TOC</b> and <b>TOCI</b> structure elements which are
part of the <i>standard structure namespace for PDF 1.7</i> and are entirely valid for use in PDF 2.0 under the <i>default standard structure namespace</i>
(see 14.8.6, "Standard structure namespaces").</ins>
</p>

<p>...</p>

<p class="location">Correct Figure H.5 as follows (page numbers are all vertically aligned):</p>

<p style="margin-left: 50px">TABLE OF CONTENTS</p>
<p style="margin-left: 80px">1. Chapter One<ins onMouseEnter="mouseEnter(this)" data-issue="419" data-iso="approved">.............</ins>3</p>
<p style="margin-left: 80px">&nbsp;&nbsp;&nbsp;&nbsp;1.<del onMouseEnter="mouseEnter(this)" data-issue="419" data-iso="approved">2</del><ins onMouseEnter="mouseEnter(this)" data-issue="419" data-iso="approved">1</ins> Section A<ins>.............</ins>4</p>
<p style="margin-left: 80px">&nbsp;&nbsp;&nbsp;&nbsp;1.<del onMouseEnter="mouseEnter(this)" data-issue="419" data-iso="approved">3</del><ins onMouseEnter="mouseEnter(this)" data-issue="419" data-iso="approved">2</ins> Section B<ins onMouseEnter="mouseEnter(this)" data-issue="419" data-iso="approved">.............</ins>5</p>
<p style="margin-left: 80px">2. Chapter Two<ins onMouseEnter="mouseEnter(this)" data-issue="419" data-iso="approved">.............</ins>6</p>
<p style="margin-left: 80px">3. Chapter <del onMouseEnter="mouseEnter(this)" data-issue="419" data-iso="approved">Two</del><ins onMouseEnter="mouseEnter(this)" data-issue="419" data-iso="approved">Three.........</ins>7</p> 
<p style="margin-left: 80px">&nbsp;&nbsp;&nbsp;&nbsp;3.1 Section A<ins onMouseEnter="mouseEnter(this)" data-issue="419" data-iso="approved">............</ins>8</p>

<p>...</p>

<p class="location">Replace Figure H.6 with the following corrected version:</p>

<figure>
  <ins onMouseEnter="mouseEnter(this)" data-issue="415" data-iso="approved">
    <img src="Figure H.6.svg" alt="Corrected Figure H.6 — Association between content and marked-content identifiers">
  </ins>
  <figcaption>Figure H.6 — Association between content and marked-content identifiers</figcaption>
</figure>

<p>...</p>

<p class="location">Replace Figure H.7 with the following corrected version:</p>

<figure>
  <ins onMouseEnter="mouseEnter(this)" data-issue="418" data-iso="approved">
    <img src="Figure H.7.svg" alt="Corrected Figure H.7 — Hierarchy of structure elements and relationship with marked-content">
  </ins>
  <figcaption>Figure H.7 — Hierarchy of structure elements and relationship with marked-content</figcaption>
</figure>

<p>...</p>

<p class="location">Correct the last EXAMPLE as follows:</p>

<code>...
400 0 obj
    &lt;&lt;/Type /StructElem
       /S <ins onMouseEnter="mouseEnter(this)" data-issue="425" data-iso="approved">/</ins>TOC
       /K [201 0 R 211 0 R 301 0 R 214 0 R 215 0 R 302 0 R]
       <ins onMouseEnter="mouseEnter(this)" data-issue="425" data-iso="approved">/P 400 0 R</ins>
    &gt;&gt;
endobj

</code>

<h3 id="HH.8.3">H.8.3 Hierarchical lists</h3>

<p class="location">Change the first paragraph as follows:</p>

<p>
The structure element’s structure type entry (<b>S</b>) may have values that establish hierarchical relationships between entries in a list. The <b>LI</b> value specifies an individual list entry. The <b>L</b> value specifies a list made up of individual list entries and/or lists of list entries. The trailing character in <b>LI</b> is an <del onMouseEnter="mouseEnter(this)" data-issue="75" data-iso="approved">upper case</del> <ins onMouseEnter="mouseEnter(this)" data-issue="75" data-iso="approved">uppercase</ins> "i".
</p>

<p>...</p>

<p class="location">Replace Figure H.9 with the following corrected version:</p>

<figure>
  <ins onMouseEnter="mouseEnter(this)" data-issue="418" data-iso="approved">
    <img src="Figure H.9.svg" alt="Corrected Figure H.9 — Hierarchy of structure elements and relationship with marked-content">
  </ins>
  <figcaption>Figure H.9 — Hierarchy of structure elements and relationship with marked-content</figcaption>
</figure>

<p>...</p>

</div>


<hr>
<p class="footnote">Last modified: {{page.modified}}</p>
