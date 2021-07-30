---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 13
title: Multimedia features
---

{% include iso-style.html %}
<div class="isostyle">


<h1>{{ page.clause }}. {{ page.title }}</h1>


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
    then the <b>DefaultRGB</b> color space shall be used (see 8.6.5.6 Default colour spaces).<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/18" target="_blank">Issue #18</a></span></span>
    If this key is not present, the colour space for the 3D artwork colour values  <span class="deleted-text">are<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/18" target="_blank">Issue #18</a></span></span>
    <span class="new-text">is<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/18" target="_blank">Issue #18</a></span></span> considered undefined and a PDF processor may choose any appropriate
    RGB-based colour space, such as sRGB.
    </td>
  </tr>
</table>

<h3>13.6.4 3D Views</h3>

<h4>13.6.4.1 General</h4>

<table>
  <caption>Table 315 - Entries in a 3D view dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>P</b></td>
    <td>dicionary</td>
    <td>
    <p>...</p>
    <p>Default value: a projection dictionary where the value of <b>Subtype</b> is
    <span class="deleted-text"><i>Perspective</i><span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/91" target="_blank">Issue #91</a></span></span><span class="new-text"><i>P</i> (perspective)<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/91" target="_blank">Issue #91</a></span></span>,
    the value of <b>FOV</b> is 90, and all other entries take their default values.
    </p>
    </td>
  </tr>
</table>


<h4>13.6.4.3 3D background dictionaries</h4>

<p>...</p>

<p><i>New paragraph is added before existing NOTE:</i></p>

<span class="new-text">PDF processors that render 3D data streams shall do so directly and without regard to keys and values in the annotation dictionary that
define appearance streams or how appearance streams would be rendered onto the page. They shall ignore the values of the <b>C</b>, <b>IC</b>, <b>Border</b>, <b>BS</b>,
<b>BE</b>, <b>BM</b>, <b>CA</b> and <b>ca</b> keys from "Table 166 - Entries common to all annotation dictionaries".<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/39" target="_blank">Issue #39</a></span></span>

<p>...</p>


<table>
  <caption>Table 317 - Entries in a 3D background dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>CS</b></td>
    <td>name <span class="deleted-text">or array<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/38" target="_blank">Issue #38</a></span></span></td>
    <td>
    <p>(<i>Optional</i>) The colour space of the background. The only valid value shall be the name <i>DeviceRGB</i>.</p>
    <p>Default value: <i>DeviceRGB</i>.</p>
    <p><span class="deleted-text">PDF consumers shall be prepared to encounter other values that may be supported in future versions of PDF.<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/38" target="_blank">Issue #38</a></span></span></p>
    </td>
  </tr>
  <tr>
    <td><b>C</b></td>
    <td><span class="deleted-text">(various)<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/38" target="_blank">Issue #38</a></span></span>
        <span class="new-text">array<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/38" target="_blank">Issue #38</a></span></span>
    </td>
    <td>
    <p>(<i>Optional</i>)
    <span class="new-text">An array of 3 numbers in the range 0.0 to 1.0, representing the<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/38" target="_blank">Issue #38</a></span></span>
    <span class="deleted-text">The<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/38" target="_blank">Issue #38</a></span></span>
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
    <td><span class="new-text"><b>IV</b><span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/49" target="_blank">Issue #49</a></span></span></td>
    <td><span class="new-text">boolean<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/49" target="_blank">Issue #49</a></span></span></td>
    <td>
	<p><span class="new-text">(<i>Optional</i>>) A flag indicating the visibility of the cutting plane. If <i>true</i>, then the cutting plane shall be visible.
	If <i>false</i>, then the cutting plane shall not be visible.<br/>
	Default value: <i>true</i><span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/49" target="_blank">Issue #49</a></span></span></p>
    </td>
  </tr>
  <tr>
    <td><b>PV</b></td>
    <td>boolean</td>
    <td>
	<p>...</p>
    <p>Default value: <span class="deleted-text">false<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/50" target="_blank">Issue #50</a></span></span> <span class="new-text">true<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/50" target="_blank">Issue #50</a></span></span></p>
    </td>
  </tr>
</table>


<h5>13.7.2.2.2 RichMediaActivation dictionary</h5>


<table>
  <caption>Table 335 - Entries in a RichMediaActivation dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><span class="new-text"><b>Scripts</b><span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/59" target="_blank">Issue #59</a></span></span></td>
    <td><span class="new-text">array<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/59" target="_blank">Issue #59</a></span></span></td>
    <td>
    <div class="new-text">
    <p>
    (<i>Optional; PDF 2.0</i>) An array of indirect object references to file specification dictionaries, each of which describe a JavaScript file that shall be present in
    the <b>Assets</b> name tree of the RichMediaContent dictionary. If the array has no elements, no script is executed.</p>
    <p>Default value: an empty array.</p>
    <span class="new-tooltiptext">Issue #59</span></div>
    </td>
  </tr>
</table>


<h5>13.7.2.3.4 RichMediaInstance dictionary</h5>


<table>
  <caption>Table 343 - Entries in a RichMediaInstance dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Asset</b></td>
    <td>dictionary</td>
    <td>
    <p>(<i>Required; PDF 2.0</i>) A dictionary that shall be an indirect object reference to a file specification dictionary that
    <span class="deleted-text">is also<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/58" target="_blank">Issue #58</a></span></span>
    <span class="new-text">may also be<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/58" target="_blank">Issue #58</a></span></span>
    referenced in the <b>Assets</b> name tree specified in the RichMediaContent dictionary of the annotation.
    </p>
    <p>
    <span class="new-text">NOTE the RichMedia asset itself is not referenced by name, however other assets may be referenced from the
    RichMedia asset by name and thus need to be in the <b>Assets</b> name tree.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/58" target="_blank">Issue #58</a></span></span>
    </p>
    </td>
  </tr>
</table>


</div>


<hr>
<p class="footnote">Last modified: 18 June 2021</p>
