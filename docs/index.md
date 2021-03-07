---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

---
<div class="github-wp">



<h2>Background</h2>

<p>
This public repository is hosted by the <a href="https://www.pdfa.org">PDF Association</a> in order to provide developers
with a means of openly reporting issues against the latest core PDF 2.0 specification (<a href="https://www.iso.org/standard/75839.html">ISO 32000-2:2020</a>)
for review and resolution by industry and ISO experts. All issues in the PDF specification are important, from minor typos and formatting issues, to
larger ambiguous, unclear or apparently contradictory statements. By reaching consensus on resolutions as an industry,
PDF interoperability and implementation reliability will be improved.
</p>

<p>
Resolutions proposed here are <b>not</b> officially authorized by the ISO working group responsible for PDF
(ISO TC 171 SC 2 WG 8) and may be changed in future ISO 32000 publications.
</p>

<h2>Issues Resolved</h2>

<p>
The current set of resolved issues are presented as localized marked up changes
(<span style="background-color: lightyellow; color: green; position: relative; display: inline-block;">additions</span>
and <span style="background-color: seashell; color: red; text-decoration: line-through; text-decoration-color: red; position: relative; display: inline-block;">deletions</span>) to the published
wording in ISO 32000-2:2020 under each top level clause. Issue numbers (implemented here as popup tooltips) refer back to
<a href="https://github.com/pdf-association/pdf-issues/issues?q=is%3Aclosed+label%3A%22proposed+solution%22">closed GitHub pdf-issues with a "proposed solution" label</a>.
Due to ISO copyright, only minimal surrounding text from ISO 32000-2:2020 is provided that is sufficient to locate where the resolution is being applied.
</p>

{% for clause in site.clauses %}
  <h3>
    <a href="{{ site.baseurl }}{{ clause.url }}">
      {{ clause.number }} - {{ clause.title }}
    </a>
  </h3>
{% endfor %}

<br/><hr>
<p class="footnote">Last modified: 7 March 2021</p>

</div>
