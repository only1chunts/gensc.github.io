{% include header.html %}

# MIxS checklist terms



<ul> {% for term in site.data.terms %}
* MIXS ID - {{ term.mixsId }}
<br>
    <ul>{% for detail in term.details %}
			* Structured Comment name - {{detail.structuredCommentName}}
			* Term display name - {{detail.label}}
			* Definition - {{detail.definition}}
			* Expected value - {{detail.expectedValue}}
			* Value syntax - {{detail.valueSyntax}}
			* Example - {detail.example}}
			* Prefered Unit - {{detail.preferredUnit}}
			* Number of occurences permitted - {{detail.occurence}}
	</ul>	
		{% endfor %}
</ul>		
{% endfor %}

