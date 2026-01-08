# Abstract-Summarizer
Abstract Summarizer is a GenAI-powered web app that extracts abstracts from research papers and generates concise, human-readable summaries using a BART model. It supports PDF/TXT/CSV files, analyzes AI-style content patterns, visualizes scores, and allows multi-file upload with ZIP download support.
Abstract Summarizer using GenAI
An interactive Gradio-based web application that automatically extracts, summarizes, and analyzes abstracts from research papers (PDF, TXT, or CSV) using Generative AI (BART model).

This app is ideal for researchers, students, and academic professionals who want to quickly understand key insights from multiple papers.

#Features
Automatic Abstract Extraction: Detects and retrieves abstract sections from uploaded research papers.

Smart Summarization: Generates concise, human-like summaries using the Facebook BART model.

AI-style Content Scoring: Evaluates original and summarized texts for AI-generated writing patterns.

Visualization: Displays a bar chart comparing AI-content scores before and after summarization.

Batch Processing: Upload and process multiple files at once, then download all results as a ZIP file.

Login System: Includes a simple authentication interface.

User-friendly UI: Built using Gradio Tabs and Blocks layout.

Tech Stack
Component	Technology Used
Frontend UI	Gradio
PDF Parsing	PyMuPDF (fitz)
Summarization	Hugging Face Transformers - BART Model
Visualization	Matplotlib
Zip/IO Handling	OS, Zipfile
Language	Python 3.8+
📦 Installation
1. Clone the Repository
bash
git clone https://github.com/yourusername/abstract-summarizer-genai.git
cd abstract-summarizer-genai
2. Install Dependencies
bash
pip install -q PyMuPDF gradio transformers matplotlib
Optional: Use a virtual environment to keep packages isolated

bash
python -m venv venv
source venv/bin/activate  # for Linux/Mac
venv\Scripts\activate     # for Windows
⚙️ Usage
1. Run the App
bash
python app.py
2. Access in Browser
Once launched, Gradio will display:

text
Running on local URL: http://127.0.0.1:7860
Open that link to use the web interface.

How It Works
Login: Enter your credentials


Upload Files: PDF, TXT, or CSV files containing academic papers.

Summarize: Click the “🧠 Summarize” button.

View Results:

Extracted abstract

Summarized text

AI-content style comparison chart

Download: Get all your processed summaries as a ZIP file.

Example Output
Input: Research paper PDF
Output Includes:

Extracted abstract

Summarized abstract (7–8 sentences)

Content scorer visualization (via Matplotlib)

Downloadable .zip of summaries
