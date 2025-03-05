# cnn-dailymail-rag

## Project Overview
This project is about building a RAG (Retrieval-Augmented Generation) pipeline using the CNN/DailyMail dataset. The idea is to create a system that can search for relevant news articles and then generate summaries or answers from those articles.

RAG is cool because it combines retrieval (finding the right documents) and generation (writing a good response). This method works really well for things like question answering, summarization, or any task where we need to use information from a lot of documents.

## Dataset
**Name:** CNN/DailyMail  
**Source:** Hugging Face Dataset Hub  
**Description:** This dataset contains news articles from CNN and Daily Mail, along with corresponding summaries.

## Tech Stack

| Tool            | Purpose                          |
|------------------|----------------------------------|
| Python          | Main programming language        |
| Hugging Face Datasets | Load dataset           |
| FAISS           | For document retrieval           |
| Transformers    | For generation (language model)  |
| Google Colab    | Execution environment            |
| GitHub          | Version control & project sharing|


## cnn_dailymail_rag/
├── data/              # Folder for raw & processed data (local if needed)
│   ├── raw/            # Original dataset files
│   ├── processed/      # Preprocessed (cleaned, tokenized, etc.)
│
├── notebooks/          # Optional (if we split work into multiple notebooks)
│   ├── 1-data_exploration.ipynb
│   ├── 2-data_preprocessing.ipynb
│   ├── 3-rag_pipeline.ipynb
│
├── src/                 # Scripts (if you want to split some code later)
│   ├── data_loading.py
│   ├── preprocessing.py
│   ├── retrieval.py
│   ├── generation.py
│
├── README.md            # This file
├── requirements.txt     # Libraries needed (if someone wants to run locally)
├── .gitignore           # To avoid pushing unnecessary files

## workflow steps

Data Exploration: Understanding the dataset — articles, summaries, lengths.
Preprocessing: Cleaning text, tokenization, vectorization for retrieval.
Retrieval: Using FAISS (or similar) to search for relevant articles.
Generation: Using a language model (like distilbart or flan-t5) to generate summaries or answers.
Evaluation: Checking how well the system works (optional).

