# Fine-Tuning Large Language Models for Swiss German Song Generation

This repository contains the code and training pipeline for a research project focused on fine-tuning a pre-trained LLM (Recurrent Neural Network with GRUs) to generate lyrics in the **Bernese dialect of Swiss German**.

The goal of this project was to explore whether large language models can generate culturally meaningful and coherent text in underrepresented dialects, using Swiss German song lyrics as a case study.

## Project Context

This work was conducted as part of a **Master's research project** at the Lucerne University of Applied Sciences and Arts (HSLU) and the Fernfachhochschule Schweiz (FFHS) in 2024.

> 📄 Full paper (PDF): _Available upon request_

## Overview

- **Language Focus:** Bernese dialect of Swiss German  
- **Model Architecture:** Recurrent Neural Network (RNN) with GRU cells  
- **Frameworks:** TensorFlow · Keras · Python 3  
- **Tasks Covered:**  
  - Custom dataset curation  
  - Preprocessing (tokenization, standardization)  
  - Model fine-tuning  
  - Output generation  
  - Evaluation based on perplexity and human review

## Key Findings

- Successful adaptation of a GRU-based model to a low-resource dialect  
- Generated lyrics were partially coherent and stylistically aligned with dialect norms  
- Challenges included data scarcity and dialect-specific token variability  
- The project demonstrates potential for LLM-based text generation in underrepresented linguistic contexts

## Repository Structure

```
├── data/
│   ├── raw_lyrics.txt
│   └── cleaned_lyrics.csv
├── notebooks/
│   ├── 01_preprocessing.ipynb
│   └── 02_training_and_generation.ipynb
├── models/
│   └── bernese_lyrics_model.h5
├── README.md
└── requirements.txt
```

## Getting Started

### Requirements
```bash
pip install -r requirements.txt
```

### Run Training
```bash
python train_model.py
```

### Generate Lyrics
```bash
python generate_text.py --seed "Ich bi dr"
```

## 📄 License

This project is for academic and educational purposes only.  
Please contact [sreterannamaria1@gmail.com](mailto:sreterannamaria1@gmail.com) for further inquiries.
