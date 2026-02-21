# Structured JSON Output Case Study

This repository demonstrates how prompt design can enforce
strictly structured JSON output from a large language model.
The same input domain (platypus biology) is intentionally used
to focus on prompt behavior and output controllability rather
than content variation.

---

## Model Configuration

- Model: GPT-4
- Interaction mode: Chat-based interaction
- Temperature: default
- Top-p: default
- Same input text for all runs

---

## Goal
Produce stable, machine-readable JSON suitable for automated
processing and downstream systems.

---

## Method
- Same task
- Same model
- Same input text
- 3 consecutive runs
- Qualitative evaluation of structure and stability

---

## Structure
- `prompt/` – system and user prompt used to generate JSON output
- `results/` – real model outputs across multiple runs
- `evaluation.md` – observations and conclusions

## Key Result
The prompt consistently produced valid, schema-compliant JSON
across multiple runs. Output variability was limited to wording
only, while structure and field integrity remained stable,
making the results suitable for automation.
