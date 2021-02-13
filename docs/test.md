---
---

<style>
  body {  
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

# Test H1

## Markdown Test H2
Jekyll pages are written in [Markdown](https://learnxinyminutes.com/docs/markdown/) and can supposedly also use HTML tags. 
~~This text is strikethrough.~~ **This text is bold.** _This text is italic_ **_This is both bold and italic_**

This text has strikethrough on ~~**bold**~~ and ~~_italic_~~ and ~~**_both_**~~

| Col1         | Col2     | Col3          |
| :----------- | :------: | ------------: |
| Left-aligned | Centered | Right-aligned |
| blah blah blah blah | blah blah blah blah | blah blah blah blah |
| blah <span class="new-text">blah<span class="new-tooltiptext">Issue #999</span></span> blah | blah blah blah| <span class="deleted-text">blah<span class="deleted-tooltiptext">Issue #692</span></span> blah |



## Some HTML H2

Hopefully this mimics what ISO 32000-2:2020 looks like. MSWord master doc uses Cambria 11 for body, and Cambria 13 for H3.

### 8.9.7 Inline images

The key-value pairs appearing between the <b>BI</b> and <b>ID</b> operators (as listed in "Table 91 - Entries in an inline 
image object")are analogous to their respective key-value pairs in an image XObject dictionary (see "Table 87 - Additional 
entries specific to an imagedictionary") or a stream dictionary (see "Table 5 - Entries common to all stream dictionaries"). 
For convenience, the abbreviations shown in "Table 91 - Entries in an inline image object" and "Table 92 - Additional 
abbreviations in an inline image object" may be used in place of the full names. 
<span class="new-text">In the situation where both an abbreviated key name and the corresponding full key name from Table 91 are present, 
the abbreviated key name shall take precedence.<span class="new-tooltiptext">Issue #5</span></span> 
Entries other than those listed shall be ignored. 
<span class="deleted-text">Fake deleted text.<span class="deleted-tooltiptext">Issue #3</span></span>

<table>
  <caption>Table 93 - Additional entries specific to a Type 1 form dictionary</caption>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Value</th>
  </tr>
  <tr>
    <td><b>Type</b></td>
    <td>name</td>
    <td>(<i>Optional</i>) The type of PDF object <span class="new-text">that this dictionary describes<span class="new-tooltiptext">Issue #1</span></span>; if present,shall be <i>XObject</i> for a form XObject.</td>
  </tr>
  <tr>
    <td><b>Matrix</b></td>
    <td>array</td>
    <td>(<i>Optional</i>) An array of six numbers specifying the form matrix, which maps form space into user space (see 8.3.4, "Transformation 
    matrices"). Default value: the identity <span class="deleted-text">matrix<span class="deleted-tooltiptext">Issue #7</span></span> <i>[1 0 0 1 0 0]</i>.</td>
  </tr>
</table>
