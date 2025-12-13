# Auto Summary Pipeline

## Overview
This notebook demonstrates an automated text summarization pipeline using Google Gemini / Generative AI.  
It allows you to feed a text file (`input.txt`) and automatically generate concise summaries with a single call to the Gemini model. The pipeline is designed to be reproducible, portfolio-ready, and secure with private API key handling.

---

## Features
- Safely input your Gemini API key without exposing it in the notebook.
- Load text from a `.txt` file.
- Automatically summarize large text content with Gemini.
- Helper functions for displaying outputs and screenshots.
- Fully reproducible workflow for showcasing in a portfolio.

---

## File Structure

/content/
├── screenshots/
│ ├── Step 2 - Configure API & Load Text File.png
│ └── Step 5 - Run the Auto-Summary Pipeline.png
├── input.txt
├── Auto_Summary_Pipeline.ipynb
└── README_Auto_Summary_Pipeline.md


---

## Setup Instructions

1. **Clone or download the repository** containing this notebook.  
2. **Upload `input.txt`** to the same folder as the notebook if not already present.  
3. **Ensure the `screenshots` folder** contains the corresponding images for visual reference.  

---

## Running the Notebook

1. **Configure Gemini API Key**

   Use the secure prompt in the notebook to enter your API key:
   ```python
   import getpass
   import google.generativeai as genai

   genai.configure(api_key=getpass.getpass("Enter your Gemini API key: "))

2. Load the text file

Ensure input.txt exists in the notebook folder. The helper function will read its content:
from pathlib import Path

def load_text_file(filename="input.txt"):
    if not Path(filename).exists():
        raise FileNotFoundError(f"{filename} not found!")
    return Path(filename).read_text(encoding="utf-8")

3. Run Auto-Summary

The notebook contains a ready-to-run pipeline that generates a summary from the loaded text.

Screenshots

Step 2 - Configure API & Load Text File
<br>
<img width="1779" height="734" alt="Step 2 - Configure API   Load Text File" src="https://github.com/user-attachments/assets/e009c411-c9cb-4db1-898f-fd86c9d6714e" />
<br>
Step 5 - Run the Auto-Summary Pipeline
<br>
<img width="1780" height="770" alt="Step 5 - Run the Auto-Summary Pipeline" src="https://github.com/user-attachments/assets/bf00a1c8-3d7a-4c94-accb-22d4a4557fb1" />
<br>

Notes

- Ensure your Gemini API key is kept private. Do not commit it to GitHub.

- The notebook is designed for Google Colab but can be adapted for local Python environments.

- input.txt can contain any text content you want to summarize; the model automatically handles large text inputs.
___

Next Steps

- Extend the pipeline to process multiple text files at once.

- Integrate with Google Drive to automatically fetch documents.

- Experiment with different Gemini models to compare summary quality.
___

License

This notebook and associated files are provided for personal and educational use. Do not share API keys publicly.
