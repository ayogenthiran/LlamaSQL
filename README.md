# LlamaSQL: Fine-Tuning Llama-2 for Expert SQL Query Generation

LlamaSQL is a fine-tuned version of Llama-2 optimized for SQL query generation and understanding. Using the ChrisHayduk Llama-2-SQL-Dataset and NousResearch/Llama-2-7b-hf, this project enhances Llama's ability to process, generate, and optimize SQL queries effectively.

## Project Overview

Large Language Models (LLMs) like Llama-2 have shown exceptional capabilities in natural language processing. This project fine-tunes Llama-2 specifically for SQL tasks, enabling it to:

* Generate SQL queries from natural language prompts
* Optimize and correct SQL queries
* Explain SQL queries in human-readable format

## Technologies Used

* **Model:** NousResearch/Llama-2-7b-hf
* **Dataset:** ChrisHayduk/Llama-2-SQL-Dataset
* **Framework:** Hugging Face transformers, peft, bitsandbytes
* **Fine-Tuning Approach:** LoRA (Low-Rank Adaptation) & Full Fine-Tuning
* **Evaluation Metrics:** BLEU Score (Measures SQL query similarity to ground truth)

## Fine-Tuning Process

### 1. Data Preparation

The dataset from ChrisHayduk/Llama-2-SQL-Dataset is preprocessed and tokenized.

### 2. Training Setup

LoRA is applied to efficiently fine-tune the NousResearch/Llama-2-7b-hf model.

### 3. Fine-Tuning

Model trained on T4 GPU from colab using bitsandbytes for memory efficiency.

### 4. Evaluation & Testing

Evaluated using SQL execution correctness.

---

**Note:** This project is designed to run in a Google Colab environment with T4 GPU support. Make sure you have sufficient computational resources before training.