# Healthcare Benefit Extraction AI Agent

## Problem Statement
Healthcare benefit documents (SBCs, OOCs, and policy files) are unstructured, inconsistent, and time-consuming to interpret manually. This creates operational delays and increases the risk of configuration errors in downstream TPA/ASO systems.

---

## Solution Overview
This project demonstrates an AI-powered extraction framework that converts unstructured healthcare benefit documents into structured, standardized data formats suitable for operational use.

The solution uses prompt engineering principles and LLM-style reasoning to extract and normalize key benefit attributes.

---

## Inputs
- Summary of Benefits and Coverage (SBC)
- Outline of Coverage (OOC)
- Plan policy documents (PDF/text-based content)

---

## Outputs
Structured benefit dataset including:
- Deductible (individual / family)
- Out-of-pocket maximum
- Primary care copay
- Specialist copay
- Coinsurance values
- Plan identifiers

Output format: JSON / Excel-ready structure

---

## Example Output

```json
{
  "plan_name": "Silver PPO 2026",
  "deductible_individual": 1500,
  "deductible_family": 3000,
  "out_of_pocket_max": 8000,
  "primary_care_copay": 25,
  "specialist_copay": 50,
  "coinsurance": "20%"
}
