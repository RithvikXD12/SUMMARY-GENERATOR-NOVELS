## Summary Generator for Novels

## Overview
This project implements a novel summary generator using advanced natural language processing (NLP) techniques. The model takes a novel's text and generates a concise summary tailored to the given genre. 
The implementation leverages state-of-the-art pre-trained models (T5 or BART) fine-tuned on a custom dataset for enhanced summarization performance. The system is evaluated using several metrics, ensuring 
the quality and relevance of the generated summaries.

## Features
**Summarization Engine:**
- A fine-tuned model capable of generating concise, genre-specific summaries of novels.
- Optimized preprocessing and tokenization for handling large text inputs.

**Evaluation Metrics:**
- ROUGE (Recall-Oriented Understudy for Gisting Evaluation):
    - Measures the overlap between generated and reference summaries.
    - Provides recall, precision, and F1-score for the evaluation.
- BLEU (Bilingual Evaluation Understudy):
    - Measures the similarity of the generated summary to the reference summary.
- Subjective Analysis:
    - Includes human evaluation for qualitative assessment of summary relevance and readability

## Requirements
**To run the project, ensure the following dependencies are installed:**

 - Python 3.x
 - Hugging Face Transformers: For the T5/BART pre-trained models.
 - PyTorch: Backend framework for deep learning.
 - NumPy: For numerical computations.
 - Pandas: For dataset manipulation.
 - datasets: For processing datasets.
- Matplotlib: For visualizing results.
 - sklearn.metrics: For evaluation metrics like ROUGE and BLEU.
 - Google Colab: Recommended for training and fine-tuning the model.
 - faiss-cpu: (Optional) For fast similarity searches.

## Model Features
- Input: Novel text and its genre.
- Output: Concise, high-quality summary of the novel.
- Pre-trained Model: Supports both T5 and BART models.
- Fine-Tuning: The pre-trained model is fine-tuned using a custom dataset of novel texts and summaries.

## Evaluation Metrics
- **ROUGE:**
    - Measures the overlap between the generated summary and the reference summary.
    - Metrics: ROUGE-1, ROUGE-2, and ROUGE-L.

- **BLEU:**
    - Measures the similarity of the generated summary to the reference summary using n-grams.

## Usage
- **Data Preparation:**
    - Preprocess the dataset to tokenize and truncate novel texts and their corresponding summaries.

- **Model Training:**
    - Fine-tune the T5 or BART model on the preprocessed dataset.

- **Evaluation:**
    - Evaluate the model's performance using the defined metrics.

- **Generate Summaries:**
    - Use the fine-tuned model to generate summaries for novel texts.

## Future Enhancements
   - Integrate the model into a Library Management System for automatic summary generation.
   - Explore zero-shot learning to summarize novels in unseen genres.
   - Deploy the model as a web application for public use.




