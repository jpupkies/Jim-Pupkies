# Gemini Document Triage & Action Classification

## Overview
This notebook demonstrates a **document triage and action classification pipeline** using the Google Gemini API.  
Documents such as emails, alerts, and internal notes are classified into **actionable categories**:

- Follow-up Required  
- Informational  
- Escalation Needed  

The notebook emphasizes **production-minded design**, including quota-safe simulation, optional live API execution, and structured evaluation with pandas.

---

## Features
- Deterministic prompt construction for document classification  
- Explicit rules to prevent hallucination or guesswork  
- Quota-safe simulation mode for testing  
- Optional live Gemini API execution  
- Structured pandas outputs for evaluation  
- Step-by-step screenshots for portfolio presentation  

---

## Skills Demonstrated
- Prompt engineering for classification tasks  
- Rule-based validation of LLM outputs  
- Integration with structured data (pandas) for analysis  
- Safe and reproducible execution patterns  
- Production-minded notebook design ready for GitHub  

---

## Sample Data
Example documents and expected classifications:

| Document | Expected Classification |
|---------|------------------------|
| "Reminder: Submit your remote work timesheets for this week by 5 PM today." | Follow-up Required |
| "FYI: The new collaboration feature in our project management tool is now live." | Informational |
| "Alert: Production server is down. Immediate attention required from the DevOps team." | Escalation Needed |
| "Please provide feedback on the draft Q1 marketing strategy deck by end of day tomorrow." | Follow-up Required |
| "Weekly update: Team achieved 95% of sprint goals; planning for next sprint underway." | Informational |

---

## Pipeline Steps
1. **Sample Data** – Defines documents with expected classifications.  
2. **Prompt Construction** – Builds deterministic, rule-based prompts.  
3. **Simulation Mode Execution** – Generates simulated classifications without consuming API quota.  
4. **Optional Live Mode** – Sends prompts to Gemini for live classification (if enabled).  
5. **Results Table & Evaluation** – Compares simulated/live classifications to expected outcomes and flags pass/fail.  
6. **Screenshot Display** – Inline visualization of each major step.  

---

## Screenshots

### Step 2 — Sample Data
<img width="1200" height="401" alt="Step 2 - Sample Data" src="https://github.com/user-attachments/assets/65becc8c-5c85-4182-80ec-8b57f357734b" />

### Step 3 — Prompt Construction
<img width="1608" height="451" alt="Step 3 - Prompt Construction" src="https://github.com/user-attachments/assets/e61c5ea5-ede5-429a-825f-41b3aa31fe7f" />

### Step 4 — Simulation Mode Execution
<img width="1392" height="353" alt="Step 4 - Simulation Mode Execution" src="https://github.com/user-attachments/assets/22bd7e01-6c8a-410e-8fa7-15d9ad6e4e1e" />

### Step 6 — Apply Live Mode
<img width="1624" height="429" alt="Step 6 - Apply Live Mode" src="https://github.com/user-attachments/assets/6487a841-b638-4498-9b88-3caa8a211aa4" />

---

## Next Steps / Usage
- Toggle `live_mode = True` to run live Gemini API queries.  
- Extend the DataFrame with additional documents for testing.  
- Integrate into larger workflows for email triage, reporting, or alert classification.  

---

## Notes
- Simulation mode ensures **safe, deterministic execution** without using API quota.  
- Evaluation columns clearly show pass/fail results against expected classifications.  
- Fully **self-contained, reproducible, and portfolio-ready**.
