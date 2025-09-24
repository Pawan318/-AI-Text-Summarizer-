# -AI-Text-Summarizer-
AI-powered Text Summarizer built with Hugging Face Transformers. Uses the BART pre-trained model to generate concise and readable summaries from long text. Implemented in Python for fast and easy summarization.

# Features

Uses BART pre-trained model for abstractive text summarization.

Converts long articles into short, meaningful summaries.

Helps make content more readable and saves time.

Easy to use via a Colab notebook or Python script.

# Tech Stack

Python

Hugging Face Transformers

PyTorch

# How It Works

Load the pre-trained BART model using Hugging Face pipeline.

Pass your long text as input.

Get a concise summary as output.

# BART-Based AI Text Summarizer

A simple AI-powered **Text Summarizer** that uses the **BART pre-trained model** from Hugging Face Transformers to generate concise summaries of news articles or long text.

## Business Objective
Text summarization helps convert long articles into short, readable summaries while keeping the main meaning intact. This project is useful for:
- Reading news articles faster
- Summarizing meeting notes or reports
- Generating concise documentation
- Educational content simplification

## Dataset (Optional)
If using a dataset for training:
- 40,000 news articles with professional summaries
- CSV format with:
  - `Article Titles`
  - `Summaries`
  - `Article Content`
  - `Publication Dates`
  - `URLs` to original articles

## Aim
Use **BART (Bidirectional and Auto-Regressive Transformer)** model to perform **abstractive summarization** on long text input.

## Tech Stack
- **Programming Language:** Python  
- **Libraries:** transformers, torch, pandas (optional)  
- **Environment:** Google Colab (GPU-enabled)

## How It Works
1. Load the **BART pre-trained summarization model** using Hugging Face pipeline.  
2. Input a long text or news article.  
3. Generate a short, human-readable summary.  

## Usage (Colab / Python)

# ``python
from transformers import pipeline

# Load summarization pipeline
summarizer = pipeline("summarization", model="facebook/bart-large-cnn")

# Example text
text = "Your long text or news article here."

# Generate summary
summary = summarizer(text, max_length=80, min_length=30, do_sample=False)
print(summary[0]['summary_text'])

<img width="739" height="172" alt="image" src="https://github.com/user-attachments/assets/5e1a81eb-47d0-4c8c-80cb-c31cc49ff78d" />


# Installation

1.Clone the repository:

git clone <repository_url>
cd AI-Text-Summarizer

2.Install dependencies:
pip install -r requirements.txt

# Contact

For questions or suggestions:

Name: Pawan Prajapati
GitHub: <Pawan318>
Email: <pawanprajapati7068@gmail.com>
