# Udacity Generative AI Nanodegree - Course Materials

This repository contains the complete course materials for the Udacity Generative AI Nanodegree program. It includes hands-on exercises, projects, and comprehensive learning resources covering the fundamentals of generative AI and large language models.

## Course Overview

The Generative AI Nanodegree program provides comprehensive training in modern generative AI technologies, from foundational concepts to advanced implementation techniques. Students will learn to build, evaluate, and deploy generative AI applications using state-of-the-art tools and frameworks.

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

This repository includes three requirements files to help you set up the necessary dependencies:

### Core Dependencies
- **`requirements.txt`** - Contains all the core Python packages needed for the course, including Jupyter, OpenAI, transformers, and other essential libraries.

### PyTorch Dependencies
Choose the appropriate PyTorch installation based on your hardware:

- **`requirements-torch-cpu.txt`** - PyTorch installation for CPU-only systems
  - Use this if you don't have a CUDA-compatible GPU
  - Includes CPU-optimized versions of torch, torchaudio, and torchvision

- **`requirements-torch-gpu.txt`** - PyTorch installation for GPU systems
  - Use this if you have a CUDA-compatible GPU for faster training
  - Includes GPU-accelerated versions of torch, torchaudio, and torchvision

### Installation Instructions

1. **Install core dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Install PyTorch (choose one):**
   
   For CPU-only systems:
   ```bash
   pip install -r requirements-torch-cpu.txt
   ```
   
   For GPU systems:
   ```bash
   pip install -r requirements-torch-gpu.txt
   ```

3. **Verify your installation:**
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

**Note**: This repository contains educational materials for the Udacity Generative AI Nanodegree program. All content is designed for learning purposes and follows best practices in generative AI development.
