# Gemini Prompt Demo Notebook

## Overview
This notebook demonstrates **interactive multimodal prompt testing** using Google Gemini. Users can input text prompts and upload images to generate content responses. The notebook is designed to be **GitHub-safe**: the API key is never stored in the notebook, and screenshots illustrate the workflow.

---

## Features
- Interactive prompt interface with text input and model selection.
- Image upload and analysis using Gemini multimodal models.
- Safe API key entry using `getpass` (no keys are stored in the notebook).
- Screenshot helper to display step outputs clearly.
- Fully reproducible workflow for experimentation and portfolio use.

---

## Setup & Usage

1. **Clone or download this notebook** from GitHub.  
2. **Install required packages** (Colab handles most automatically):
```python
!pip install google-generativeai pillow --quiet
---
3.
import getpass
import google.generativeai as genai

genai.configure(api_key=getpass.getpass("Enter your Gemini API key: "))
___

4. Seelect a Gemini model (example using a valid multimodal model):
model = genai.GenerativeModel("gemini-2.5-flash-image")
___

5. Run the interactive prompt / image analysis cells:

- Upload an image when prompted.

- Enter your text prompt.

- Click “Analyze” to see the response.
___

Screenshot Helper
The notebook includes a helper function to display screenshots:
import os
from IPython.display import Image as ColabImage, display, Markdown

# Ensure screenshots folder exists
os.makedirs("/content/screenshots", exist_ok=True)

def show_screenshot(filename, caption=None):
    path = f"/content/screenshots/{filename}"
    if not os.path.exists(path):
        print(f"⚠️ Screenshot not found: {path}")
        return
    display(Markdown(f"### {caption or filename}"))
    display(ColabImage(path))
___

Screenshots
show_screenshot("Interactive Imagine Analysis UI.1.png", "Step 4: Interactive Image Analysis UI - Part 1")
show_screenshot("Interactive Imagine Analysis UI.2.png", "Step 4: Interactive Image Analysis UI - Part 2")
___

Notes

- Do not hardcode your API key; always use secure input methods like getpass in Colab.

- The notebook is portfolio-ready and safe to share on GitHub.

- Supports only the Gemini models that allow generateContent for multimodal inputs.
___

License

Feel free to adapt this notebook for your own experiments and learning purposes.

This covers **everything a reader needs**: overview, setup, usage, screenshots, folder structure, and safety notes.  

Do you want me to also **suggest a shorter README title** so it doesn’t conflict with your other notebook’s README?
