# Structured JSON Output — Business Case (B2B Lead Analysis)

## Overview

This repository demonstrates a production-oriented LLM prompt design
focused on strict structured JSON output for real business use cases.

The case simulates a B2B SaaS lead analysis system, where inbound customer
messages are automatically classified, scored, and routed using an LLM.

The output is designed to be:
- machine-readable;
- schema-valid;
- automation-ready;
- suitable for CRM / BI / sales pipelines.

---

## Business Problem

B2B SaaS companies receive high volumes of inbound messages via:
- website forms;
- emails;
- chat widgets;
- CRM integrations.

Manual triage does not scale.

---

**Goal:**  
Use an LLM to transform unstructured text into structured business intelligence
that can drive automated decision-making.

---

## Output Capabilities

The model produces:
- lead classification
- intent analysis
- estimated business value
- risk assessment
- recommended sales action
- confidence score

All outputs strictly follow a predefined JSON schema.

---

## Repository Structure
```
structured-json-output-case/
│
├─ README.md
├─ requirements.txt
│
├─ prompts/
│   ├─ system_prompt.txt
│   ├─ user_prompt.txt
│
├─ schemas/
│   └─ lead_analysis.schema.json
│
├─ examples/
│   ├─ input_example.txt
│   └─ output_example.json
│
├─ validation/
│   └─ model.py
│
└─ pipeline/
    └─ run.py

```

---

## Typical Production Flow
```
Inbound message
↓
LLM (structured prompt)
↓
JSON validation
↓
CRM / Sales Routing / Analytics

```

---

## Why This Matters

This project demonstrates:
- disciplined prompt engineering;
- schema-first design;
- LLMs as decision-support systems;
- real-world business reasoning (LTV, risk, prioritization).

---

## Possible Extensions

- Confidence threshold routing;
- Prompt versioning;
- Output evaluation & scoring;
- Multi-model comparison;
- CRM webhook integration.

