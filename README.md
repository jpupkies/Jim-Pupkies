Automated Prompt Testing with Gemini API

This project allows users to automatically test a list of prompts using the Google Gemini API and generate results into a CSV file. It is designed as a starter tool for exploring AI responses and building a personal AI portfolio.
______________________________________________________________________________________________________________________________

Features

• Load prompts from a CSV file (easily editable)

• Send prompts in bulk to Gemini

• Save all responses into an output.csv

• Optional screenshot support for confirming execution in Colab

• Fully hosted + runnable in Google Colab (no local setup needed)
______________________________________________________________________________________________________________________________

AI_Portfolio/
├── Automated_Prompt_Testing.ipynb   # Main Colab notebook
├── prompts.csv                      # Input prompts (editable)
├── output.csv                       # Saved model responses
└── screenshots/                     # Proof-of-execution images
______________________________________________________________________________________________________________________________

How to Run

1. Clone or download this repository
2. Open the notebook in Google Colab
3. Run the Setup cell and enter your Gemini API key when prompted
4. Upload or edit the prompts.csv file
5. Continue running all remaining cells to generate output.csv
6. Review the results and included screenshots of successful execution
______________________________________________________________________________________________________________________________

### Workflow / Architecture Diagram

This diagram shows the end-to-end flow of the batch prompt runner:

1. Load prompts from `prompts.csv`
2. Send prompts to Gemini via the batch function
3. Collect responses
4. Save responses to `output.csv`

![Workflow Diagram](screenshots/Section4.1.png)
____________________________________________________________________________________________________________________________

### Skills Demonstrated & Next Steps

**Skills Demonstrated:**
- Python scripting for automation
- Working with CSV files for batch processing
- Generative AI integration (Google Gemini API)
- Error handling and response validation
- Visualization of workflows and pipelines
- Version control readiness for GitHub

**Next Steps:**
- Deploy a user-friendly batch UI
- Implement prompt versioning for better reproducibility
- Expand support to additional AI models
- Add automated testing for batch processing
____________________________________________________________________________________________________________________________

