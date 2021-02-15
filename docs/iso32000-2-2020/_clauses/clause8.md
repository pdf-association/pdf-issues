---
number: 8
title: Graphics
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


# 8. Graphics

### 8.9.5 Image dictionaries


#### 8.9.5.1. General


<table>
  <caption>Table 87 - Additional entries specific to an image dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Intent</b></td>
    <td>name</td>
    <td>...<br/><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext">Issue #13</span></span></td>
  </tr>
  <tr>
    <td><b>ImageMask</b></td>
    <td>boolean</td>
    <td>(<i>Optional</i>) A flag indicating whether the image shall be treated as an image mask (see 8.9.6, "Masked images"). If this flag is <i>true</i>,
    the value of <b>BitsPerComponent</b>, if present, shall be 1 and <span class="deleted-text">Mask<span class="deleted-tooltiptext">Issue #14</span></span>
    <span class="new-text"><b>Mask</b><span class="new-tooltiptext">Issue #14</span></span> and <b>ColorSpace</b> shall not be specified; unmasked areas shall be
    painted using the current nonstroking colour. Default value: <i>false</i>.
    </td>
  </tr>
  <tr>
    <td><b>Alternates</b></td>
    <td>array</td>
    <td>...<br/><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext">Issue #13</span></span></td>
  </tr>
  <tr>
    <td><b>SMask</b></td>
    <td>stream</td>
    <td>...<br/><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext">Issue #13</span></span></td>
  </tr>
  <tr>
    <td><b>Name</b></td>
    <td>name</td>
    <td>...<br/><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext">Issue #13</span></span></td>
  </tr>
  <tr>
    <td><b>StructParent</b></td>
    <td>integer</td>
    <td>...<br/><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext">Issue #13</span></span></td>
  </tr>
  <tr>
    <td><b>ID</b></td>
    <td>byte string</td>
    <td>...<br/><span class="new-text">Additional limitations also apply to this key when used in soft-mask image dictionaries - see clause 11.6.5.2
    Soft-mask images.<span class="new-tooltiptext">Issue #13</span></span></td>
  </tr>
</table>


### 8.9.7 Inline images


...<br/>


Inline image objects shall not be nested; that is, two <b>BI</b> operators shall not appear without an intervening <b>EI</b> to close the first object.
Similarly, an <b>ID</b> operator shall only appear between a <b>BI</b> and its balancing <b>EI</b>. Unless the image uses <b>ASCIIHexDecode</b> or
<b>ASCII85Decode</b> as <span class="deleted-text">one of its filters<span class="deleted-tooltiptext">Issue #20</span></span>
<span class="new-text">its final or only filter<span class="new-tooltiptext">Issue #20</span></span>, the <b>ID</b> operator shall be followed by a
single white-space character, and the next character shall be interpreted as the first byte of image data.


The key-value pairs appearing between the <b>BI</b> and <b>ID</b> operators (as listed in "Table 91 - Entries in an inline
image object") are analogous to their respective key-value pairs in an image XObject dictionary (see "Table 87 - Additional
entries specific to an image dictionary") or a stream dictionary (see "Table 5 - Entries common to all stream dictionaries").
For convenience, the abbreviations shown in "Table 91 - Entries in an inline image object" and "Table 92 - Additional
abbreviations in an inline image object" may be used in place of the full names. <span class="new-text">In the situation where
both an abbreviated key name and the corresponding full key name from Table 91 are present, the abbreviated key name shall take
precedence.<span class="new-tooltiptext">Issue #3</span></span> Entries other than those listed shall be ignored.


...<br/>


<span class="deleted-text">NOTE 3 The names <b>DeviceGray</b>, <b>DeviceRGB</b>, and <b>DeviceCMYK</b> (as well as their abbreviations <b>G</b>, <b>RGB</b>, and <b>CMYK</b>) always
identify the corresponding colour spaces directly; they never refer to resources in the <b>ColorSpace</b> subdictionary.<span class="deleted-tooltiptext">Issue #19</span></span>


<span class="new-text">The names <b>DeviceGray</b>, <b>DeviceRGB</b>, and <b>DeviceCMYK</b> (as well as their abbreviations <b>G</b>, <b>RGB</b>, and <b>CMYK</b>) never refer to
resources in the <b>ColorSpace</b> subdictionary; they always identify the corresponding colour spaces either directly or via a default colour space (see
8.6.5.6 "Default colour spaces").<span class="new-tooltiptext">Issue #19</span></span>


...<br/>


</div>

