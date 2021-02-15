---
number: 13
title: Multimedia features
---

<style>
  .iso32000 {
    font-family: Cambria, Georgia, serif;
  }
  .new-text {
    background-color: lightyellow;
    color: green;
    position: relative;
    display: inline-block;
  }
  .new-tooltiptext {
    font-family: Arial, Helvetica, sans-serif;
    visibility: hidden;
    color: green;
    background-color: lightyellow;
    border-radius: 6px;
    padding: 5px 0;
    text-align: center;
    min-width: 80px;
    border: 3px solid green;
    /* Position the tooltip */
    position: absolute;
    z-index: 1;
    bottom: 100%;
    left: 50%;
    margin-left: -50%;
  }

  .new-text .new-tooltiptext::after {
    content: "";
  }

  .new-text:hover .new-tooltiptext {
    visibility: visible;
    opacity: 1;
  }

  .deleted-text {
    background-color: seashell;
    color: red;
    text-decoration: line-through;
    text-decoration-color: red;
    position: relative;
    display: inline-block;
  }

  .deleted-tooltiptext {
    font-family: Arial, Helvetica, sans-serif;
    visibility: hidden;
    background-color: seashell;
    color: red;
    min-width: 80px;
    text-align: center;
    border-radius: 6px;
    border: 3px solid red;
    padding: 5px 0;
    /* Position the tooltip */
    position: absolute;
    z-index: 1;
    bottom: 100%;
    left: 50%;
    margin-left: -50%;
  }
  .deleted-text .deleted-tooltiptext::after {
    content: "";
  }
  .deleted-text:hover .deleted-tooltiptext {
    visibility: visible;
    opacity: 1;
  }

  table {
    margin-left: auto;
    margin-right: auto;
    border-collapse: collapse;
    border: 1px solid black;
  }
  caption {
    font-weight: bold;
  }
  th {
    text-align: left;
    border-collapse: collapse;
    border: 1px solid black;
    border-top: solid thick;
    border-bottom: solid thick;
  }
  td {
    text-align: left;
    min-width: 50px;
    max-width: 500px;
    border-collapse: collapse;
    border: 1px solid black;
  }
</style>


<div class="iso32000">


# 13. Multimedia features


### 13.6.3 3D streams

### 13.3.6.1 General


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

