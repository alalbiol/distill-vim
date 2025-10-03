# distill-vim

**Distill-ViM** is a PyTorch framework for **knowledge distillation from state-of-the-art CNNs and Vision Transformers into Vision Mamba (ViM)** students.  
The goal is to improve the accuracy, calibration, and robustness of efficient state-space models while keeping their low latency and memory footprint.

---

## 🔹 Features
- Baseline **fine-tuning of ViM models** on ImageNet.  
- **Logit distillation** with KL divergence and Jensen–Shannon divergence.  
- Planned: **Bidirectional-aware Feature Distillation (Bi-KD)** to exploit forward–backward scanning in ViM.  
- Easy configuration via command line or YAML configs.  
- Training and evaluation scripts for ImageNet and transfer datasets (CIFAR-100, Food-101, Oxford Pets).  
- Reproducible experiments with checkpoints and W&B logging.  

---

## 🔹 Installation

```bash
# clone repo
git clone https://github.com/alalbiol/distill-vim.git
cd distill-vim

# create env (conda or venv)
conda create -n distillvim python=3.10 -y
conda activate distillvim

# install dependencies
pip install -r requirements.txt
