{% include header.html %}

# MIxS checklist terms



<ul> {% for term in site.data.terms %}
* MIXS ID - {{ term.mixsId }}
<br>
			* Structured Comment name - {{term.details.structuredCommentName}}
			* Term display name - {{term.details.label}}
			* Definition - {{term.details.definition}}
			* Expected value - {{term.details.expectedValue}}
			* Value syntax - {{term.details.valueSyntax}}
			* Example - {term.details.example}}
			* Prefered Unit - {{term.details.preferredUnit}}
			* Number of occurences permitted - {{term.details.occurence}}

</ul>		
{% endfor %}

