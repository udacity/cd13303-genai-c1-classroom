# Starter Folder

Use this notebook to complete the GenAI C1 project: teach an instruction‑tuned LLM to reason step‑by‑step (letter counting with GRPO).

- Main file: `project/starter/gen_ai_fundamentals_project_starter.ipynb`

## Environment and Hardware

- Single "T4 Tesla" GPU with 16GB VRAM (e.g., AWS `g4dn.xlarge`).
- Tested with NVIDIA driver 575.57.08 and CUDA 12.9.1 on Ubuntu 24.04 x86_64.

Install driver + CUDA only if you are sure they are not already installed (nvidia-smi will run properly if you have it installed)
```
sudo apt update && sudo apt install gcc make -y
wget https://developer.download.nvidia.com/compute/cuda/12.9.1/local_installers/cuda_12.9.1_575.57.08_linux.run
sudo sh cuda_12.9.1_575.57.08_linux.run --silent --toolkit --driver --no-drm
```

Install uv and Python headers:
```
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Set up the Python environment from the repo root:
```
uv python pin 3.12.3
uv init
uv sync
uv add ipykernel pip
uv pip install -r requirements.txt
```

Open and run the starter notebook with the `.venv` kernel.
