---
number: 14
title: Document interchange
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


# 14. Document interchange


### 14.13.5 Associated files linked to graphics objects


...<br/>


The property list associated with the marked-content shall specify an array of file specification dictionaries to which
the content is associated. The named resource in the <span class="deleted-text"><b>Property List</b><span class="deleted-tooltiptext">
Issue #14</span></span> <span class="new-text"><i>property list</i><span class="new-tooltiptext">Issue #14</span></span>
(see 14.6.2, "Property lists") shall specify an array of file specification dictionaries to which the content is associated.
The relationship that the associated files have to the PDF content is supplied by the AFRelationship key in each file specification dictionary.


...<br/>


</div>

