{% include header.html %}

# MIxS checklist terms


<ul> {% for term in site.data.terms %}
* MIXS ID - {{ term.mixsId }}
<br>
<br> Structured Comment name - {{term.details.structuredCommentName}}
<br> Term display name - {{term.details.label}}
<br> Definition - {{term.details.definition}}
<br> Expected value - {{term.details.expectedValue}}
<br> Value syntax - {{term.details.valueSyntax}}
<br> Example - {term.details.example}}
<br> Prefered Unit - {{term.details.preferredUnit}}
<br> Number of occurences permitted - {{term.details.occurence}}
<br>
---		
{% endfor %}

