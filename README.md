
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

## 📁 Directory Structure

.
├── data/ # TSP instance generators and input graphs
├── models/ # GNN models and training logic
├── local_search/ # Heuristic algorithms for tour refinement
├── utils/ # Metrics, plotting, and helper functions
├── results/ # Output: plots, heatmaps, tour metrics
├── train.py # Training script
├── local_search.py # Local search execution
├── evaluate.py # Evaluation metrics and plots
└── README.md


## 🚀 Getting Started

### Clone the repository
```bash
git clone https://github.com/your-username/UTSP.git
cd UTSP
Install dependencies
pip install -r requirements.txt
Train the model
python train.py
Run local search on predicted heatmap
python local_search.py
Evaluate results
python evaluate.py
📊 Evaluation Metrics

Tour Length
Runtime
Optimality Gap (%)
Edge Heatmap Visualization
🔬 Experimental Insights

GAT outperformed SAG in sparse graphs.
Alternate loss functions reduced convergence time.
Improved local search led to ~3% better tours.
Scaled successfully up to n = 500 with optimized batch processing.
📚 References

📄 Paper: https://arxiv.org/abs/2303.10538
💻 Original UTSP Repo: https://github.com/yimengmin/UTSP
👥 Mentors

Shivansh Gupta – 9560749686
Toshit Jain – 6354642173
📬 Contact

For any queries or contributions, raise an issue or open a pull request.

