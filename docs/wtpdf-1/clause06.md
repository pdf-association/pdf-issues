---
isodoc: WTPDF 1.0
title: 6. Conformance
last_modified_date: 29 May 2024
parent: Well-Tagged PDF 1.0
nav_order: 6
---

<nav class="subclauses">
<ul>
 <li>6.1 Conformance levels
   <ul>
     <li><a href="#H6.1.2">6.1.2 Conformance level for reuse</a>
     </li>
     <li><a href="#H6.1.3">6.1.3 Conformance level for accessibility</a>
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

<h2 id="H6.1">6.1 Conformance levels</h2>

<h3 id="H6.1.2">6.1.2 Conformance level for reuse</h3>

<p class="location">Correct the third paragraph as follows:</p>

<p>
Files conforming to the conformance level for reuse shall include a PDF Declaration with the URI identifier “http://pdfa.org/declarations/wtpdf<del onMouseEnter="mouseEnter(this)" data-issue="395">/</del>#reuse1.0” as its <i>pdfd:conformsTo</i> entry. The PDF Declaration may provide additional claim information using the <i>pdfd:claimData</i> entry.
</p>

<p class="location">Correct the example as follows:</p>

<code>...
&lt;pdfd:conformsTo&gt;
  http://pdfa.org/declarations/wtpdf<del onMouseEnter="mouseEnter(this)" data-issue="395">/</del>#reuse1.0
&lt;/pdfd:conformsTo&gt;
...

</code>

<h3 id="H6.1.3">6.1.3 Conformance level for accessibility</h3>

<p class="location">Correct the fourth paragraph as follows:</p>

<p>
Files conforming to the conformance level for accessibility shall include a PDF Declaration with the URI identifier “http://pdfa.org/declarations/wtpdf<del onMouseEnter="mouseEnter(this)" data-issue="395">/</del>#accessibility1.0” as its <i>pdfd:conformsTo</i> entry. The PDF Declaration may provide additional claim information using the <i>pdfd:claimData</i> entry.
</p>

<p class="location">Correct the example as follows:</p>

<code>...
&lt;pdfd:conformsTo&gt;
  http://pdfa.org/declarations/wtpdf<del onMouseEnter="mouseEnter(this)" data-issue="395">/</del>#accessibility1.0
&lt;/pdfd:conformsTo&gt;
...

</code>

</div>
