{% include header.html %}

# MIxS checklist terms


{% for term in site.data.terms %}
<h4>MIXS ID - {{ term.mixsId }} </h4>

<tbody>
    {% for detail in term.details %}
        <tr>
            <td width="20%">
            </td>
            <td>
            <p><b>Term display name - {{detail.label}}</b></p>
	        <p>Structured Comment name - {{term.details.structuredCommentName}}</p>
<br> Definition - {{term.details.definition}}
<br> Expected value - {{term.details.expectedValue}}
<br> Value syntax - {{term.details.valueSyntax}}
<br> Example - {{term.details.example}}
<br> Prefered Unit - {{term.details.preferredUnit}}
<br> Number of occurences permitted - {{term.details.occurence}}
<br>
            </td>
        </tr>
    {% endfor %}
</tbody>

<br>		
{% endfor %}

