{% include header.html %}

# soil package terms
{% for row in site.data.soil %}
<h4>MIXS ID - {{row.MIXS-ID}} </h4>
<br> **Structured Comment Name -** {{row.structuredCommentName}}
<br> **Example -** {{row.requirement}}
{% endfor %}


# GSC defined terms

Below we list the complete set of terms available accross all checklists and environmental packages. 


{% for term in site.data.terms %}
<h4>MIXS ID - {{ term.mixsId }} </h4>
**Term display name -** {{term.label}}
<br> **Structured Comment name -** {{term.structuredCommentName}}
<br> **Definition -** {{term.definition}}
<br> **Expected value -** {{term.expectedValue}}
<br> **Value syntax -** {{term.valueSyntax}}
<br> **Example -** {{term.example}}
<br> **Prefered Unit -** {{term.preferredUnit}}
<br> **Number of occurences permitted -** {{term.occurence}}
<br>
<br>		
{% endfor %}

