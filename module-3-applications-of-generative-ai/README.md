# Applications of Generative AI

This module explores how to translate real-world problems into generative AI workflows. You will practice spotting automation opportunities, orchestrating language model prompts, and validating the outputs against traditional software expectations.

## Learning Outcomes
- Identify scenarios where generative AI can accelerate software development tasks
- Break down open-ended prompts into reproducible steps for an LLM collaborator
- Critically evaluate LLM-generated code and tests against quality and safety criteria
- Capture and communicate iteration history when refining model outputs

## Exercise Overview
- **LLM-Assisted Merge Sort Workshop** (`exercises/`): Use a large language model to draft a Python merge sort implementation and accompanying tests, then iteratively refine the solution while documenting each prompt, revision, and reflection. Starters and solutions are provided so you can practice independently or review a worked example.

## Directory Map
- `exercises/INTRODUCTION.md` – learner-facing overview for the hands-on activity
- `exercises/INSTRUCTIONS.md` – step-by-step walkthrough of the exercise workflow
- `exercises/starter/` – starter notebook and assets for students
- `exercises/solution/` – reference implementation, exercise specification (`exercise.yml`), and facilitation notes

## Getting Started
1. Review the introduction and instructions inside `exercises/` to understand the scenario and deliverables.
2. Launch the starter notebook from `exercises/starter/llm-assisted-merge-sort-starter.ipynb` (or open in your preferred notebook environment).
3. Keep a record of every prompt/response exchange with the LLM so you can reflect on the iteration log requested in the exercise brief.
4. Compare your work with the solution notebook when you want to check your approach or prepare for facilitation.

## Prerequisites & Tooling
- Python 3.10+ with Jupyter Lab/Notebook support
- Access to at least one capable language model (web chat or API)
- Familiarity with basic Python functions, lists, and unit testing
- Optional: version control to track iterations and prompt transcripts

## Additional Resources
- [Udacity Generative AI Nanodegree Resources](https://www.udacity.com/) for supplemental readings
- Hugging Face guides on prompt engineering and evaluation best practices
- Python standard library documentation for reference implementations and testing utilities
