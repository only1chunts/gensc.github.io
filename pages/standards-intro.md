{% include header.html %}
 
 
# Minimum Information about any Sequence (MIxS)

The current versions of the GSC family of minimum information standards (MIxS - Minimum Information about any (x) Sequence)
 are available below. We have provided the information in sections to enable users to understand the relationships between the various levels of complexity. You may wish to refer to our glossary (bottom of this page) of terminology. 
In addition, we maintain a [GitHub repository](https://github.com/GenomicsStandardsConsortium/mixs) where the next versions are being developed and discussed, please feel free to join the discussion using the github issue tracker. The [GitHub Wiki](https://github.com/GenomicsStandardsConsortium/mixs/wiki) in that repository also contains some more techincal specifications. 

You can find all previous versions of the checklistsin our [mixs-legacy GitHub](https://github.com/GenomicsStandardsConsortium/mixs-legacy) repository.



## Checklists

As of release 5.0, the following checklists are under the MIxS umbrella:
- MIGS: Minimum information about a genome sequence. see [publication](https://pubmed.ncbi.nlm.nih.gov/18464787)
- MIMS: Minimum information about a metagenome sequence. see [publication](https://pubmed.ncbi.nlm.nih.gov/18479204/)
- MIMARKS: Minimum information about a marker gene sequence. see [publication](https://pubmed.ncbi.nlm.nih.gov/21552244/)
- MISAG: Minimum information about a single amplified genome sequence. see NEED TO ADD [publication]()
- MIMAG: Minimum information about a metagenome-assembled genome sequence. see NEED TO ADD [publication]()

MIGS and MIMARKS are further divided into additional subchecklists, based on the genome sequence in question, or the sequencing type.
- MIGS-EU: [MIGS for eukaryotic genome sequences](standards/mig_eu_min.html)
- MIGS-BA: MIGS for bacterial and archaeal genome sequences
- MIGS-PL: MIGS for plasmid sequences
- MIGS-VI: MIGS for viral genome sequences
- MIGS-ORG: MIGS for organelle sequences
- MIMARKS-SP: MIMARKS-survey  for marker gene sequences obtained directly from the environment
- MIMARKS-SU: MIMARKS-specimen for marker gene sequences from cultured or voucher-identifiable specimens


## Core and specific descriptors
All checklists share the same central set of core (Minimum) descriptors, which are:
- **investigation type**
- **project name**
- **geographic location (latitude and longitude)**
- **geographic location (country and/or sea,region)**
- **collection date**
- **environment (biome, feature, and material)**
- **sequencing method**

Each checklist is then defined by additional type-specific descriptors. These specific descriptors are summarized below for each checklist and subchecklist. Please note that this summary only includes minimum information for each sequence type, meaning that other conditional and optional descriptors are not included. 

### MIGS-EU
- isolation and growth condition
- assembly quality
- assembly software
- number of contigs

### MIGS-BA
- number of replicons
- reference for biomaterial
- isolation and growth condition
- assembly quality
- assembly software
- number of contigs

### MIGS-PL
- propagation
- isolation and growth condition
- assembly software

### MIGS-VI
- propagation
- isolation and growth condition
- assembly software

### MIGS-ORG
- isolation and growth condition
- assembly software

### MIMS

### MIMARKS-S
- target gene

### MIMARKS-C
- isolation and growth condition
- target gene

### MISAG
- taxonomic identity marker
- assembly quality
- assembly software
- completeness score
- completeness software
- contamination score 
- sorting technology
- single cell lysis approach
- WGA amplification approach

### MIMAG
<details>
<summary> Click to show mandatory terms.</summary>

  * taxonomic identity marker<br>
  * assembly quality<br>
  * assembly software<br>
  * completeness score<br>
  * completeness software<br>
  * contamination score<br> 
  * binning parameters<br>
  * binning software
</details>

## Extensions
In order to encourage more comprehensive metadata inclusion with sequence data the GSC have encouraged the development of many extensions that can be used in addition to the Minimum Information for each checklist. These extnesions consist of many recomended terms that have been compiled by experts in the relevant field of research. Explore all the ready made checklist extensions that we have [available](/pages/standards/mixs-ext-and-profiles.html).
If there is not a suitable checklist already available and you are interested in developing your own extention, [this page](/pages/standards/mixs-ext-and-profiles.html) also contains details on Developing Extensions that you may find useful.




## [Compliance and Implementation](standards/compliance.html)
Details of how to comply with the standard, and which repositories and institutions are currently making use of them

## [The Terms](standards/all-terms.html)
The complete set of terms defined across all of the checklists and packages can be found [here](standards/all-terms.html).
If you are interested in a specific term or terms, we provide a [simple search](standards/search-terms.html) function to aid you in finding the relevant term(s).


## Terminology (GSC parlance) :

- **MIxS checklists** - Used to refer to the entire collection of all checklists under the MIxS umbrella, or replace the MIxS with a specific Checklist to refer to any individual complete collection of terms, such as MIGS or MIMAGS checklists.

- **Sub-checklist or Type-Specific checklists** - User to refer to the subdivisions of checklists within any of the main checklist types, e.g. MIGS is a checklist, MIGS-EU is a sub-checklist of MIGS. (Note. This terminology is rarely used, often the sub-checklists are simply refered to as checklists).

- **Package / Extension / Environmental Package** - These are the collections of recomended terms as developed by community experts and ratified by the GSC members, the most commonly reused packages tend to be related to specific environments. As we move to the RDF implementation of MIxS it is expected that individual projects will start to create their own specific packages, hence to move away from "environmental packages" to just "packages".

- **Core** - Historically we have refered to the set of terms that could be used in any checklist as being "core", but we now more strictly define the core as those terms which are the Mandatory or Conditional Mandatory in ANY individual (specific) checklist.

- **Term / Item / Descriptor / Attribute** - There is some historical flexibility in how we have refered to the attribute terms over the years, sometime they are refered to as Items, Terms or Descriptors. We would like to unify this, and to now only use the word "terms" to mean the individual attribute terms within the checklists. Each term is uniquely defined and given its own URI. See the [terms page](standards/all-terms.html) for a complete list of all terms.

- **Sections** - All the terms are allocated into sections to aid checklist development. These sections are;

        **Investigation** - terms that relate the project and linking it other electronic resources
		
		**Nucleic acid sequence source** - terms that are about where and how the DNA sample was created
		
		**Sequencing** - terms that relate to how the DNA sample was processed for sequencing
		
		**Environmental** - terms that relate to the environment from which the sample/DNA was obtained
		
The packages tend to focus on the Environmental section terms, whilst the other sections are largely covered in the checklists and sub-checklists.


