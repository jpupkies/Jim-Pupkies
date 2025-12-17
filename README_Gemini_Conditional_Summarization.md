# Gemini Conditional Summarization

## Overview
This notebook demonstrates **conditional text summarization** using the Google Gemini API via the `google-generativeai` Python SDK. Summaries are generated under explicit constraints for **length, tone, and focus keywords**, enabling controlled and reproducible outputs.

The notebook is **quota-safe by default**, using a simulation mode that produces deterministic placeholder summaries. An optional live mode is included for generating real Gemini outputs without hard-coding API credentials.

## Features
- Conditional summarization under explicit constraints  
- Deterministic, quota-safe simulation mode  
- Optional live Gemini API execution  
- Structured batch processing using `pandas`  
- Step-by-step, portfolio-ready notebook design  

## Skills Demonstrated
- Prompt engineering for controlled LLM outputs  
- Python function abstraction and reuse  
- DataFrame-based input/output workflows  
- Safe API usage patterns for public notebooks  
- Reproducible, professional notebook presentation  

## How to Use
1. Run the notebook top to bottom in simulation mode (default).  
2. Review sample texts and summarization constraints.  
3. Inspect constructed prompts for correctness and clarity.  
4. Generate conditional summaries in a structured DataFrame.  
5. (Optional) Enable live mode by supplying your own Gemini API key securely.

## Screenshots

### Step 2 – Sample Texts and Constraints
Shows the structured input data, including sample texts and explicit summarization constraints used for conditional processing.
<img width="1653" height="528" alt="Step 2 - Sample Text and Constraints" src="https://github.com/user-attachments/assets/9a927443-0f6c-43e9-80a8-a282fd71d4a5" />

### Step 4 – Conditional Summarization Function
Demonstrates the application of the summarization pipeline across the DataFrame, producing controlled summaries under defined constraints.
<img width="1649" height="512" alt="Step 4 - Conditional Summarization Function" src="https://github.com/user-attachments/assets/e9ff8b59-de37-43fb-af41-dd20b8dabbeb" />

### Step 5 – Optional Live Mode
Illustrates the quota-safe live mode toggle, allowing real Gemini API execution without exposing API credentials.
<img width="1648" height="503" alt="Step 5 - Optional Live Mode" src="https://github.com/user-attachments/assets/b8606496-ee33-4c15-a40b-efd286537e2f" />

## Notes
This notebook is designed for **portfolio demonstration**, emphasizing safe API usage, deterministic behavior, and clear separation between simulation and live execution modes.
