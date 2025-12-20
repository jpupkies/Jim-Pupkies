# Gemini Context-Grounded Question Answering

## Overview
This notebook demonstrates a **multi-document, context-grounded question answering (QA) pipeline** using the Google Gemini API.  
Given a user query and a set of reference documents, the model provides **answers strictly grounded in the provided sources**, with explicit refusal if the answer is not present in the documents.

The notebook emphasizes **production-minded design**, including deterministic prompt construction, quota-safe simulation mode, optional live API execution, and structured pandas outputs for evaluation.

---

## Features
- Multi-document ingestion for evidence-based QA
- Deterministic, rule-based prompt construction
- Quota-safe simulation mode for testing without API usage
- Optional live Gemini API execution
- Structured evaluation comparing model outputs to expected answers
- Step-by-step screenshots for documentation and clarity

---

## Skills Demonstrated
- Prompt engineering for evidence-grounded responses
- Rule-based control to prevent hallucinations
- Structured multi-document reasoning pipelines using pandas
- Safe, reproducible LLM execution patterns
- Clear workflow documentation and reproducible notebook design

---

## Sample Data
Example queries with multiple reference documents and expected answers:

| Query ID | Query | Documents | Expected Answer |
|----------|-------|-----------|----------------|
| 1 | What were the main reasons for the recent NHS doctors' strike? | Multiple documents detailing pay erosion and training bottlenecks | The strike was primarily due to real-term pay erosion and career/training bottlenecks affecting NHS resident doctors. |
| 2 | Why were thousands of flights grounded recently worldwide? | Multiple documents about airline system outage | The worldwide flight grounding was caused by a major airline system outage due to software fragility in flight management systems. |
| 3 | Summarize the impact of the new analytics features on user engagement. | Documents about Q2 product launch and feedback | The new analytics features increased user engagement, with potential infrastructure requirements to support growth. |

---

## Pipeline Steps
1. **Sample Data** — Load queries, reference documents, and expected answers  
2. **Prompt Construction** — Build deterministic, evidence-grounded prompts  
3. **Simulation Mode Execution** — Generate quota-safe placeholder answers  
4. **Optional Live Mode** — Send prompts to Gemini for live QA (if enabled)  
5. **Results & Evaluation** — Compare simulated/live answers with expected answers  
6. **Screenshots** — Inline visualization for each major step

---

## Screenshots

### Step 2 — Sample DataFrame
<img width="1585" height="647" alt="Step 2 - Sample DataFrame" src="https://github.com/user-attachments/assets/319c39f3-020d-4c98-9293-f44a87997e59" />

### Step 3 — Apply Prompt Construction
<img width="1630" height="685" alt="Step 3 - Apply Prompt Construction" src="https://github.com/user-attachments/assets/f49abd62-01f6-431e-a468-b51d3ed9d8ad" />

### Step 4 — Apply Simulation Mode
<img width="1574" height="504" alt="Step 4 - Apply Simulation Mode" src="https://github.com/user-attachments/assets/1186fef8-a449-45ed-a3bc-a624752f661a" />

### Step 5 — Apply Live Mode
<img width="1432" height="502" alt="Step 5 - Apply Live Mode" src="https://github.com/user-attachments/assets/d43ee42f-ff4e-49c1-8b23-a81375edeaa7" />

### Step 6 — Apply Evaluation
<img width="1524" height="610" alt="Step 6 - Apply Evaluation" src="https://github.com/user-attachments/assets/6fbd8eac-fd3c-42cb-86e9-441da4f5bf39" />

---

## Next Steps / Usage
- Toggle `live_mode = True` to run live Gemini API queries  
- Add additional queries and reference documents for extended testing  
- Integrate this QA pipeline into research, reporting, or executive briefing workflows  

---

## Notes
- Simulation mode ensures **deterministic, quota-safe execution**  
- Evaluation column provides a **simple, reproducible measure of alignment** with expected answers  
- Fully **self-contained and reproducible**
