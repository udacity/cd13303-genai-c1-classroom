# Generative AI Fundamentals - Course Materials

This repository contains the complete course materials for the Udacity Generative AI Fundamentals course. It includes hands-on exercises, projects, and comprehensive learning resources covering the fundamentals of generative AI and large language models.

## Course Overview

The Generative AI Fundamentals course provides comprehensive training in modern generative AI technologies, from foundational concepts to advanced implementation techniques. Students will learn to build, evaluate, and deploy generative AI applications using state-of-the-art tools and frameworks.

## Repository Structure

```
├── module-3-applications-of-generative-ai/
│   ├── exercises/
│   │   ├── starter/          # Student starting materials
│   │   └── solution/         # Complete solutions
│   └── README.md
├── module-5-building-applications-using-foundation-models/
│   ├── exercises/
│   │   ├── starter/
│   │   └── solution/
│   └── README.md
├── module-8-implementing-evaluations-for-generative-ai-models/
│   ├── exercises/
│   │   ├── starter/
│   │   └── solution/
│   └── README.md
├── module-10-implementing-neural-networks-using-pytorch/
│   ├── exercises/
│   │   ├── starter/
│   │   └── solution/
│   └── README.md
├── module-12-generating-text-using-llms/
│   ├── exercises/
│   │   ├── starter/
│   │   └── solution/
│   └── README.md
├── module-14-implementing-role-based-prompting-in-python/
│   ├── exercises/
│   │   ├── starter/
│   │   └── solution/
│   └── README.md
├── module-16-applying-peft-on-foundation-models/
│   ├── exercises/
│   │   ├── starter/
│   │   └── solution/
│   └── README.md
├── module-18-reinforcement-fine-tuning-on-foundation-models/
│   ├── exercises/
│   │   ├── starter/
│   │   └── solution/
│   └── README.md
├── project/
│   ├── starter/              # Capstone project materials
│   └── solution/
└── README.md
```

## Requirements and Dependencies

This repository includes three requirements files, one per group of modules. Install only the file for the modules you are working on, using Python 3.12.

### Available Files

- **`requirements3-5.txt`** - Modules 3 and 5: applications of generative AI and building applications using foundation models.
- **`requirements8-10-12.txt`** - Modules 8, 10, and 12: evaluations, PyTorch, and text generation. This is `venv1` in the Vocareum workspace.
- **`requirements16-18-project.txt`** - Modules 16 and 18 plus the course project: adds `torch`, `vllm`, `unsloth`, and `triton` for PEFT and GRPO fine-tuning. Requires a CUDA GPU. This is `venv2` in the Vocareum workspace.

### Installation Instructions

1. **Modules 3 and 5:**
   ```bash
   pip install -r requirements3-5.txt
   ```

2. **Modules 8, 10, and 12:**
   ```bash
   pip install -r requirements8-10-12.txt
   ```

3. **Modules 16, 18, and the project (GPU):**
   ```bash
   pip install -r requirements16-18-project.txt --no-deps
   ```

   **`--no-deps` is required here:** this file deliberately pins `triton==3.2.0`, below the `triton==3.3.1` that `torch==2.7.1` asks for, because Triton 3.3.x cannot compile vLLM's LoRA kernels on Turing GPUs (Tesla T4, compute capability 7.5) - without `--no-deps` the resolver upgrades Triton and the project notebook fails on model load with `RuntimeError: PassManager::run failed`.

4. **Verify your installation:**
   ```python
   import torch
   print(f"PyTorch version: {torch.__version__}")
   print(f"CUDA available: {torch.cuda.is_available()}")
   ```

## Course Materials

Each module contains:
- **Comprehensive README** with learning objectives and setup instructions
- **Hands-on exercises** with starter code and complete solutions
- **Demo notebooks** showcasing key concepts
- **Detailed documentation** for all exercises and projects

## License

This educational content is licensed under the **Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)** License. See [LICENSE.md](LICENSE.md) for full details.

## Support

For questions about course content or technical issues:
- Review the module-specific README files
- Check the exercise solutions for reference implementations
- Consult the Udacity Generative AI Nanodegree resources

---

**Note**: This repository contains educational materials for the Udacity Generative AI Fundamentals course. All content is designed for learning purposes and follows best practices in generative AI development.
