
# 🧠 Unsupervised Travelling Salesman Problem (UTSP)

This repository contains an implementation and extension of the **UTSP** framework, which applies Graph Neural Networks (GNNs) and unsupervised learning to solve the Travelling Salesman Problem (TSP) without labeled data. The model predicts a heatmap of edge probabilities and uses local search heuristics to derive near-optimal tours.

## 📝 Problem Statement

Replicate and enhance the UTSP model from the original paper [arXiv:2303.10538](https://arxiv.org/abs/2303.10538), which learns tour patterns via surrogate loss functions without supervised labels. The project includes architectural improvements, scalable extensions, and performance benchmarking.

## 📌 Objectives

- Reimplement the UTSP model from scratch.
- Explore alternate GNNs (GAT, GIN, GraphSAGE).
- Experiment with different surrogate loss functions.
- Modify and enhance the local search procedure.
- Improve T → H transformation.
- Scale to TSP sizes: n = 20, 50, 100, 200, 500.
- Compare modified models against the UTSP baseline.

## 🛠 Tech Stack

- **Programming**: Python
- **Libraries**:
  - PyTorch, PyTorch Geometric (GNN Modeling)
  - NumPy, NetworkX (Graph Handling)
  - Matplotlib (Visualization)

