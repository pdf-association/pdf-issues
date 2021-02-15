# ISO 32000-2 Issues

## Background
This public repository is hosted by the [PDF Association](https://www.pdfa.org) in order to provide developers with a means of openly reporting issues against the latest core PDF 2.0 specification ([ISO 32000-2:2020](https://www.iso.org/standard/75839.html)) for review and resolution by industry and ISO experts. All issues in the PDF specification are important, from minor typos and formatting issues, to larger ambiguous, unclear or apparently contradictory statements. By reaching consensus on resolutions as an industry, PDF interoperability and implementation reliability will be improved.

Resolutions proposed here are **not** officially authorized by the ISO working group responsible for PDF (ISO TC 171 SC 2 WG 8) and may be changed in future ISO 32000 publications.

## Issues Resolved

The current set of resolved issues are presented as marked up changes (additions and deletions) to the published wording in ISO 32000-2:2020 under each top level clause. Issue numbers refer back to [closed GitHub pdf-issues with a "proposed solution" label](https://github.com/pdf-association/pdf-issues/issues?q=is%3Aclosed+label%3A%22proposed+solution%22).


{% for clause in site.clauses %}
  <h3>
    <a href="{{ clause.url }}">
      {{ clause.number }} - {{ clause.title }}
    </a>
  </h3>
{% endfor %}

