# Article-Summarizer
This project is a Python tool that summarizes lengthy articles using advanced Natural Language Processing (NLP) models — specifically Facebook’s BART model from the Hugging Face Transformers library. It’s designed to generate clear, concise summaries from long documents.
⚙️ Requirements:

Python 3.6+
Libraries:
transformers
torch
Installation:
pip install transformers torch
🔍 How It Works:

Uses a pre-trained summarization pipeline from Hugging Face.
If the input article is longer than 1024 tokens (model’s limit), it splits the text into chunks.
Each chunk is summarized individually, and all summaries are combined into the final output.
▶️ Usage:

Run the script.
Paste your article when prompted.
View the summary output in the terminal.
🧠 Core Python Code:

Defines a function summarize_article(article_text, max_length, min_length) to handle the summarization.
Automatically detects long input and applies chunking logic.
Uses facebook/bart-large-cnn as the summarization model.
Includes a simple __main__ block for terminal interaction.
