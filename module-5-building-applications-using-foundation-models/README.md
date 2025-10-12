# Building Applications Using Foundation Models

This module focuses on turning general-purpose foundation models into targeted applications. You will practice framing product requirements, assembling lightweight datasets, and orchestrating prompting strategies that let an LLM deliver reliable, auditable results.

## Learning Outcomes
- Translate product requirements into an end-to-end foundation model workflow
- Source and structure lightweight datasets to validate LLM-driven features
- Design prompts that balance instruction, context, and output formatting for downstream automation
- Evaluate model responses, capture iteration history, and decide when to add more guidance or tooling

## Exercise Overview
- **LLM Spam Classifier Lab** (`exercises/`): Build a spam detector by prompting a foundation model to label short-form messages, measure baseline accuracy, and iterate with few-shot examples. Starter and solution notebooks illustrate both the hands-on workflow and a reference implementation.

## Directory Map
- `exercises/INTRODUCTION.md` – learner-facing overview that sets the scenario and success criteria
- `exercises/INSTRUCTIONS.md` – numbered checklist covering data prep, prompting, evaluation, and iteration
- `exercises/starter/` – classroom-ready notebook and assets for students to complete the lab
- `exercises/solution/` – facilitator notebook plus scaffolding for demonstrations and support material

## Getting Started
1. Read the introduction and instructions in `exercises/` to understand the storyline and deliverables.
2. Open `exercises/starter/module-5-building-applications-using-foundation-models-starter.ipynb` in Jupyter Lab or your preferred notebook environment.
3. Ensure you have access to an LLM endpoint (web UI or API) capable of following structured prompts and returning JSON when requested.
4. Keep a log of prompts, responses, and accuracy measurements so you can complete the reflection items and share iteration insights.

## Prerequisites & Tooling
- Python 3.10+ environment with Jupyter support
- Access to a capable foundation model (e.g., OpenAI, Anthropic, Gemini, or an open-source model served locally)
- Familiarity with Python data handling and evaluating classification tasks
- Optional: spreadsheet or lightweight database to track prompt experiments and accuracy metrics

## Additional Resources
- Provider documentation for your chosen foundation model (prompt syntax, rate limits, formatting options)
- Guides on few-shot prompting and output parsing from Hugging Face or OpenAI
- Recommended Udacity readings on application design patterns for generative AI systems
