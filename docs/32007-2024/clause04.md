---
isodoc: ISO 32007:2024
title: 4. RichMedia annotations with glTF assets
last_modified_date: 13 October 2026
parent: 'ISO TS 32004: '
nav_order: 4
---

<nav class="subclauses">
<ul class="noprint">
 <li><a href="#H4.8">4.8 Marking the Extension Level in PDF</a>
 </li>
</ul>
</nav>
<hr>

<div class="isostyle">
<div class="fixedpopup" id="issuelink">
  Issue #xxxx
</div>

<p class="fake-h1">{{ page.title }}</p>

<h2 id="H4.8">4.8 Marking the Extension Level in PDF</h2>

<p class="location">Change the EXAMPLE as follows (correct <b>ExtensionLevel</b> value to an integer):</p>

<pre>
%PDF-2.0 
&lt;&lt; /Type /Catalog 
    /Extensions 
    &lt;&lt;/ISO_ 
       &lt;&lt; /Type /DeveloperExtensions 
          /BaseVersion /2.0 
          /ExtensionLevel <del onMouseEnter="mouseEnter(this)" data-issue="835" data-iso="approved">/</del>32007 
          /ExtensionRevision (1:2024) 
          /URL (https://www.iso.org/standard/45880.html) 
       &gt;&gt; 
    &gt;&gt;
&gt;&gt;
</pre>

</div>
