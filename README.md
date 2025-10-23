# Fine-Tuning a Large Language Model (LLM) for Domain-Specific Medical Question Answering

## Overview
This project fine-tunes GPT-2 Medium using PEFT (LoRA + QLoRA) to improve performance on a specialized medical question-answering dataset. The goal is to demonstrate parameter-efficient fine-tuning for domain adaptation.

## Steps to Reproduce
1. Open `llm_finetune_kishore_final_explained.ipynb` in Google Colab.
2. Enable GPU (Tesla T4).
3. Run all cells sequentially.
4. Model artifacts and results will be saved in `./medical-qa-model/`.

## Requirements
Install dependencies using:
```bash
pip install -r requirements.txt
```

## Dataset
- Source: `medalpaca/medical_meadow_medical_flashcards` from Hugging Face
- Format: Instruction-based Q&A for medical reasoning

## Evaluation Metrics
- ROUGE-1, ROUGE-2, ROUGE-L
- ~40% improvement over baseline GPT-2

## Disclaimer
Outputs are for **educational use only** and not for real medical advice.
