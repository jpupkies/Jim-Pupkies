# Gemini Multi-Step Reasoning & Decision Pipeline

## Overview
This notebook demonstrates a **multi-step reasoning pipeline** using the Google Gemini API.  
Given a user query and a set of reference documents, the model performs **chained reasoning**: triaging documents, extracting key facts, generating recommendations, and producing structured outputs.  

The notebook emphasizes **production-minded design**, including deterministic prompt construction, rule-based validation, quota-safe simulation mode, optional live API execution, and structured outputs with pandas.

---

## Features
- Multi-step reasoning pipeline for complex queries
- Deterministic, evidence-grounded prompt construction
- Rule-based validation and priority classification
- Confidence and abstention handling
- Optional live Gemini API execution
- Structured pandas outputs for evaluation
- Inline screenshots for each major step

---

## Skills Demonstrated
- Prompt engineering for multi-document, multi-step reasoning
- Rule-based control to prevent hallucinations or low-confidence outputs
- Integration of pandas for structured output and evaluation
- Safe, reproducible LLM execution patterns
- Clear workflow documentation for portfolio-ready notebooks

---

## Sample Data
Example queries with reference documents:

| Query ID | Query | Documents |
|----------|-------|-----------|
| Q1 | What were the main causes and impacts of the recent Bondi Beach shooting in Sydney? | Bondi Beach incident reports |
| Q2 | Did climate-linked flooding in Southeast Asia displace significant populations in December 2025? | Flooding summaries from multiple countries |
| Q3 | What are the primary debates around gun violence following the Brown University campus shooting? | US campus violence reports |
| Q4 | What specific measures have been proposed by governments in response to recent protests in Bulgaria? | Bulgaria political protest updates |
| Q5 | What long-term economic effects are expected from rising geopolitical tensions involving U.S.–Venezuela maritime actions? | US–Venezuela maritime and sanctions summaries |

---

## Pipeline Steps

1. **Step 1 — Sample Queries & Documents**  
   - Loaded recent news-driven queries and supporting documents.

2. **Step 2 — Gemini Query Interface**  
   - Set simulation mode and defined deterministic interface for candidate answers.

3. **Step 3 — Prompt Construction & Candidate Answers**  
   - Built structured prompts for each query.
   - Generated simulated answers with supporting facts and confidence signals.

4. **Step 4 — Rule-Based Validation & Priority Classification**  
   - Applied rules for priority and abstention decisions.
   - Assigned High / Medium / Low priority levels based on confidence and supporting evidence.

5. **Step 5 — Optional Live Mode / Simulation Review**  
   - Toggle between simulation and live Gemini API execution.
   - Refreshed final structured outputs.

6. **Step 6 — Visualization & Inline Screenshots**  
   - Displayed results in a DataFrame.
   - Embedded step-by-step screenshots for clarity.

7. **Step 7 — Summary, Notes, and Next Steps**  
   - Summarized the workflow.
   - Provided guidance for future use and expansion.

---

## Screenshots

### Step 1
<img width="1628" height="582" alt="Step 1" src="https://github.com/user-attachments/assets/7411674e-093b-4b06-8be1-cb61585481eb" />

### Step 3
<img width="1634" height="690" alt="Step 3" src="https://github.com/user-attachments/assets/6269d7ce-cfef-4205-ade4-0bca261e0dbf" />

### Step 4
<img width="1680" height="506" alt="Step 4" src="https://github.com/user-attachments/assets/ecea9800-4920-49f9-85df-a60f00fc11f5" />

### Step 5
<img width="1637" height="574" alt="Step 5" src="https://github.com/user-attachments/assets/0cee8ae9-5111-46bb-9ca5-c009b9f3d940" />

### Step 6
<img width="1630" height="580" alt="Step 6" src="https://github.com/user-attachments/assets/90e8d552-5075-4924-b01f-52853633368b" />

---

## Next Steps / Usage
- Set `LIVE_MODE = True` to run live Gemini API queries.
- Extend queries and reference documents for broader testing.
- Integrate this multi-step reasoning pipeline into research, reporting, or executive briefing workflows.
- Consider adding additional rule-based checks for domain-specific priorities.

---

## Notes
- Simulation mode ensures **deterministic, quota-safe execution**.
- Confidence signals guide **triaging and abstention**.
- Inline screenshots make the notebook **portfolio-ready** and fully reproducible.
- Structured outputs allow clear evaluation of intermediate and final results.
