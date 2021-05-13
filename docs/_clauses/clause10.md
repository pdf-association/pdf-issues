---
number: 10
title: Rendering
---


<html lang="en">
<head>
<meta charset="UTF-8">
<title>ISO 32000-2:2020 Clause 10: Rendering</title>
{% include iso-style.html %}
</head>
<body>


<div class="iso32000">


<h1>10. Rendering</h1>


<h4>10.6.5.6 Type 5 halftones</h4>


<table>
  <caption>Table 132 - Entries in a Type 5 halftone dictionary</caption>
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
    <span class="deleted-text">The value shall not be 5.<span class="deleted-tooltiptext">Issue #12</span></span>
    <span class="new-text">The halftone shall not be a Type 5 halftone.<span class="new-tooltiptext">Issue #12</span></span>
    If there are any nonprimary colourants, the default halftone shall have a transfer function.
    </td>
  </tr>
</table>


</div>


<br/><hr>
<p class="footnote">Last modified: 16 February 2021</p>

</body>
</html>
