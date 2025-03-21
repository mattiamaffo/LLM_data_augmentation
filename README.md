# NLP Homework 2 - FEVER Dataset Fine-Tuning and Augmentation

This project is part of a homework assignment for a Natural Language Processing course. The objective is to fine-tune a pre-trained language model on the FEVER dataset and enhance its performance using various data augmentation techniques.

## Model & Dataset

- **Model**: `distilbert-base-uncased` from HuggingFace Transformers
- **Dataset**: Subset of [FEVER](https://fever.ai/) loaded via `datasets` library

## Data Augmentation Techniques

Five augmentation strategies were developed to improve model robustness:

1. **Hypernym/Hyponym Replacement** – Replace nouns with semantically similar alternatives.
2. **Agent/Patient Swapping** – Swap subject/object roles based on semantic role labeling.
3. **Antonym Replacement** – Use antonyms for adjectives/adverbs to change sentence meaning.
4. **Paraphrasing** – Generate paraphrases using Pegasus.
5. **Proper Noun Replacement** – Swap named entities with similar alternatives (e.g., cities, people).

## 📝 Notes

The project emphasizes generating coherent and semantically valid augmented data. While improvements were modest, the pipeline is adaptable and could benefit from stronger models or additional tuning.
