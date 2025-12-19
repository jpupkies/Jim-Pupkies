# Gemini Multi-Audience Summarization

## Overview
This notebook demonstrates a **multi-audience summarization pipeline** using the Google Gemini API.  
Given a single source document, the model generates **separate summaries tailored to different audiences**, such as executives, technical teams, and general stakeholders.

The notebook emphasizes **production-minded design**, including deterministic prompt construction, quota-safe simulation mode, optional live API execution, and structured pandas outputs.

---

## Features
- Audience-specific summarization from a single source document
- Deterministic, rule-based prompt construction
- Quota-safe simulation mode for testing
- Optional live Gemini API execution
- Structured pandas outputs for evaluation
- Step-by-step screenshots for portfolio presentation

---

## Skills Demonstrated
- Prompt engineering for controlled, audience-aware generation
- Rule-based LLM behavior enforcement
- Structured NLP pipelines using pandas
- Safe and reproducible API usage patterns
- Production-minded notebook design suitable for GitHub portfolios

---

## Sample Data
Example source documents and intended summaries:

| Document ID | Audience | Summary Intent |
|------------|----------|----------------|
| 1 | Executive | High-level implications on healthcare operations and workforce challenges |
| 1 | Technical | Detailed causes of strikes, statistical polling data, and systemic healthcare bottlenecks |
| 1 | General | Plain-language overview of the doctor strike and why it matters to everyday people |
| 2 | Executive | High-level risks to airline operations and regulatory concerns |
| 2 | Technical | System-level causes of the outage and implications for engineering teams |
| 2 | General | Simplified explanation of the airline outage for everyday travelers |

---

## Pipeline Steps
1. **Sample Data** – Defines source documents with audiences and intended summary goals  
2. **Prompt Construction** – Builds deterministic, audience-aware prompts  
3. **Simulation Mode Execution** – Generates quota-safe placeholder summaries  
4. **Optional Live Mode** – Sends prompts to Gemini for live summarization (if enabled)  
5. **Results Table & Evaluation** – Compares simulated/live summaries and provides qualitative evaluation  
6. **Screenshot Display** – Inline visualization of each major step

---

## Screenshots

### Step 2 — Sample DataFrame
<img width="1724" height="695" alt="Step 2 - Sample DataFrame" src="https://github.com/user-attachments/assets/166fba53-d619-4df7-9b30-42eb9304d34e" />

### Step 3 — Apply Prompt Construction
<img width="1673" height="691" alt="Step 3 - Apply Prompt Construction" src="https://github.com/user-attachments/assets/639f85ee-a639-4c5f-beef-e5d0bb415e33" />

### Step 4 — Apply Simulation
<img width="1567" height="416" alt="Step 4 - Apply Simulation" src="https://github.com/user-attachments/assets/0b706958-10ea-44d4-89c3-1c4d6922e16c" />

### Step 5 — Apply Live Gemini API Mode
<img width="1569" height="297" alt="Step 5 - Apply Live Gemini API Mode" src="https://github.com/user-attachments/assets/fb145b6f-6b6a-4261-8db0-df406323f7cb" />

### Step 6 — Apply Evaluation Column
<img width="1568" height="468" alt="Step 6 - Apply Evaluation Column" src="https://github.com/user-attachments/assets/c2627ecf-0823-4682-a448-c696ae75fdd8" />

---

## Next Steps / Usage
- Toggle `live_mode = True` to run live Gemini API queries  
- Extend the DataFrame with additional documents and audiences for broader testing  
- Integrate into larger workflows for reporting, executive briefings, or educational summaries  

---

## Notes
- Simulation mode ensures **safe, deterministic execution** without using API quota  
- Evaluation column demonstrates **structured review and quality control**  
- Fully **self-contained, reproducible, and portfolio-ready**
