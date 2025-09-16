# Diffusion Transformer (minDiT)

[![Python](https://img.shields.io/badge/python-3.9-blue)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/pytorch-2.1.1-red)](https://pytorch.org/)
[![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)

Implementation of the Diffusion Transformer model (DiT) from the paper:

> [Scalable Diffusion Models with Transformers](https://arxiv.org/abs/2212.09748)

Official PyTorch implementation by Facebook Research: [DiT](https://github.com/facebookresearch/DiT)

---

## Table of Contents

- [Preview](#preview)
- [Dependencies](#dependencies)
- [Training minDiT](#training-mindit)
- [Implementation Notes](#implementation-notes)
- [Todo](#todo)

---

## Preview

<img src="./img/latentdit.png" width="450px" alt="DiT Architecture" />

### Sample Outputs

**minDiT (39.89M parameters) on CIFAR-10:**

<img src="./img/ditcifar.png" width="550px" alt="CIFAR-10 Samples" />

**minDiT on CelebA:**

<img src="./img/ditceleba64.png" width="650px" alt="CelebA Samples" />

**More Samples:**

<img src="./img/minditcifar.gif" width="650px" alt="CIFAR-10 GIF Samples" />
<img src="./img/minditceleba64.gif" width="550px" alt="CelebA GIF Samples" />

---

## Dependencies

- Python 3.9
- PyTorch 2.1.1
- Other standard libraries: `torchvision`, `numpy`, `PIL`, `scipy`, `tqdm`, `matplotlib`

---

## Training minDiT

Run the training script and specify the dataset path:

```bash
python train.py --data_dir=./data/
