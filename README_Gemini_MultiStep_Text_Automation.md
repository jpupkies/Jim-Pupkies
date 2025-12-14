# Gemini Multi-step Text Automation (Quota-Safe)

## Overview

This notebook demonstrates multi-step text automation using the Google Gemini API (`google-generativeai` Python SDK).

The workflow is designed for portfolio demonstration, is fully reproducible in Google Colab, and avoids exceeding free-tier API quotas by using pre-generated example outputs instead of live API calls.

The notebook demonstrates how to:

- Securely configure and instantiate a Gemini model
- Prepare sample text data using pandas
- Perform multi-step text automation:
  - Summarization
  - Professional rewriting
  - Structured JSON extraction
- Store structured outputs in a pandas DataFrame
- Document results with screenshots

## Features

- Multi-step prompt design and structured output workflows
- Quota-safe execution for Colab free-tier users
- Clean pandas integration
- Portfolio-ready presentation with screenshots

## Notebook Steps

### Step 1 — Install & Import Libraries

Installs required libraries and imports all dependencies used throughout the notebook, including pandas, JSON handling, and display utilities.

### Step 2 — Configure Gemini API Key

The Gemini API key is configured using secure input methods.  
For quota-safe demonstration purposes, no live API calls are executed in this notebook.

Screenshot:

![Step 2 - Configure Gemini API Key](screenshots/Step 2 - Configure Gemini API Key.png)

### Step 3 — Prepare Sample Data

A small pandas DataFrame is created containing example text entries.  
Each entry represents an event or action suitable for multi-step automation.

### Step 4 — Multi-step Automation (Simulated)

The multi-step process includes:

1. Summarizing the original text
2. Rewriting the summary in a professional tone
3. Extracting structured JSON fields:
   - person
   - action
   - object
   - date/time

To avoid free-tier quota limits, pre-generated example outputs are used.

### Step 5 — Apply Automation to DataFrame

The simulated outputs are applied to the DataFrame.  
Structured JSON fields are expanded into individual columns for clear, tabular presentation.

Screenshot:

![Step 3-5 - Use Fully Simulated Outputs](screenshots/Step 3-5 - Use Fully Simulated Outputs.png)

## Usage Notes

- Supported Gemini models include `gemini-2.5-flash` and other models that support `generateContent`
- Live API calls can be enabled by upgrading the API plan or enabling billing
- API keys should never be committed to version control

## Skills Demonstrated

- Multi-step text automation and prompt chaining
- Structured JSON extraction
- pandas-based data workflows
- Quota-safe, reproducible Colab notebook design
- Portfolio-quality documentation

## Optional Extensions

- Replace simulated outputs with live API calls when quota allows
- Add batch processing for larger datasets
- Extend the JSON schema with additional fields
- Combine with summarization or classification pipelines

