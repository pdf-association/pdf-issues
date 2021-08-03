---
subset: PDF 2.0
isodoc: ISO 32000-2:2020
clause: 8
title: Graphics
---

{% include iso-style.html %}
<div class="isostyle">


<h1>{{ page.clause }}. {{ page.title }}</h1>

<h2 id="H8.2">8.2 Graphics objects</h2>

<p>...</p>

<table>
  <caption id="Table50">Table 50 - Operator categories</caption>
  <tr>
    <th>Category</th>
    <th>Operators</th>
    <th>Location</th>
  </tr>
  <tr>
    <td>Shading patterns</td>
    <td>
    <span class="deleted-text"><b>Sh</b><span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/80" target="_blank">Issue #80</a></span></span>
    <span class="new-text"><b>sh</b><span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/80" target="_blank">Issue #80</a></span></span>
    </td>
    <td>"Table 76 — Shading operator"
    </td>
  </tr>
  <tr>
    <td>...</td>
    <td>...</td>
    <td>...</td>
  </tr>
  <tr>
    <td>Marked-content</td>
    <td><b>MP, DP, BMC, BDC, EMC</b></td>
    <td>
    <span class="deleted-text">"Table 351 — Entries in a data dictionary"<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/85" target="_blank">Issue #85</a></span></span>
    <span class="new-text">"Table 352 — Marked-content operators"<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/85" target="_blank">Issue #85</a></span></span>
    </td>
  </tr>
</table>

<h3 id="H8.5.3">8.5.3 Path-painting operators</h3>

<h4 id="H8.5.3.1">8.5.3.1 General</h4>

<p>...</p>

<table>
  <caption id="Table59">Table 59 - Path-painting categories</caption>
  <tr>
    <th>Operands</th>
    <th>Operator</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>-</td>
    <td><b>B</b></td>
    <td>
    <p>Fill and then stroke the path, using the non-zero winding number rule to determine the region to fill.
    <span class="new-text">In the opaque imaging model, this<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/103" target="_blank">Issue #103</a></span></span>
    <span class="deleted-text">This<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/103" target="_blank">Issue #103</a></span></span> operator shall produce the same result
    as constructing two identical path objects, painting the first with <b>f</b> and the second with <b>S</b>.</p>
    <p>...</p>
    </td>
  </tr>
</table>


<h4 id="H8.6.5.8">8.6.5.8 Rendering Intents</h4>

<p>...</p>

<p>
NOTE The exact set of rendering intents supported can vary from one output device to another; a particular device
<span class="deleted-text">does not have to support all PDF rendering intents and<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/63" target="_blank">Issue #63</a></span></span>
can support additional ones beyond those listed in the table above.
</p>


<h3 id="H8.9.5">8.9.5 Image dictionaries</h3>


<h4 id="H8.9.5.1">8.9.5.1 General</h4>


<table>
  <caption id="Table87">Table 87 - Additional entries specific to an image dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Intent</b></td>
    <td>name</td>
    <td>
    	<p>...</p>
    	<p><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    	Soft-mask images.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/13" target="_blank">Issue #13</a></span></span></p>
    </td>
  </tr>
  <tr>
    <td><b>ImageMask</b></td>
    <td>boolean</td>
    <td>(<i>Optional</i>) A flag indicating whether the image shall be treated as an image mask (see 8.9.6, "Masked images"). If this flag is <i>true</i>,
    the value of <b>BitsPerComponent</b>, if present, shall be 1 and <span class="deleted-text">Mask<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span>
    <span class="new-text"><b>Mask</b><span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/14" target="_blank">Issue #14</a></span></span> and <b>ColorSpace</b> shall not be specified; unmasked areas shall be
    painted using the current nonstroking colour. Default value: <i>false</i>.
    </td>
  </tr>
  <tr>
    <td><b>Alternates</b></td>
    <td>array</td>
    <td>
    	<p>...</p>
    	<p><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/13" target="_blank">Issue #13</a></span></span></p></td>
  </tr>
  <tr>
    <td><b>SMask</b></td>
    <td>stream</td>
    <td><p>...</p><p><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/13" target="_blank">Issue #13</a></span></span></p></td>
  </tr>
  <tr>
    <td><b>Name</b></td>
    <td>name</td>
    <td><p>...</p><p><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/13" target="_blank">Issue #13</a></span></span></p></td>
  </tr>
  <tr>
    <td><b>StructParent</b></td>
    <td>integer</td>
    <td><p>...</p><p><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/13" target="_blank">Issue #13</a></span></span></p></td>
  </tr>
  <tr>
    <td><b>ID</b></td>
    <td>byte string</td>
    <td><p>...</p><p><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/13" target="_blank">Issue #13</a></span></span></p></td>
  </tr>
</table>


<h3 id="H8.9.7">8.9.7 Inline images</h3>


<p>...</p>

<p>
Inline image objects shall not be nested; that is, two <b>BI</b> operators shall not appear without an intervening <b>EI</b> to close the first object.
Similarly, an <b>ID</b> operator shall only appear between a <b>BI</b> and its balancing <b>EI</b>. Unless the image uses <b>ASCIIHexDecode</b> or
<b>ASCII85Decode</b> as <span class="deleted-text">one of its filters<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/20" target="_blank">Issue #20</a></span></span>
<span class="new-text">its final or only filter<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/20" target="_blank">Issue #20</a></span></span>, the <b>ID</b> operator shall be followed by a
single white-space character, and the next character shall be interpreted as the first byte of image data.
</p>

<p>
The key-value pairs appearing between the <b>BI</b> and <b>ID</b> operators (as listed in "Table 91 - Entries in an inline
image object") are analogous to their respective key-value pairs in an image XObject dictionary (see "Table 87 - Additional
entries specific to an image dictionary") or a stream dictionary (see "Table 5 - Entries common to all stream dictionaries").
For convenience, the abbreviations shown in "Table 91 - Entries in an inline image object" and "Table 92 - Additional
abbreviations in an inline image object" may be used in place of the full names. <span class="new-text">In the situation where
both an abbreviated key name and the corresponding full key name from Table 91 are present, the abbreviated key name shall take
precedence.<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/3" target="_blank">Issue #3</a></span></span> Entries other than those listed shall be ignored.
</p>

<p>...</p>

<p>
<span class="deleted-text">NOTE 3 The names <b>DeviceGray</b>, <b>DeviceRGB</b>, and <b>DeviceCMYK</b> (as well as their abbreviations <b>G</b>, <b>RGB</b>, and <b>CMYK</b>) always
identify the corresponding colour spaces directly; they never refer to resources in the <b>ColorSpace</b> subdictionary.<span class="deleted-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/19" target="_blank">Issue #19</a></span></span>


<span class="new-text">The names <b>DeviceGray</b>, <b>DeviceRGB</b>, and <b>DeviceCMYK</b> (as well as their abbreviations <b>G</b>, <b>RGB</b>, and <b>CMYK</b>) never refer to
resources in the <b>ColorSpace</b> subdictionary; they always identify the corresponding colour spaces either directly or via a default colour space (see
8.6.5.6 "Default colour spaces").<span class="new-tooltiptext"><a href="https://github.com/pdf-association/pdf-issues/issues/19" target="_blank">Issue #19</a></span></span>
</p>

<p>...</p>

</div>


<hr>
<p class="footnote">Last modified: 30 July 2021</p>
