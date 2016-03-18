# drugtarget
Drug efficacy targets, indications, and pharmacologic class

##Data tables

###Drug target table

**Field**       |**Description**
----------------|----------------------------------------------------
DRUG_ID         |unique identifier assigned to each active ingredient
CHEMBL_ID       |ChEMBL database assigned identifier
DRUG_NAME       |WHO INN name assigned to active ingredient, where available http://www.who.int/medicines/services/inn/en/
TARGET_NAME     |protein(s) name
TARGET_FAMILY   |high level target classification (GPCR, Enzyme, Ion Channel, Transporter, Nuclear Receptor, etc.)
UNIPROT         |Uniprot (http://www.uniprot.org/) accessions for protein targets, multicomponent targets and protein family targets list all Uniprot accessions
GENE            |gene symbol according to HUGO (http://www.genenames.org/)
ACTION_TYPE     |type of modulatory action exerted by drug on protein target
SOURCE          |source of mechanism of action annotation
REFERENCE       |reference for source URL or publication reference

###Drug indication table

**Field**       |**Description**
----------------|----------------------------------------------------
DRUG_ID         |unique identifier assigned to each active ingredient
DRUG_NAME       |WHO INN name assigned to active ingredient, where available http://www.who.int/medicines/services/inn/en/
INDICATION_FDB  |drug indication extracted from OMOP v4 http://archive-omop.fnih.org/CDMvocabV4
UMLS_CUI        |UMLS concept unique identifier http://www.nlm.nih.gov/research/umls/
SNOMEDCT_CUI    |SNOMED-CT concept unique identifier http://www.nlm.nih.gov/research/umls/Snomed/snomed_main.html
DOID            |Disease Ontology identifier http://disease-ontology.org/

###Pharmacologic class table

**Field**       |**Description**
----------------|---------------------------------------------------
DRUG_ID         |unique identifier assigned to each active ingredient
DRUG_NAME       |WHO INN name assigned to active ingredient, where available http://www.who.int/medicines/services/inn/en/
TYPE            |type according to source: FDA - Mechanism of Action (MOA), Physiologic Effect (PE), Chemical Structure (CS), and FDA Established Pharmacologic Class (EPC), MeSH - Pharmacological Action (PA), CHEBI - application (has role)
CLASS_SOURCE_ID |class identifier provided by source
CLASS           |pharmacologic class
SOURCE          |source of classification: MeSH http://www.nlm.nih.gov/mesh/pa_abt.html, FDA http://www.fda.gov/ForIndustry/DataStandards/StructuredProductLabeling/ucm162549.htm, and CHEBI https://www.ebi.ac.uk/chebi/

###LINCS Mappings

**Field**       |**Description**
----------------|----------------------------------------------------
SMILES          |SMILES code for LINCS compounds
DRUG_ID         |unique identifier assigned to each active ingredient
SM_LINCS_ID     |LINCS compound id
DRUG_NAME       |WHO INN name assigned to active ingredient, where available http://www.who.int/medicines/services/inn/en/

