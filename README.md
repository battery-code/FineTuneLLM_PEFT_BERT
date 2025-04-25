# Sentiment Analysis with PEFT: Adapters, LoRA, QLoRA

## Overview

This project fine-tunes a pre-trained foundation model for a specific NLP task: sentiment analysis. The goal is educational — to explore different Parameter-Efficient Fine-Tuning (PEFT) techniques and compare their performance in accuracy, efficiency, and resource usage.

## Task

- Objective: Fine-tune a foundation model to classify sentiment in movie reviews.

- Dataset: A stratified subsample (5,000 train / 5,000 test) from stanfordnlp/imdb.

## Foundation Model

- Model: bert-base-uncased (~110M parameters)

- Encoder-only architecture (ideal for classification tasks).

- Fits well within compute constraints of the Udacity Tesla T4 GPU environment.

- Pre-trained on a large corpus of English and used as a frozen base for PEFT.

## Motivation
Fine-tuning large language models (LLMs) from scratch is resource-intensive. PEFT techniques allow us to fine-tune only small, task-specific components while keeping most of the LLM frozen. This dramatically reduces memory and compute requirements without significant performance loss.
