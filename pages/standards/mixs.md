{% include header.html %}

# MIxS checklist terms

{% for term in site.data.terms %}
<h4>MIXS ID - {{ term.mixsId }} </h4>
Term display name - {{term.label}}
<br> Structured Comment name - {{term.structuredCommentName}}
<br> Definition - {{term.definition}}
<br> Expected value - {{term.expectedValue}}
<br> Value syntax - {{term.valueSyntax}}
<br> Example - {{term.example}}
<br> Prefered Unit - {{term.preferredUnit}}
<br> Number of occurences permitted - {{term.occurence}}
<br>
<br>		
{% endfor %}

