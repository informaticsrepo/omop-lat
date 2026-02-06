# OMOP Laterality
This repository supports study looking at lateral specific concepts



# abstract
(to be pasted later)

# Tables
## Phase 1 results
Percentages quantify what proportion of total events is contributed by a given source concept.
See CSV files above for full results.
This image may be outdated. See files for most up to date results.
It provides a preview of the work.
<img width="965" height="646" alt="image" src="https://github.com/user-attachments/assets/a8f094f7-b1e1-420f-953c-2bc4c588e513" />


# --Additional results--

# Phase 2 results
Considering all diagnoses (phase 2), we found 42192 ICD10CM DiseaseConceptsWithLaterality. These 42192 concepts are mapped to 3747 standard concepts. 

Of those 3747 concepts, 643 concepts distinguish laterality (two seperate concepts for bursitis of left and right shoulder; ICD10CM code of M75.51 mapped to standard concept_id of 762212) and 3103 concepts are DiseaseConceptsWithoutLaterality (pain in right hip and pain in left hip mapped to 'hip pain'; M25.552 mapped to concept_id of 45572430). Proportion wise, 17.2% (643/3747) of standard concepts preserve laterality information from source codes in general diagnosis scope (phase 2). 


# Phase 3
Procedures in ophtalmology:

### Intraocular drug administration
: While source diagnostic data use pre-coordination, procedural data (in CPT [Current procedural terminology]) use potcoordination for drug injection procedures. For example, code 67028 (Intravitreal injection of a pharmacologic agent) is combined with  modifier 50 for bilateral injections and modifiers LT and RT for left and right eye injections. 67028+LT and 67028+RT and 67028+50 may all be mapped to https://athena.ohdsi.org/search-terms/terms/4334590 (Injection of drug into vitreous, SNOMED CT concept code 231755001)  


### Procedure on eye
Also use post-coordination. For example, cataract removal with intraocular lense insertion also use LT and RT modifiers (no use of bilateral modifier)



# Phase 4

Lateral specific procedures (in general)

# Generalization

During our study, we noted that the information loss can be analyzed in general.  
With data on source concepts usage frequency, for each standard concepts with multiple source concepts mapped to it, we can try to identify (and study) any information loss. This can be viewed by some as desired and intended. Others may view this as an information loss and try to avoid it but still keep in mind some optimal granularity of the standard concept model layer. 
Standard concepts are meant to facilitate harmonization. What level of granularity is built into such standard concepts is a design choice of model administrators. To some extend, this granularity level is dictated by available terminologies in existence. For example, the choice of SNOMED CT as a standard terminology for condition domain in 2008. 

