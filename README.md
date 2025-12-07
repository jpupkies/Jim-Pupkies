Automated Prompt Testing with Gemini API

This project allows users to automatically test a list of prompts using the Google Gemini API and generate results into a CSV file. It is designed as a starter tool for exploring AI responses and building a personal AI portfolio.
___________________________________________________________________________________________________________________________________________

Features

• Load prompts from a CSV file (easily editable)

• Send prompts in bulk to Gemini

• Save all responses into an output.csv

• Optional screenshot support for confirming execution in Colab

• Fully hosted + runnable in Google Colab (no local setup needed)
___________________________________________________________________________________________________________________________________________

1. Open the notebook
Launch Automated_Prompt_Testing.ipynb in Google Colab.

2. Set up your environment
Colab will automatically install required packages. You only need to enter your Gemini API key when prompted.

3. Prepare prompts
Edit prompts.csv to include the text prompts you want to test.

4. Run the batch process
Execute the notebook cells in order. Responses will be saved to output.csv and screenshots can be optionally generated for verification.

5. Review results
Check output.csv for all generated responses. Use screenshots to confirm workflow execution if needed.
___________________________________________________________________________________________________________________________________________

AI_Portfolio/
├── Automated_Prompt_Testing.ipynb   # Main Colab notebook

├── prompts.csv                      # Input prompts (editable)

├── output.csv                       # Saved model responses

└── screenshots/                     # Proof-of-execution images
___________________________________________________________________________________________________________________________________________

How to Run

1. Clone or download this repository
2. Open the notebook in Google Colab
3. Run the Setup cell and enter your Gemini API key when prompted
4. Upload or edit the prompts.csv file
5. Continue running all remaining cells to generate output.csv
6. Review the results and included screenshots of successful execution
___________________________________________________________________________________________________________________________________________

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
___________________________________________________________________________________________________________________________________________

**Step 1 – Prepare Prompts:** Creating and previewing the `prompts.csv` file.

<img width="633" height="780" alt="Step1_PromptCSV_Example" src="https://github.com/user-attachments/assets/d800e1f9-e6c4-4cd0-bc6b-971a87bae367" />

<img width="339" height="408" alt="Step1_PromptCSV_Example" src="https://github.com/user-attachments/assets/1bf2d6d2-00b4-4472-bd17-1d4feb21dba9" />
___________________________________________________________________________________________________________________________________________

**Step 2 – Define Batch Workflow Function:** This screenshot shows the batch function that reads prompts from the CSV, sends them to Gemini, and saves the responses.

<img width="418" height="690" alt="Step2_PromptCSV_Example" src="https://github.com/user-attachments/assets/707d3486-6487-4286-952b-aa87e3e1cd0f" />

<img width="321" height="651" alt="Step2_PromptCSV_Example" src="https://github.com/user-attachments/assets/ff14bae6-93d7-4a2f-982c-afea94134341" />

<img width="1830" height="474" alt="Step2_PromptCSV_Example" src="https://github.com/user-attachments/assets/d9bc6e7e-c025-4631-9c88-7b60a474b342" />

<img width="254" height="530" alt="Step2_PromptCSV_Example" src="https://github.com/user-attachments/assets/97b7110e-55bd-4a87-9c6d-f3d95321524a" />

<img width="370" height="706" alt="Step2_PromptCSV_Example" src="https://github.com/user-attachments/assets/dc30b656-cb4e-48a8-8eb7-2aa81889bb83" />
___________________________________________________________________________________________________________________________________________

**Step 3 – Run Batch Process:** This screenshot shows executing the batch function, sending prompts to Gemini, and previewing the timestamped output CSV.

<img width="324" height="523" alt="Step3_PromptCSV_Example" src="https://github.com/user-attachments/assets/0ca6ef0b-0a0c-4e27-961d-0bef91df5610" />

<img width="817" height="587" alt="Step3_PromptCSV_Example" src="https://github.com/user-attachments/assets/00a80d1c-e790-44c7-bfa4-d9e1c700c500" />
___________________________________________________________________________________________________________________________________________

**Step 4 – Workflow Diagram:** This diagram shows the end-to-end flow of the batch prompt runner: loading prompts from CSV, sending them to Gemini via the batch function, collecting responses, and saving them to output.csv.

<img width="567" height="740" alt="Step4_PromptCSV_Example" src="https://github.com/user-attachments/assets/d6402582-d16d-484c-a539-ef6008074aac" />
