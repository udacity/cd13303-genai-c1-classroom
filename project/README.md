# GenAI C1 Project: Teach an LLM to Reason

This project guides you through teaching an instruction-tuned LLM to reason step‑by‑step using GRPO (Group Relative Policy Optimization). The model learns to break a word into letters and count a specific letter.

Key notebooks and files:
- `project/starter/gen_ai_fundamentals_project_starter.ipynb`
- `project/solution/gen_ai_fundamentals_project_solution.ipynb`
- `requirements.txt`

## Hardware

- Runs on a single "T4 Tesla" GPU with 16GB VRAM (e.g., AWS `g4dn.xlarge`).

## NVIDIA Driver and CUDA (tested)

- OS: Ubuntu 24.04 (x86_64)
- NVIDIA driver: 575.57.08
- CUDA: 12.9.1

Install driver + CUDA toolkit only if you are sure drivers/CUDA are not already installed on your system (if you can run nvidia-smi, you have them installed definitely).
```
sudo apt update && sudo apt install gcc make -y
wget https://developer.download.nvidia.com/compute/cuda/12.9.1/local_installers/cuda_12.9.1_575.57.08_linux.run
sudo sh cuda_12.9.1_575.57.08_linux.run --silent --toolkit --driver --no-drm
```

## Other Dependencies

Install uv and Python headers:
```
curl -LsSf https://astral.sh/uv/install.sh | sh
```
Restart your terminal to ensure `uv` is available.

## Environment Setup

From the repository root (or the `project/` directory):
```
uv python pin 3.12.3
uv init
uv sync
uv add ipykernel pip
uv pip install -r requirements.txt  --no-deps
```

## Run the Project

- Open `project/starter/gen_ai_fundamentals_project_starter.ipynb` in Jupyter and select the `.venv` kernel.
- Execute cells in order. The notebook installs any remaining Python dependencies needed for training and evaluation.


## Built With

- PyTorch, Transformers, Unsloth, vLLM, TRL

## License

See `LICENSE.md`.
