---
---

<style>
body {
  font-family: Cambria, Georgia, serif;
}
.new-text {
  background-color: lightyellow; 
  color: green;
}
.deleted-text {
  background-color: seashell; 
  color: red; 
  text-decoration: line-through; 
  text-decoration-color: red; 
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

Jekyll pages are written in Markdown](https://learnxinyminutes.com/docs/markdown/) and can supposedly also use HTML tags.
~~This text is strikethrough.~~ **This text is bold.** _This text is italic_ **_This is both bold and italic_**

This text has strikethrough on ~~**bold**~~ and ~~_italic_~~ and ~~**_both_**~~

| Col1         | Col2     | Col3          |
| :----------- | :------: | ------------: |
| Left-aligned | Centered | Right-aligned |
| blah         | blah     | blah          |
| blah blah blah | blah blah blah| blah blah blah |

## Some HTML H2

Hopefully this mimics what ISO 32000-2:2020 looks like. MSWord master doc uses Cambria 11 for body, and Cambria 13 for H3.

<h3>8.9.7 Inline images</h3>

<p>The key-value pairs appearing between the <b>BI</b> and <b>ID</b> operators (as listed in "Table 91 — Entries in an inline image object") are analogous to their respective key-value pairs in an image XObject dictionary (see "Table 87 — Additional entries specific to an image dictionary") or a stream dictionary (see "Table 5 — Entries common to all stream dictionaries"). For convenience, the abbreviations shown in "Table 91 — Entries in an inline image object" and "Table 92 — Additional abbreviations in an inline image object" may be used in place of the full names. <span id="new-text">In the situation where both an abbreviated key name and the corresponding full key name from Table 91 are present, the abbreviated key name shall take precedence.</span> Entries other than those listed shall be ignored. <span id="deleted-text">Fake deleted text.</span>
</p>

And this is a random dictionary table from PDF 2.0.


<table>
<caption>Table 93 — Additional entries specific to a Type 1 form dictionary</caption>
<tr>
	<th>Key</th>
	<th>Type</th>
	<th>Value</th>
</tr>
<tr>
	<td><b>Type</b></td>
	<td>name</td>
	<td>(<i>Optional</i>) The type of PDF object that this dictionary describes; if present,
	shall be <i>XObject</i> for a form XObject.</td>
</tr>
<tr>
	<td><b>Matrix</b></td>
	<td>array</td>
	<td>(<i>Optional</i>) An array of six numbers specifying the form matrix, which maps form space 
	into user space (see 8.3.4, "Transformation matrices"). Default value: the identity matrix <i>[1 0 0 1 0 0]</i>.
	</td>
</tr>
</table>
