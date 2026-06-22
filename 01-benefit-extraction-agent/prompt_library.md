# Prompt Library — Healthcare Benefit Extraction AI Agent

## Purpose
This prompt library standardizes how unstructured healthcare benefit documents are processed into structured, operational datasets.

It ensures consistency, accuracy, and repeatability in AI-driven benefit extraction workflows.

---

## Prompt 1 — Core Benefit Extraction

### Instruction
Extract structured healthcare benefit data from the provided document.

Return ONLY valid JSON.

Focus on:
- deductible (individual / family)
- out-of-pocket maximum
- primary care copay
- specialist copay
- coinsurance

### Output Format
```json
{
  "plan_name": "",
  "deductible_individual": "",
  "deductible_family": "",
  "out_of_pocket_max": "",
  "primary_care_copay": "",
  "specialist_copay": "",
  "coinsurance": ""
}
Prompt 2 — Data Validation

Compare extracted values against the source text.

Identify:

missing fields
conflicting values
ambiguous benefit definitions

Return a structured validation report.

Prompt 3 — Normalization Rules

Standardize all outputs:

dollar values → numeric format
percentages → consistent % format
naming conventions → uniform field naming across plans
Design Principles

This prompt system is designed for:

high accuracy extraction from healthcare documents
regulatory consistency (ACA / CMS aligned workflows)
scalable automation in TPA/ASO environments
repeatable AI-driven operations
---


Added prompt engineering library for benefit extraction workflow
