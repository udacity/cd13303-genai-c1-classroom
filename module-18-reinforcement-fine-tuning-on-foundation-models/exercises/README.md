# Reinforcement Fine-Tuning on Foundation Models - Exercises

This directory contains hands-on exercises for learning advanced fine-tuning techniques using reinforcement learning. The exercises focus on implementing GRPO and RLHF for language model alignment.

## Exercise: Teach an LLM to Spell with GRPO

### Overview
In this exercise, you will implement Group Relative Policy Optimization to fine-tune a language model for spelling correction. You'll build a reward model based on spelling accuracy, implement the GRPO algorithm, and train the model to improve its spelling correction capabilities through reinforcement learning.

## Folder Structure

```
exercises
    |_ starter
    |   |_ teach-an-llm-to-spell-with-grpo-starter.ipynb
    |   |_ README.md
    |_ solution
    |   |_ teach-an-llm-to-spell-with-grpo-solution.ipynb
    |   |_ demo.ipynb
    |   |_ data/
    |   |   |_ counting-grpo/
    |   |   |_ spelling-grpo/
    |   |_ README.md
    |_ README.md
```

### Exercise Structure
- **Starter Materials** (`starter/`): Contains GRPO implementation starter code and reward model framework
- **Solution Materials** (`solution/`): Complete reinforcement fine-tuning pipeline with GRPO and evaluation metrics