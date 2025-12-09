---
subset: XMP RELAX NG schemas
isodoc: ISO 16684-2:2014
title: 'Annex C: (informative) RELAX NG schema for the XMP namespace'
last_modified_date: 11 November 2025
parent: ISO 16684-2:2014 XMP RELAX NG schema
nav_order: 1
---

<div class="isostyle">
<div class="fixedpopup" id="issuelink">
	Issue #xxxx
</div>

<p class="fake-h1">{{ page.title }}</p>

<p class="location">Based on <a href="https://github.com/pdf-association/pdfa-twg/issues/56">PDF/A Errata #56</a>, change the RELAX NG XML as follows:</p>

<code>
   &lt;rng:define name=”xmp.Base.Rating” combine=”choice”&gt;
      &lt;rng:choice&gt;
         <ins>&lt;!-- NOTE: Earlier versions of XMP specifications specified this property as Integer --&gt;</ins>
         &lt;rng:value type=”<del>float</del><ins>double</ins>”&gt;-1&lt;/rng:value&gt; 
         &lt;rng:data type=”<del>float</del><ins>double</ins>”&gt;
            &lt;rng:param name=”minInclusive”&gt;0&lt;/rng:param&gt; 
            &lt;rng:param name=”maxInclusive”&gt;5&lt;/rng:param&gt;
         &lt;/rng:data&gt;
      &lt;/rng:choice&gt;
   &lt;/rng:define&gt;

</code>

</div>
