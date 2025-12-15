# Gemini Rule-Grounded Text Validation Demo

## Overview
This notebook demonstrates a **rule-grounded text validation pipeline** using the Google Gemini API.  
It evaluates short text entries against explicit rules, producing **structured, deterministic outputs** suitable for data quality, content moderation, or editorial enforcement.

**Portfolio Goal:** Showcase practical LLM usage in a quota-safe, reproducible way, without embeddings or experimental features.

---

## Features

- **Deterministic Validation:** Text is only evaluated against rules, never rewritten.  
- **Structured Output:** Each entry returns a JSON-like result with:
  - `is_valid`: Boolean indicating if text passes all rules
  - `violations`: List of broken rules (empty if none)
- **Quota-Safe Simulation:** Default mode is fully reproducible and safe for free-tier API usage.  
- **Optional Live Gemini Mode:** Switch to `mode="live"` for real API validation.  
- **Portfolio-Ready:** Screenshots and clear DataFrame outputs included.

---

## Validation Rules
1. Text must be 280 characters or fewer.  
2. Text must be written in complete sentences.  
3. Text must not contain profanity or hate speech.  
4. Text must clearly relate to a news or informational topic.  

---

## Sample Data
A small dataset includes valid entries, invalid entries, and edge cases for demonstration:

- `The city council approved a new housing development after a lengthy public hearing.` ✅  
- `Breaking news!!! This is absolute garbage and everyone knows it.` ❌  
- `A new study shows that daily exercise can significantly reduce stress levels and improve overall health.` ✅  
- `lol this makes no sense` ❌  
- `The company announced record quarterly earnings, exceeding analyst expectations.` ✅  

**Screenshot:** Step 2 — Sample Text
<img width="1718" height="644" alt="Step 2 - Sample Text" src="https://github.com/user-attachments/assets/a392e869-db58-4abd-bf05-b1d98687ea19" />

---

## Deterministic Prompt
Each text is converted into a strict JSON prompt for Gemini, ensuring reproducible evaluation:

**Screenshot:** Step 3 — Test Prompt
<img width="1723" height="650" alt="Step 3 - Test Prompt" src="https://github.com/user-attachments/assets/403e824d-03fe-4990-bfb7-8b60133fadf0" />

---

## Usage
1. Modify or expand `VALIDATION_RULES` to suit different use cases.  
2. Add text entries to the DataFrame.  
3. Run `validate_text()` in `simulated` mode for safe testing.  
4. Optionally switch to `live` mode for real Gemini evaluation.

---

## Skills Demonstrated
- Rule-grounded LLM usage  
- Deterministic JSON output handling  
- Quota-safe pipeline design  
- Portfolio-ready Colab notebook with screenshots  
- DataFrame integration and structured results
