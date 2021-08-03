---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 10
title: Rendering
---

{% include iso-style.html %}
<div class="isostyle">


<h1>{{ page.clause }}. {{ page.title }}</h1>


<h4 id="H10.6.5.6">10.6.5.6 Type 5 halftones</h4>


<table>
  <caption id="Table132">Table 132 - Entries in a Type 5 halftone dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Default</b></td>
    <td>dictionary or<br/>stream</td>
    <td>
    (<i>Required</i>) A halftone that shall be used for any colourant or colour component that does not have an entry of its own.
    <span class="deleted-text">The value shall not be 5.<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/12" target="_blank">Issue #12</a></span></span>
    <span class="new-text">The halftone shall not be a Type 5 halftone.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/12" target="_blank">Issue #12</a></span></span>
    If there are any nonprimary colourants, the default halftone shall have a transfer function.
    </td>
  </tr>
</table>


</div>


<hr>
<p class="footnote">Last modified: 16 February 2021</p>
