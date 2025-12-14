**Gemini Structured JSON Extraction**

**Overview**

This notebook demonstrates structured information extraction from free-text data using the Google Gemini API (google-generativeai Python SDK). The workflow is designed to be portfolio-ready, reproducible, and fully compatible with Colab.

The notebook shows how to:

- Securely configure the Gemini API key.

- Prepare a sample dataset in a pandas DataFrame.

- Extract structured JSON fields from text using prompt design.

- Integrate JSON results into pandas for clean, tabular output.

- Visualize outputs and include screenshots for documentation.
___

**Features**

- **Structured JSON output** for deterministic parsing.

- **Pandas integration** for clean data handling.

- **Error handling** to manage unexpected model responses.

- **Portfolio-friendly:** fully working in Colab without unsupported features.
___

**Notebook Steps**

**Step 1 — Install & Import Libraries**

- Installs google-generativeai and pandas.

- Imports all necessary modules.

**Step 2 — Configure Gemini API Key**

- Securely enter your API key using getpass or Colab secrets.

- Instantiate a supported Gemini model (gemini-2.5-flash).

**Step 3 — Prepare Sample Data**

- Create a pandas DataFrame containing sample text.

- Example texts include sentences describing actions, dates, and entities.

**Screenshot: Step 3**
<br>
<img width="1776" height="362" alt="Step 3 - Prepare Sample Data" src="https://github.com/user-attachments/assets/85f3a929-2d8d-4516-9fa7-ee5ed44d47ef" />


**Step 4 — Define JSON Extraction Function**

- Define a Python function that prompts Gemini to extract structured fields:

- person

- action

- object

- date/time

- Includes JSON parsing with error handling.

**Step 5 — Apply Extraction to DataFrame**

- Apply the extraction function to each row in the DataFrame.

- Expand the JSON fields into separate columns for clean tabular output.

**Screenshot: Step 5**
<br>
<img width="1775" height="282" alt="Step 5 - Apply Extraction to DataFrame" src="https://github.com/user-attachments/assets/cd2bf146-51a4-41c0-b8a7-a53456a42e55" />
___

**Usage Notes**

- **Supported Models:** Use one of the models from genai.list_models() with generateContent. Recommended: "gemini-2.5-flash" or "gemini-flash-latest".

- **Security:** Never commit your real API key. Use Colab secrets or getpass for secure input.

- **Scalability:** This workflow can be extended to larger datasets, file-based inputs, or multi-step pipelines.
___

**Skills Demonstrated**

- Gemini API integration in Python.

- Structured prompt design for JSON extraction.

- Pandas workflows for storing and visualizing structured data.

- Portfolio-ready Colab notebook design, including screenshots.
___

**Optional Extensions**

- Batch multiple rows to reduce API calls.

- Add logging or retry logic for API errors.

- Extend JSON schema for additional entities, actions, or relations.

- Combine with summarization or classification pipelines for multi-step automation.
___
