{% include header.html %}

# MIxS checklist terms



<ul> {% for term in site.data.terms %}
* MIXS ID - {{ term.mixsId }}
<br>
    <ul>
			* Structured Comment name - {{term.details.structuredCommentName}}
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

