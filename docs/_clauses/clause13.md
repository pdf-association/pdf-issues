---
number: 13
title: Multimedia features
---


<html>
<head>
<title>ISO 32000-2:2020 Clause 13: Multimedia</title>
</head>
<body>


{% include iso-style.html %}


<div class="iso32000">


<h1>13. Multimedia features</h>


<h3>13.6.3 3D streams</h4>

<h4>13.3.6.1 General</h4>


<table>
  <caption>Table 311 - Entries in a 3d stream dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>ColorSpace</b></td>
    <td>name or array</td>
    <td>
    (<i>Optional, PDF 2.0</i>) The RGB colour space in which the 3D artwork's colour values are encoded. Valid values are the name
    <b>DeviceRGB</b>, an array specifying a valid <b>CalRGB</b> color space (see 8.6.5.3 "CalRGB colour spaces"), or an array specifying
    a valid RGB-based <b>ICCBased</b> color space (see 8.6.5.5 "ICCBased colour spaces").
    <span class="new-text">If the name is <b>DeviceRGB</b> and the page where the annotation referencing the 3D stream is used has a <b>DefaultRGB</b> color space,
    then the <b>DefaultRGB</b> color space shall be used (see 8.6.5.6 Default colour spaces).<span class="new-tooltiptext">Issue #18</span></span>
    If this key is not present, the colour space for the 3D artwork colour values  <span class="deleted-text">are<span class="deleted-tooltiptext">Issue #18</span></span>
    <span class="new-text">is<span class="new-tooltiptext">Issue #18</span></span> considered undefined and a PDF processor may choose any appropriate
    RGB-based colour space, such as sRGB.
    </td>
  </tr>
</table>

</div>

<hr>
<p style="text-align:center">Last modified: 16 February 2021</p>

</body>
</html>
