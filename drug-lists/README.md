## About
This folder contains the drug code lists created using BNF treatment summaries for the agreed list of conditions

### Folder and file structure

The lists for each drug are contained within a single folder, named after the drug class, e.g. `Benzodiazepines`.
Within the folder, there are the following files:
- the drug codes for that medication as found in the [CEGEDIM data](https://www.cegedim-health-data.com/solutions/real-world-data-evidences/patient-cohort/)
- the drug codes for that medication as found in [CPRD](https://cprd.com/primary-care-data-public-health-research) AURUM, the Clinical Practice Research Datalink, using EMIS clinical systems
- the drug codes for that medication as found in [CPRD](https://cprd.com/primary-care-data-public-health-research) GOLD, the Clinical Practice Research Datalink, using InPS Vision clinical systems
- the drug codes for that medication as found in [IMRD](https://www.iqvia.com/library/fact-sheets/uk-emr-iqvia-medical-research-data), the Iqvia Medical Research Data
- the drug codes for that medication as found in [UHB](https://www.research.uhb.nhs.uk/), the University Hospitals Birmingham data.

Each file contains the following columns (this information is copied from the [CodeBuilder documentation](https://github.com/krisgoks/markdowns/blob/master/codebuilder/codebuilderintro.md) written by Krishna Gokhale)
- `Drug code id`: the actual term stored in the drug database that represents the code you are looking for, this might be a number, a short string, or a hexadecimal value
- `Description`: the text description of the drug code, this will also include (where available) the drug substance, strength, route of administration etc.
- `BNF1`, `BNF2`:, `BNF3`: The [British National Formulary (BNF)](https://digital.nhs.uk/data-and-information/areas-of-interest/prescribing/practice-level-prescribing-in-england-a-summary/practice-level-prescribing-glossary-of-terms) codes from this pseudo-classification are used in the prescribing dataset as a unique identifier to show what was prescribed.
- `ATC`: the code for this drug in the [Anatomical Therapeutic Chemical Classification System](https://www.whocc.no/) (ATC). The ATC is a drug classification system that classifies the active ingredients of drugs according to the organ or system on which they act and their therapeutic, pharmacological, and chemical properties.
- `Database`: the database to which this information applies

### How to use

You can use either drug_code_id (*usually local database identifiers), BNF, ATC code or even the Description columns for the databases relevant to your study.

Note that the BNF and ATC code is not always populated, and the dm+d code is in the pipeline for Code Builder to include as part of the code list outputs so these can be used for query.

#### Example snippet

Below is an example approach code snippet of using postgresql to filter out the list of unique_identifiers for a chosen drug in your data source

```postgresql
--using term sets:
SELECT unique_identifier, * 
FROM drug_dictionary
WHERE description IN (
    'add',
    'term descriptions',
    'here' 
    )
LIMIT 10;

--OR using code sets:
SELECT unique_identifier, * 
FROM drug_dictionary
WHERE drug_id in (
    'bnfcode',
    'dmdcode',
    'atccode' 
    )
LIMIT 10;

-- these can then be joined on patient tables to identify relevant cohorts