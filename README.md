# drugtarget
Drug efficacy targets and indications

##Data tables

###Drug target table

**Field**   |**Description**
____________|_____________________________________________________
DRUG_ID     |unique identifier assigned to each active ingredient
CHEMBL_ID   |ChEMBL database assigned identifier
DRUG_NAME   |WHO INN name assigned to active ingredient, where available
TARGET_NAME |protein(s) name
UNIPROT     |Uniprot accessions for protein targets, multicomponent targets and protein family targets list all Uniprot accessions
ACTION_TYPE |type of modulatory action exerted by drug on protein target
SOURCE      |source of mechanism of action annotation
REFERENCE   |reference for source, *EXPERT CURATOR* do not have any reference assigned

###Drug indication table

**Field**      |**Description**
_______________|_____________________________________________________
DRUG_ID        |unique identifier assigned to each active ingredient
DRUG_NAME      |WHO INN name assigned to active ingredient, where available
INDICATION_FDB |drug indication extracted from OMOP v4
UMLS_CUI       |UMLS concept unique identifier
SNOMEDCT_CUI   |SNOMED-CT concept unique identifier
DOID           |Disease Ontology identifier
