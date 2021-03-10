{% include header.html %}

# MIxS checklist terms

{% for term in site.data.terms %}
<h4>MIXS ID - {{ term.mixsId }} </h4>

    {% for detail in term.details %}
            <b>Term display name - {{detail.label}}</b>
<br> Structured Comment name - {{term.details.structuredCommentName}}
<br> Definition - {{term.details.definition}}
<br> Expected value - {{term.details.expectedValue}}
<br> Value syntax - {{term.details.valueSyntax}}
<br> Example - {{term.details.example}}
<br> Prefered Unit - {{term.details.preferredUnit}}
<br> Number of occurences permitted - {{term.details.occurence}}
<br>
    {% endfor %}


<br>		
{% endfor %}

