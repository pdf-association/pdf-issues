---
number: 9
title: Text
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


# 9. Text


## 9.8 Font descriptors


### 9.8.1 General


<table>
  <caption>Table 120 - Entries common to all font descriptors</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>FontName</b></td>
    <td>name</td>
    <td>
    (<i>Required <span class="new-text">for non-Type 3 fonts<span class="new-tooltiptext">Issue #11</span></span></i>)
    The PostScript name of the font. This name shall be the same as the value of <b>BaseFont</b> in the font or CIDFont dictionary
    that refers to this font descriptor.
    </td>
  </tr>
</table>


#### 9.8.3.3 FD


...<br/>


The key for each entry in an <b>FD</b> dictionary shall be the name of a class of glyphs - that is, a particular subset of the CIDFont's
character collection. The entry's value shall be a font descriptor whose contents shall <span class="new-text">be a subset of the keys defined
in "Table 120 - Entries common to all font descriptors" that<span class="new-tooltiptext">Issue #5</span></span> override the font-wide attributes for that
class only. This font descriptor <span class="deleted-text">shall contain<span class="deleted-tooltiptext">Issue #5</span></span><span class="new-text">contains<span
class="new-tooltiptext">Issue #5</span></span> entries for metric information only; it shall not include <b>FontFile</b>, <b>FontFile2</b>,
<b>FontFile3</b>, or any of the entries listed in <span class="deleted-text">"Table 120 - Entries common to all font descriptors"
<span class="deleted-tooltiptext">Issue #5</span></span><span class="new-text">"Table 122 - Additional font descriptor entries for CIDFonts"
<span class="new-tooltiptext">Issue #5</span></span>.

</div>

