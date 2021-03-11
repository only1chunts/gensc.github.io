{% include header.html %}


site map
the page called "implimentation" should be the main Standards front page with the addition of some of the points below.

the "current checklist" page should list the links to the various checklists, and packages as well as containing a link to the "Terms index" i.e. the complete list of terms by ID number



# MIxS 


**The GSC family of minimum information standards (checklists) – Minimum Information about any (x) Sequence (MIxS)**

MIxS currently consists of three separate checklists; **[MIGS for genomes](https://pubmed.ncbi.nlm.nih.gov/18464787 "MIGS/MIMS")**, **[MIMS for metagenomes](https://pubmed.ncbi.nlm.nih.gov/18479204/ "MIGS/MIMS")**, and [**MIMARKS for marker genes**](https://pubmed.ncbi.nlm.nih.gov/21552244/).

To create a single entry point to all minimum information checklists from the GSC and to the environmental packages, we created an overarching framework, the MIxS standard ([publication in Nature Biotechnology](http://www.nature.com/nbt/journal/v29/n5/full/nbt.1823.html)). MIxS includes the technology-specific checklists from the previous MIGS and MIMS standards, provides a way of introducing additional checklists such as MIMARKS, and also allows annotation of sample data using environmental packages.

The three checklists that are currently under MIxS share the same central set of core descriptors, but have checklist specific descriptors as well. Additionally, they enable a detailed description of environment through the use of optional environmental packages.

## Environmental packages

The core MIxS team have developed a series environmental packages which expand on the basic set of mandatory terms to help flesh out metadata expectations for more specific environmental samples. These packages are described more on their individual [pages]().


# A few important notes:

* All dates, times, durations and intervals should be written in ISO 8601 formats
* Units – Strict units are not defined for items in the MIxS checklists, but suggestions are made under “preferred units”, wherever applicable the unit of choice should accompany the value of an item. The units should be in accordance with the The International System of Units (SI)
* If a value is missing, please consider using the INSDC missing value vocabulary:
   * Not applicable - information is inappropriate to report, can indicate that the standard itself fails to model or represent the information appropriately
   * Not collected - information of an expected format was not given because it has not been collected
   * Not provided - information of an expected format was not given, a value may be given at the later stage
   * Restricted access - information exists but can not be released openly because of privacy concerns
   * Missing - its unknown if the data was collected or not

* Notes on using the ENVO terms in the MIxS context are provided [here](https://github.com/EnvironmentOntology/envo/wiki/Using-ENVO-with-MIxS).


# MIxS checklist terms

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

