{% include header.html %}

# MIxS checklist terms

{% for term in site.data.terms %}

<ul>
# MIXS ID - {{ term.mixsId }}
	
        {% for detail in term.details %}
			* Structured Comment name - {{detail.structuredCommentName}}
			* Term display name - {{detail.label}}
			* Definition - {{detail.definition}}
			* Expected value - {{detail.expectedValue}}
			* Value syntax - {{detail.valueSyntax}}
			* Example - {detail.example}}
			* Prefered Unit - {{detail.preferredUnit}}
			* Number of occurences permitted - {{detail.occurence}}
			
		{% endfor %}
</ul>		
{% endfor %}

