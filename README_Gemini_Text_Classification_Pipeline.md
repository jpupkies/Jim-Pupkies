# Gemini Text Classification Pipeline

## Overview
This notebook demonstrates a **text classification workflow** using the Google Gemini API (`google-generativeai` Python SDK`). It is designed for **portfolio presentation**, fully reproducible in Google Colab, and can run **quota-safe** without live API calls. The workflow highlights: **Structured text classification**, **Deterministic label mapping**, **pandas integration** for batch processing, and **Quota-safe simulation mode**.

## Features
- Closed-set text classification
- Deterministic simulation mode for quota safety
- Optionally plug in live API calls
- Clear demonstration of real-world NLP workflow
- Easily extendable to new categories or larger datasets

## Notebook Steps

**Step 1 — Install & Import Libraries**  
Installs required packages and imports essential modules:

```python
!pip install --quiet google-generativeai pandas
import pandas as pd
import google.generativeai as genai
from IPython.display import display
```

**Step 2 — Prepare Sample Classification Data**  
A sample DataFrame is created with news-relevant text entries. This simulates real-world classification scenarios.

**Screenshot:**  
<img width="1726" height="626" alt="Step 2 — Prepare Sample Classification Data (Sample DataFrame)" src="https://github.com/user-attachments/assets/908627dd-4fe1-4f0b-a2af-5f6580129c64" />

**Step 3 — Define Classification Categories & Prompt Template**  
- Categories used in this notebook:  
```python
CATEGORIES = ["Politics", "Technology", "Economy", "Cybersecurity", "World Affairs"]
```  
- Prompt template is defined to produce a **single-label classification**.

**Step 4 — Classification Function (Quota-Safe)**  
Supports two modes: 1. **Simulation mode (default)** — no API calls, always runs 2. **Live mode** — plugs into Gemini API when quota allows. Simulated mode uses keyword mapping to return deterministic categories. Live mode integrates `genai.GenerativeModel("gemini-2.5-flash")`.

**Step 5 — Apply Classification & Display Results**  
- Applies the classification function to each row of the DataFrame.  
- Stores results in a new column `category`.  
- Displays the final structured DataFrame.

**Screenshot:**  
<img width="1725" height="482" alt="Step 5 — Apply Classfication   Display Results (Apply Function)" src="https://github.com/user-attachments/assets/90f410b5-f1ad-40ef-8a75-d14e26091043" />

## Usage Notes
- Fully quota-safe by default  
- Easy to convert to live API calls by setting `USE_LIVE_API = True`  
- Categories can be customized for different domains  
- API keys should **never** be committed

## Skills Demonstrated
- Text classification pipelines  
- Deterministic simulation for reproducibility  
- pandas-based batch processing  
- Quota-safe, portfolio-ready design  
- Integration-ready structure for real API calls

## Optional Extensions
- Extend categories for multi-class classification  
- Integrate live Gemini calls when quota allows  
- Add confidence scoring or validation steps  
- Combine with multi-step automation or structured JSON extraction
