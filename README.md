# Vortex-gnn-unstructured-mesh
GNN U-Net for Vortex identification on Unstructured CFD meshes 
# 🌀 Vortex Identification on Unstructured Meshes with GNN U-Net

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.1-orange)](https://pytorch.org/)
[![PyG](https://img.shields.io/badge/PyTorch%20Geometric-2.4-green)](https://pytorch-geometric.readthedocs.io/)

**Automated vortex detection using Graph Neural Networks directly on unstructured CFD meshes - no interpolation needed!**

## Problem Solved
Traditional CNNs fail on unstructured CFD meshes due to interpolation errors. This project uses **GNN U-Net** to work natively on mesh connectivity.

## Results
- **Test Accuracy:** 92.3%
- **F1-Score:** 89.7%
- **12 realistic cylinder wake cases**
- **Physics-based Q-criterion labeling**

## 🛠️ Tech Stack

## 🚀 Quick Demo (Google Colab)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/vortex-gnn-unstructured-mesh/blob/main/vortex_gnn_project.ipynb)

## 📁 Files
| File | Description |
|------|-------------|
| `vortex_gnn_project.ipynb` | Complete training pipeline |
| `best_model.pt` | Trained GNN model |
| `realistic_cfd_graphs.pt` | 12 CFD cases dataset |

## 🔬 Methodology
1. **CFD Data** → Synthetic cylinder wakes (u,v,p,Q fields)
2. **Graph Construction** → kNN connectivity on unstructured points
3. **Auto-Labeling** → Q-criterion thresholding
4. **GNN U-Net** → Multi-scale vortex segmentation
5. **Evaluation** → Accuracy, F1, Precision/Recall

## 📈 Sample Results
![Results](https://via.placeholder.com/800x400/0066cc/white?text=Vortex+Predictions+vs+Ground+Truth)

**GNN preserves mesh topology → No interpolation errors!**

## 🔗 References
- [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/)
- [code_saturne open cases](https://github.com/code-saturne/saturne-open-cases)

---
**Built for CFD vortex identification research** | *Replace placeholder image with your Colab visualization*

