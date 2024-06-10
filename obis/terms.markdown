---
layout: base
title: Terms
---

## Terms

<table class="table">
  {% for term in site.data.terms %}
    <tr>
        <td><a name="{{term.name}}" />{{term.name}}</td>
        <td>
            {{term.definition}}
            <table class="table table-info table-sm mt-2">
                <tr><td>identifier</td><td>{{term.identifier}}</td></tr>
                <tr><td>examples</td><td>{{term.examples}}</td></tr>
            </table>
        </td>
    </tr>
  {% endfor %}
</table>
