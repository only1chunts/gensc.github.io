{% include header.html %}

<div> 	{% for term in site.checklists.mixsId %}
        <div><h4>MIXS ID - {{ term.item }}</h4>
        {% for item in term.mixsId %}
			<p>Structured Comment name - {{mixsId.structuredCommentName}}</p>
			<p>Term display name - {{label}}</p>
			<p>Definition - {{definition}}</p>
			<p>Expected value - {{expectedValue}}</p>
			<p>Value syntax - {{valueSyntax}}</p>
			<p>Example - {{example}}</p>
			<p>Prefered Unit - {{preferredUnit}}</p>
			<p>Number of occurences permitted - {{occurence}}</p>
		{% endfor %}

        </div>
        {% endfor %}
</div>
