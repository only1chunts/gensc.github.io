{% include header.html %}

# MIxS checklist terms

{% for term in site.data.terms %}
	<ui><h4>MIXS ID - {{ term.mixsId }}</h4></ui>
        <li>{% for detail in term.details %}
			<p>Structured Comment name - {{detail.structuredCommentName}}</p>
			<p>Term display name - {{detail.label}}</p>
			<p>Definition - {{detail.definition}}</p>
			<p>Expected value - {{detail.expectedValue}}</p>
			<p>Value syntax - {{detail.valueSyntax}}</p>
			<p>Example - {detail.example}}</p>
			<p>Prefered Unit - {{detail.preferredUnit}}</p>
			<p>Number of occurences permitted - {{detail.occurence}}</p>
		{% endfor %}
</li>
        </div>
        {% endfor %}
</div>
