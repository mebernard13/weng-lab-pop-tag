# weng-lab-pop-tag

Methodology for identifying populations in LitCovid publication abstracts. For reference to other relevant repos, please refer to:

- [PICO Parser](https://github.com/Tian312/PICO_Parser)
- [Element Mapping](https://github.com/hl2659/PICOElementMapProject).

## Manual Methodology

### Step 1: Collect PMIDs

PMIDs are 8-digit unique identifiers for each publication within the LitCovid database. Links to respective publications are based on the following hyperlink format:

    https://www.ncbi.nlm.nih.gov/research/coronavirus/publication/ **<pmid>**

### Step 2: Confirm that the publication is within the scope of the COVID-19 PICO project

In order to be within the scope of the project, the publication must be:

1. Related to COVID-19
2. Involving human subjects at the clinical level

Any publications that are on LitCovid and not within the scope should be removed from consideration.

### Step 3: Identify mention of "patients" or "cases" within the abstract

Some abstracts do not have mention of unique sections with the following format or similar (in most cases, the section names would be bolded or italicized and at minimum usually include a colon):

<img src="https://github.com/mebernard13/weng-lab-pop-tag/blob/main/sample_study.png" width="500">

For those situations, just tag the population to the overal Abstract and locate *patient*, *patients*, *case*, *cases* as well as some form of COVID-19 or related severity terminology. Some sample situations are below:

- Critically ill *patients* with SARS-CoV-2
- *Patients* with confirmed COVID-19 pneumonia
- *Cases* of novel coronavirus disease (COVID-19)
- *Patients* with severe disease

To pick up the systematic pattern text, if the *patient* or *case* noun does not have a preposition immediately following *(e.g., of, with, etc.)* then try to include verbiage before the noun that has adjectives/descriptive nouns, especially if they contain words associated with COVID-19 *(e.g., SARS, coronavirus, severe, etc.)*. Otherwise, include both adjectives/descriptive nouns and then the prepositional phrases after the noun mention.

For situations where the abstracts are sectioned off with *(for instance, an Objective, Background, etc.)* then also tag the populations to their appropriate sections.

### Step 4: Create a population tag for the publication of interest

Based on the adjectives associated with the patients involved in the study of interest, select a population tag. Some common ones are shown below:

- COVID-19
- MERS
- SARI

## Installation

*to be completed at a later date*

## Protocol

*to be completed at a later date*
