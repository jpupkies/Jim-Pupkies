# Gemini Multi-Step Reasoning & Decision Pipeline

## Overview
This notebook demonstrates a **multi-step reasoning pipeline** using the Google Gemini API.  
Given a set of company reports or documents, the pipeline performs **triaging, key fact extraction, risk evaluation, recommendation generation, and structured output production**.

The notebook emphasizes **production-minded design**, including deterministic prompt construction, quota-safe simulation mode, optional live API execution, decision logic, and structured pandas outputs for evaluation.

---

## Features
- Multi-document ingestion and structured analysis  
- Multi-step reasoning with chained Gemini prompts  
- Quota-safe simulation mode for testing without API usage  
- Optional live Gemini API execution  
- Risk-based prioritization and recommendation logic  
- Inline screenshots for step-by-step visualization

---

## Skills Demonstrated
- Multi-step reasoning and prompt chaining with LLMs  
- Conditional logic and rule-based decision-making  
- Structured outputs using pandas DataFrames  
- Evaluation of intermediate and final outputs  
- Visualization of priority levels and recommendations  
- Clear, reproducible workflow for portfolio presentation

---

## Sample Data
Example documents for testing:

| Document Title                  | Content Summary |
|---------------------------------|----------------|
| Q1 Financial Report              | Revenue up 12%, operating costs up 5%, potential supply chain risk |
| Customer Feedback Summary        | Satisfaction improved 8%, some delivery complaints |
| Market Analysis Report           | Competitor gaining market share, AI adoption opportunities |
| Internal Audit Report            | Minor compliance issues identified |
| Product Development Update       | Prototype ready, potential component shortages |

---

## Pipeline Steps
1. **Sample Data** — Load documents and define the analysis scenario  
2. **Simulation Mode** — Enable quota-safe testing and define a Gemini simulation function  
3. **Multi-Step Reasoning** — Extract summaries, key facts, and recommendations from each document  
4. **Evaluation** — Assess completeness of outputs and detect missing information  
5. **Decision Logic** — Assign priority levels and highlight risks and recommendations  
6. **Visualization & Reporting** — Display priority counts and print structured recommendations  
7. **Screenshots** — Inline documentation of each step

---

## Screenshots

### Step 1 — Notebook Setup
<img width="1197" height="58" alt="Step 1" src="https://github.com/user-attachments/assets/2b25252f-3901-4ddb-9fa0-53cce681ee65" />

### Step 3 — Sample Documents
<img width="809" height="50" alt="Step 3" src="https://github.com/user-attachments/assets/b726b69e-bc7a-420d-b804-d9c6a08eef65" />
<img width="973" height="52" alt="Step 3b" src="https://github.com/user-attachments/assets/c8122ae8-26b6-4c5e-b246-fcc31fc67d7a" />

### Step 4 — Multi-Step Reasoning Pipeline
<img width="1647" height="623" alt="Step 4" src="https://github.com/user-attachments/assets/8148c565-2d74-413d-bb63-ce246997c8b6" />

### Step 5 — Evaluation
<img width="1688" height="635" alt="Step 5" src="https://github.com/user-attachments/assets/5e5ba36b-ce59-4df8-bf5e-927155648af2" />

### Step 6 — Decision Logic
<img width="1649" height="532" alt="Step 6" src="https://github.com/user-attachments/assets/a09b7551-d422-410a-aae2-cab944bb7faf" />

### Step 7 — Visualization & Reporting
<img width="1776" height="808" alt="Step 7" src="https://github.com/user-attachments/assets/d2876a3a-e20d-405c-b4a8-78bb4e605bec" />

---

## Example Structured Output
| Document Title                  | Priority | Risks Identified                       | Recommendation                                         |
|---------------------------------|----------|---------------------------------------|-------------------------------------------------------|
| Q1 Financial Report              | High     | Supply chain risk noted                | Mitigate supply chain risks by securing alternative suppliers |
| Customer Feedback Summary        | Normal   | No significant risks                   | Optimize logistics and improve shipment communication |
| Market Analysis Report           | Normal   | No significant risks                   | Invest in AI to maintain competitive advantage       |
| Internal Audit Report            | High     | Minor compliance issues                | Strengthen internal controls and conduct quarterly compliance checks |
| Product Development Update       | High     | Risk of component shortages            | Secure multiple suppliers to mitigate supply chain risks |

---

## Next Steps / Usage
- Toggle `SIMULATION_MODE = False` to run live Gemini API queries  
- Extend the pipeline with additional decision rules or document types  
- Integrate into dashboards or reporting systems for automated insights  

---

## Notes
- Simulation mode ensures **deterministic, quota-safe execution**  
- Decision logic allows **high-priority documents to be flagged automatically**  
- Fully **self-contained and reproducible** for portfolio presentation
