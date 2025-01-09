## About
This folder contains the drug lists themselves

### Folder and file structure

The lists for each drug are contained within a single folder, named after the category of drug, e.g. `Benzodiazepines`.
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
The code lists are in csv format so can be loaded using your preferred methods, for example, using a pandas dataframe or into a SQL table. You can then use the code lists to extract the BNF/ATC codes, or to extract drug class specific term strings to query another data source or populate a cohort.
