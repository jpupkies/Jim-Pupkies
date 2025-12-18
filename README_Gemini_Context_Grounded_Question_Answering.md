# Gemini Context-Grounded Question Answering

## Overview
This notebook demonstrates a deterministic, context-grounded question answering pipeline using the Google Gemini API.  
The model is explicitly constrained to answer **only** from provided context and must return a refusal when the answer cannot be found.  

The notebook emphasizes **production-minded design**, including quota-safe simulation, optional live API execution, and structured evaluation.

---

## Features
- Context-bounded question answering  
- Explicit hallucination prevention rules  
- Deterministic, reproducible prompt construction  
- Quota-safe simulation mode  
- Optional live Gemini API execution  
- Structured pandas outputs for evaluation  
- Inline screenshots demonstrating each step  

---

## Skills Demonstrated
- Prompt engineering for controlled LLM behavior  
- Rule-based LLM output validation  
- API-safe and reproducible execution patterns  
- Integration of structured data (pandas) for NLP tasks  
- Portfolio-ready notebook design  

---

## Sample Data
The notebook includes realistic, professional scenarios for context-grounded QA, including both **answerable** and **unanswerable** questions:

| Context | Question | Expected Behavior |
|---------|---------|-----------------|
| HR policy describing employee benefits eligibility | When do employees become eligible for benefits? | answer |
| Internal IT knowledge base | What is the budget for next quarter? | refusal |
| Performance review workflow | Who approves the company-wide bonus allocations? | refusal |
| IT access requirements | What must a new hire complete before accessing VPN? | answer |

---

## Pipeline Steps
1. **Sample Data (pandas)** – Defines context-question pairs with expected behavior.  
2. **Prompt Construction** – Builds deterministic prompts enforcing strict context-bound answers.  
3. **Simulation Mode Execution** – Tests expected behavior without consuming API quota.  
4. **Optional Live Mode** – Runs real Gemini API calls if enabled.  
5. **Results Table** – Displays simulated and live responses side-by-side.  
6. **Evaluation Column** – Flags pass/fail based on expected behavior.  
7. **Screenshot Display** – Inline visualization of key steps.  

---

## Screenshots

### Step 2 — Sample Data (pandas)
<img width="1566" height="305" alt="Step 2 - Sample Data pandas" src="https://github.com/user-attachments/assets/7baf44e4-b320-4636-b703-e70f87ff99bc" />

### Step 3 — Prompt Construction
<img width="1644" height="345" alt="Step 3 - Prompt Construction" src="https://github.com/user-attachments/assets/9d75a098-687c-4759-9462-ccc8720fbf8d" />

### Step 4 — Simulation Mode Execution
<img width="1581" height="423" alt="Step 4 - Simulation Mode Execution" src="https://github.com/user-attachments/assets/163f198e-00a9-48f7-80f2-073be62c637e" />

### Step 5b — Apply Live Mode over All Rows
<img width="1578" height="546" alt="Step 5b - Apply Live Mode over All Rows" src="https://github.com/user-attachments/assets/4b203b24-eac9-47a9-9bef-b3987596cb6b" />

### Step 6 — Evaluation Column
<img width="1559" height="468" alt="Step 6 - Evaluation Column" src="https://github.com/user-attachments/assets/036cd7bf-9a56-4e12-b1dc-032bb7387dc7" />

---

## Next Steps / Usage
- Toggle `live_mode = True` to run live Gemini API queries.  
- Extend the DataFrame with additional contexts and questions for further testing.  
- Integrate into larger pipelines for document QA, policy validation, or workflow automation.  

---

## Notes
- Simulation mode ensures **quota-safe execution** and reproducibility.  
- Deterministic prompts ensure consistent, **hallucination-free outputs**.  
- This notebook is fully self-contained and ready for **GitHub portfolio presentation**.
