# Gemini API Portfolio – Practical Notebook Demonstrations

## Overview
This repository contains a curated set of **portfolio-ready Google Colab notebooks** demonstrating practical, supported usage patterns of the **Google Gemini API** using the `google-generativeai` Python SDK.

Each notebook focuses on a **distinct large language model role** (e.g., summarization, classification, extraction, validation) and is designed to be:
- Deterministic and reproducible
- Quota-safe by default
- Cleanly structured for review
- Accompanied by screenshots and detailed per-notebook documentation

This repository is intended for **technical review**, **portfolio evaluation**, and **demonstration of applied LLM workflows**.

---

## Design Principles
All notebooks in this repository follow these shared constraints:

- ✅ Only confirmed, supported Gemini features  
- ✅ No deprecated or experimental APIs  
- ✅ Quota-safe simulation modes by default  
- ✅ Optional live Gemini execution (no hard-coded keys)  
- ✅ `pandas`-based structured input/output  
- ✅ Step-by-step, screenshot-friendly layout  

---

## Notebook Index

### Text Processing & Control
- **Gemini_Prompt_Demo.ipynb**  
  Core prompt construction and response inspection.

- **Gemini_Text_Rewrite_With_Constraints.ipynb**  
  Controlled rewriting with tone, length, reading level, and meaning preservation.

- **Gemini_Text_Classification_Pipeline.ipynb**  
  Deterministic text classification with structured outputs.

- **Gemini_Conditional_Summarization.ipynb**  
  Constraint-based summarization using length, tone, and focus keywords.

- **Auto_Summary_Pipeline.ipynb**  
  End-to-end automated summarization workflow.

---

### Structured Output & Validation
- **Gemini_Structured_JSON_Extraction.ipynb**  
  Reliable JSON extraction from unstructured text.

- **Gemini_Rule_Grounded_Text_Validation.ipynb**  
  Rule-based validation of LLM outputs against explicit constraints.

---

### Multi-Step & Automation Pipelines
- **Gemini_MultiStep_Text_Automation.ipynb**  
  Chained LLM operations with intermediate validation steps.

- **gemini_batch_prompt_runner.ipynb**  
  Batch prompt execution with reusable automation patterns.

---

### Multimodal
- **Gemini_Image_Analysis_Demo.ipynb**  
  Image understanding and analysis using Gemini’s multimodal capabilities.

---

## Documentation
Each notebook includes its own dedicated README covering:
- Purpose and scope
- Features demonstrated
- Skills highlighted
- Usage instructions
- Screenshot references

Refer to the corresponding `README_*.md` file for notebook-specific details.

---

## Intended Audience
- Hiring managers reviewing applied AI portfolios  
- Engineers evaluating practical Gemini API usage  
- Technical reviewers assessing reproducibility and design discipline  

---

## Notes
This repository emphasizes **clarity, correctness, and professional presentation** over experimental breadth. All examples are designed to run safely in public environments and to reflect real-world usage patterns.
