# Gemini Text Rewrite With Constraints

## Overview
This notebook demonstrates how to use the Google Gemini API for **controlled text rewriting under explicit constraints**.  
Instead of free-form generation, the focus is on deterministic, rule-driven transformation of text while preserving meaning.

**Portfolio Goal:** Showcase a practical, production-oriented LLM workflow that is:
- Deterministic and reproducible
- Quota-safe
- Integrated with pandas for structured outputs
- Clear and audit-friendly

---

## Features

- **Constraint-Based Text Rewriting**  
  Text is rewritten under strict rules for tone, length, reading level, and fact preservation.

- **Deterministic Prompt Design**  
  Structured prompts ensure consistent and predictable outputs.

- **Quota-Safe Simulation Mode**  
  Default mode uses deterministic simulation to avoid free-tier API overuse.

- **Optional Live Gemini Mode**  
  Switch to live API calls for production testing or deployment.

- **DataFrame Integration**  
  Supports batch-style inspection of before → after results in pandas.

- **Portfolio-Ready Screenshots**  
  Demonstrates intermediate steps and final results.

---

## Rewrite Constraints

The notebook enforces the following constraints:

1. Maximum length of 120 characters  
2. Tone: formal and neutral  
3. Reading level: general audience  
4. Preserve the original meaning  
5. Do not introduce new facts  

---

## Sample Input Data

Example inputs used in the notebook:

- "The city just passed a bunch of new rules and honestly people are pretty upset about it."  
- "Scientists say that exercising every day is super good for you and can really help with stress and other stuff."  
- "The company said they made a ton of money this quarter and things are looking really great going forward."  
- "A new law was approved, and it changes how housing developments are reviewed by local officials."

**Screenshot:** Step 2 — Sample Text
<img width="1685" height="640" alt="Step 2 - Sample Text" src="https://github.com/user-attachments/assets/61a8c219-f672-4096-b67b-15ca3013be82" />


---

## Deterministic Prompt Design

Each input is converted into a strict prompt that clearly specifies all constraints and instructions to Gemini.

**Screenshot:** Step 3 — Test Prompt
<img width="1689" height="642" alt="Step 3 - Test Prompt" src="https://github.com/user-attachments/assets/e61c2b6e-8927-466c-97b1-92f45a0ecc75" />


---

## Testing the Function

The notebook includes a **quota-safe simulated rewrite function**, demonstrating the expected outputs under the defined constraints.

**Screenshot:** Step 4 — Testing the Function
<img width="1681" height="137" alt="Step 4 - Testing the Function" src="https://github.com/user-attachments/assets/18a95fed-7efd-486a-8836-d85846d8229c" />


---

## Results

Rewriting is applied to all inputs, producing a **before → after DataFrame**.

**Screenshot:** Step 5 — Constrained Rewrite Results
<img width="1682" height="554" alt="Step 5 - Constrained Rewrite Results" src="https://github.com/user-attachments/assets/e4fdbfab-08c0-4b32-acec-35e121d13c46" />


---

## Usage Instructions

1. Modify `REWRITE_CONSTRAINTS` to fit different use cases.  
2. Add new text entries to the DataFrame.  
3. Run `rewrite_text()` in simulated mode for safe testing.  
4. Switch to `mode="live"` for real Gemini API execution.

---

## Skills Demonstrated

- Constraint-based LLM usage  
- Deterministic prompt construction  
- Quota-safe workflow design  
- DataFrame integration for structured outputs  
- Production-oriented LLM pipeline design  

This notebook illustrates how large language models can be used as **reliable transformation tools**, not just creative generators, with **clear rules and reproducible behavior**.
