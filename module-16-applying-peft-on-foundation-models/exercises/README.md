# Applying PEFT on Foundation Models - Exercises

This directory contains hands-on exercises for learning Parameter-Efficient Fine-Tuning (PEFT) techniques. The exercises focus on implementing LoRA, AdaLoRA, and QLoRA methods for efficient model adaptation.

## Exercise: Teach an LLM to Spell with SFT

### Overview
In this exercise, you will fine-tune a small language model to perform spelling correction using Supervised Fine-Tuning (SFT) with PEFT techniques. You'll implement LoRA adapters, train the model on spelling data, and evaluate its performance on spelling correction tasks.

## Folder Structure

```
exercises
    |_ starter
    |   |_ teach-an-llm-to-spell-with-sft-starter.ipynb
    |   |_ README.md
    |_ solution
    |   |_ teach-an-llm-to-spell-with-sft-solution.ipynb
    |   |_ demo.ipynb
    |   |_ data/
    |   |   |_ spelling_adapter/
    |   |   |_ SmolLM2-135M-Instruct-SFT/
    |   |_ README.md
    |_ README.md
```

### Exercise Structure
- **Starter Materials** (`starter/`): Contains PEFT implementation starter code and training datasets
- **Solution Materials** (`solution/`): Complete fine-tuning pipeline with LoRA adapters and evaluation metrics