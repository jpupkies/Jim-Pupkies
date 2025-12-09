Gemini Batch Prompt Runner – Portfolio Project

This project demonstrates a repeatable AI batch-processing workflow using multiple LLMs (Google Gemini, GPT-4, and Claude).
Prompts are loaded from a CSV file, processed in bulk, and results are saved to a timestamped CSV for analysis.
It is designed as a portfolio-ready project showcasing Python scripting, API integration, and workflow automation.
___

Features

- Load prompts from a CSV file (easy to edit or expand)

- Send prompts in bulk to one or more AI models (Gemini, GPT-4, Claude)

- Capture responses along with elapsed time

- Save results to timestamped CSV files

- Optional screenshot support for execution verification (especially in Colab)

- Fully hosted and runnable in Google Colab—no local setup required
____

Project Structure
AI_Portfolio/
├── gemini_batch_prompt_runner.ipynb  # Main Colab notebook
├── prompts.csv                        # Input prompts (editable)
├── output_YYYYMMDD_HHMMSS.csv         # Saved model responses (timestamped)
└── screenshots/                       # Proof-of-execution images
___

How It Works

1. Load prompts from prompts.csv.

2. Run multi-model batch function (run_batch_prompts) to send each prompt to selected models.

3. Capture responses along with timestamp and elapsed time.

4. Save output to a timestamped CSV (output_YYYYMMDD_HHMMSS.csv).

5. Optional screenshots provide visual confirmation of workflow execution in Colab.
___

Getting Started

1. Clone or download the repository.

2. Open gemini_batch_prompt_runner.ipynb in Google Colab.

3. Run Section 1 – Setup & API Key and securely enter your Gemini API key.

4. Edit or upload prompts.csv with the prompts you want to test.

5. Run Section 2 – Batch Workflow Function to define the multi-model batch functions.

6. Run Section 3 – Execute Batch Process to generate responses and save them to CSV.

7. Review results in the latest output_*.csv file. Screenshots can be used to confirm workflow execution.
___

Sections Overview
Section 1 – Setup & API Initialization

- Securely input your Gemini API key at runtime

- Import required libraries

- Initialize the Gemini client

- List available models

Section 2 – Multi-Model Batch Functions

- get_model_response(prompt, model_name, ...): Sends a single prompt to the selected model (Gemini, GPT-4, or Claude) and returns response text, model, and elapsed time

- run_batch_prompts(input_csv, output_dir, models, delay, openai_api_key): Processes prompts from CSV across multiple models, saves responses with timestamps and elapsed time, supports configurable delay

Section 3 – Run Batch Process & Save Outputs

- Executes the batch function using your prompts

- Captures responses from all selected models

- Saves output to a timestamped CSV file

- Preview results in the notebook

Section 4 – Workflow Diagram

- Visualizes the end-to-end process: CSV input → batch function → API calls → CSV output
___

Skills Demonstrated

- Python scripting and automation

- Working with CSV files for batch processing

- Multi-LLM integration (Gemini, GPT-4, Claude)

- Error handling and logging

- Timing and response tracking

- Workflow visualization with Graphviz

- GitHub project structure and reproducibility

Next Steps

- Deploy a user-friendly batch UI

- Implement prompt versioning for reproducibility

- Expand support for additional AI models

- Add automated testing for batch workflow
____

Screnshots/Evidence of Execution
Figure 1, Section 1 - Setup
<img width="322" height="707" alt="Section 1 1" src="https://github.com/user-attachments/assets/845e8d33-c517-4fce-8e63-e8e35210e1bf" />
Figure 2, Section 1 - Gemini Helper Function
<img width="621" height="143" alt="Section1 2" src="https://github.com/user-attachments/assets/5fe6c11f-c82e-47bf-8ecc-4cd52d26cace" />

Figure 1, Section 2 - Get Model Responses
<img width="321" height="650" alt="Section2 1" src="https://github.com/user-attachments/assets/bf89370f-0486-4e77-a1d0-40b3a93b2204" />

Figure 2, Section 2 - List Available Gemini Models
<img width="147" height="352" alt="Section2 2" src="https://github.com/user-attachments/assets/080dd257-94e8-48c9-9194-64083d5250a3" />

Figure 3, Section 2 - Sample Prompts
<img width="166" height="155" alt="Section2 3" src="https://github.com/user-attachments/assets/a3c862a4-b170-4ed7-b16a-c2a7fe7b9723" />

Figure 4, Section 2 - Display First 10 Responses
<img width="397" height="234" alt="Section2 4" src="https://github.com/user-attachments/assets/a314f9d5-0b74-4621-ba49-a7920716ea99" />

Figure 5, Section 2 - More Demonstration
<img width="169" height="141" alt="Section2 5" src="https://github.com/user-attachments/assets/7553223b-f6d7-4cf6-9207-9e47c0b6daa7" />

Figure 6, Section 2
<img width="298" height="68" alt="Section2 6" src="https://github.com/user-attachments/assets/4a7defed-bb7f-4a0b-ac7d-08c1ae42e837" />

Figure 1, Section 3 - Run Batch Processing Step 1
<img width="824" height="701" alt="Section3 1" src="https://github.com/user-attachments/assets/554920a7-0bb1-47bf-b8d7-01a91f4fd9bd" />

Figure 2, Section 3 - Step 2
<img width="830" height="628" alt="Section3 2" src="https://github.com/user-attachments/assets/b0220632-fdb2-43e1-a7a0-a33bf012c771" />

Figure 2, Section 3 - Example
<img width="824" height="653" alt="Section3 3" src="https://github.com/user-attachments/assets/7214462c-78d8-421f-be79-b0847110723d" />

Figure 1, Section 4 - Workflow Diagram
<img width="567" height="740" alt="Section4 1" src="https://github.com/user-attachments/assets/db621b25-82a2-4180-985e-71b59bf41bc6" />
