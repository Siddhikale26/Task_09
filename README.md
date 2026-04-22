# Task_09
Syracuse Open Data Civic Project

# At Least 3 Interesting Findings / Hypotheses for Further Investigation

## 1. Two-Family Residential Properties Show Disproportionately High Unfit Risk

### Finding
Two-family residential parcels represent a significantly larger share of unfit properties than their share of total parcels.

- Total parcels: ~16.8% are 2-family  
- Unfit properties: ~26.1% are 2-family  

This indicates strong overrepresentation.

### Hypothesis
The elevated unfit risk may be driven by ownership structure (small landlords, absentee owners, deferred maintenance) rather than housing age or assessed value.

### Why Further Investigation is Needed
Current parcel data does not include:
- owner-occupied vs absentee ownership  
- landlord concentration  
- tax delinquency  
- foreclosure history  

Without ownership data, the mechanism remains unproven.

---

## 2. Vacancy Appears More Strongly Associated with Unfit Status than Assessed Value

### Finding
Neighborhoods with higher vacancy rates generally show higher unfit property concentrations, while assessed value shows weak correlation with unfit status.

This suggests neighborhood structural distress may matter more than parcel wealth.

### Hypothesis
Vacancy creates a reinforcing deterioration cycle:

vacancy → reduced oversight → more maintenance decline → more complaints → formal unfit designation

### Why Further Investigation is Needed
Reverse causality is possible:

unfit properties → vacancy

rather than

vacancy → unfit properties

Temporal parcel-level vacancy data is needed to establish sequence.

---

## 3. Post-2022 Increase in Unfit Records May Reflect Enforcement Change, Not Only Housing Decline

### Finding
Unfit property records increased sharply between 2023–2025.

The increase is too steep to assume physical housing deterioration alone.

### Hypothesis
Changes in:
- code enforcement staffing  
- inspection intensity  
- complaint intake systems  
- ordinance enforcement  
- proactive inspections  

may have increased recorded unfit cases.

### Why Further Investigation is Needed
Administrative systems shape observed records.

Without:
- inspection program records  
- staffing data  
- enforcement policy history  

the increase may be misinterpreted as purely worsening housing conditions.

---

# Documentation of LLM-Assisted Analysis with Validation Results

## LLM-Assisted Analysis Process

Large Language Model (LLM) support was used to generate:
- testable hypotheses  
- causal narratives  
- bias checking for research framing  
- competing explanations for observed spatial and temporal patterns  
- weak hypothesis rejection  
- policy-oriented research questions  

The LLM was not used to produce findings directly.

All findings were first established using independently generated statistical analysis and visualization in Python using parcel-level and neighborhood-level data.

The LLM was used only for:
interpretation, hypothesis generation, and critical challenge.

This distinction is important.

LLM output is not evidence.

It is a reasoning assistant.

---

# Validation Method

Each LLM-generated hypothesis was validated against:

## 1. Ground-Truth Visual Analysis

Validation against:
- temporal trend plots  
- neighborhood unfit rate analysis  
- vacancy vs unfit scatterplots  
- land use comparison charts  
- complaint type distributions  
- age comparison distributions  
- assessed value comparisons  
- correlation matrix  
- neighborhood-year heatmaps  

Only hypotheses supported by observed quantitative patterns were retained.

### Example

LLM suggestion:  
“Older buildings are more likely to become unfit”

### Validation Result
Rejected

### Reason
Median construction years were nearly identical between unfit and non-unfit properties (1925 vs 1927), showing weak explanatory power.

---

## 2. Statistical Consistency Checks

Hypotheses were tested against:
- proportional overrepresentation  
- neighborhood rate comparisons  
- correlation strength  
- comparative distributions  

### Example

LLM suggestion:  
“Low assessed value causes unfit status”

### Validation Result
Rejected

### Reason
Correlation between assessed value and unfit status was near zero, and apartment properties had higher values while still showing unfit concentration.

---

## 3. Bias Review of LLM Outputs

LLM-generated narratives were critically reviewed for:
- confirmation bias  
- causal overreach  
- neighborhood stereotyping  
- unsupported poverty assumptions  
- policy bias  
- administrative-data misinterpretation  

### Example

LLM suggestion:  
“Downtown is highest-risk because of poverty”

### Validation Result
Rejected

### Reason
No poverty variable existed in the dataset, and Downtown’s mixed-use structure creates major confounding effects.

---

# Final Validation Outcome

## Accepted Strong Hypotheses

- Vacancy is associated with higher unfit concentration  
- Two-family housing is disproportionately represented  
- Maintenance complaints likely precede formal unfit designation  
- Post-2022 spike may reflect both housing decline and enforcement system change  

---

## Rejected Weak Hypotheses

- Older buildings are inherently more likely to be unfit  
- Low assessed value directly causes unfit status  
- Downtown risk is primarily explained by poverty  
- Open cases automatically indicate enforcement failure  

---

# Research Integrity Note

LLM outputs were treated as hypotheses requiring validation, not as conclusions.

All final claims included in the report were retained only after comparison with observed parcel-level evidence and rejection of unsupported causal assumptions.

This prevented narrative bias and improved methodological rigor.
