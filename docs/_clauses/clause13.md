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


<h1>13. Multimedia features</h1>


<h3>13.6.3 3D streams</h3>

<h4>13.3.6.1 General</h4>


<table>
  <caption>Table 311 - Entries in a 3D stream dictionary</caption>
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


<h4>13.6.4.3 3D background dictionaries</h4>

...<br/>

<p><i>New paragraph is added before existing NOTE:</i></p>

<span class="new-text">PDF processors that render 3D data streams shall do so directly and without regard to keys and values in the annotation dictionary that
define appearance streams or how appearance streams would be rendered onto the page. They shall ignore the values of the <b>C</b>, <b>IC</b>, <b>Border</b>, <b>BS</b>,
<b>BE</b>, <b>BM</b>, <b>CA</b> and <b>ca</b> keys from "Table 166 - Entries common to all annotation dictionaries".<span class="new-tooltiptext">Issue #39</span></span>

...<br/>


<table>
  <caption>Table 317 - Entries in a 3D background dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>CS</b></td>
    <td>name <span class="deleted-text">or array<span class="deleted-tooltiptext">Issue #38</span></span></td>
    <td>
    <p>(<i>Optional</i>) The colour space of the background. The only valid value shall be the name <i>DeviceRGB</i>.</p>
    <p>Default value: <i>DeviceRGB</i>.</p>
    <p><span class="deleted-text">PDF consumers shall be prepared to encounter other values that may be supported in future versions of PDF.<span class="deleted-tooltiptext">Issue #38</span></span></p>
    </td>
  </tr>
  <tr>
    <td><b>C</b></td>
    <td><span class="deleted-text">(various)<span class="deleted-tooltiptext">Issue #38</span></span>
        <span class="new-text">array<span class="new-tooltiptext">Issue #38</span></span>
    </td>
    <td>
    <p>(<i>Optional</i>)
    <span class="new-text">An array of 3 numbers in the range 0.0 to 1.0, representing the<span class="new-tooltiptext">Issue #38</span></span>
    <span class="deleted-text">The<span class="deleted-tooltiptext">Issue #38</span></span>
    colour of the background in the colour space defined by <b>CS</b>.</p>
    <p>Default value: an array [1 1 1] representing the colour white when the value of <b>CS</b> is <i>DeviceRGB</i>.</p>
    </td>
  </tr>
</table>


<h3>13.6.4.6 3D cross section dictionaries</h3>


<table>
  <caption>Table 322 - Entries in a 3D cross section dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>IV</b></td>
    <td>boolean</td>
    <td>
    ...<br/>
    <p>Default value: <span class="deleted-text">false<span class="deleted-tooltiptext">Issue #50</span></span> <span class="new-text">true<span class="new-tooltiptext">Issue #50</span></span></p>
    </td>
  </tr>
</table>


</div>


<br/><hr>
<p class="footnote">Last modified: 7 March 2021</p>

</body>
</html>
