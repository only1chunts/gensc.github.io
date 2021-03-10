{% include header.html %}

# MIxS checklist terms

{% for term in site.data.terms %}
	<ui>MIXS ID - {{ term.mixsId }}</ui>
        {% for detail in term.details %}
			<li><p>Structured Comment name - {{detail.structuredCommentName}}</p></li>
			<li><p>Term display name - {{detail.label}}</p></li>
			<li><p>Definition - {{detail.definition}}</p></li>
			<li><p>Expected value - {{detail.expectedValue}}</p></li>
			<li><p>Value syntax - {{detail.valueSyntax}}</p></li>
			<li><p>Example - {detail.example}}</p></li>
			<li><p>Prefered Unit - {{detail.preferredUnit}}</p></li>
			<li><p>Number of occurences permitted - {{detail.occurence}}</p></li>
		{% endfor %}
{% endfor %}

