# Karate Club — Recursive Spectral Modularity Partitioning

This repository contains a Jupyter notebook and all generated outputs for a Recursive Spectral Modularity Partitioning assignment on Zachary's Karate Club graph.

**Repository contents**
```
karate_github_package/
├── karate_modularity.ipynb
└── karate_modularity_outputs/
    ├── partition_iter_0.png
    ├── partition_iter_1.png
    ├── ...
    ├── metric_evolution_degree.png
    ├── metric_evolution_betweenness.png
    ├── metric_evolution_closeness.png
    ├── metric_evolution_clustering.png
    ├── heatmap_degree.png
    ├── heatmap_betweenness.png
    ├── heatmap_closeness.png
    ├── heatmap_clustering.png
    ├── metrics_over_iterations.json
    ├── discussion_summary.txt
    ├── discussion_summary.json
    └── layout.json
```

## How to use
1. Open `karate_modularity.ipynb` in Jupyter, JupyterLab, Colab, or VS Code.
2. Run the notebook top-to-bottom (it should execute without edits) to regenerate outputs if desired.
3. All pre-generated images and JSONs are in `karate_modularity_outputs/` so you can preview them directly on GitHub (click each image).

## Notes
- **Libraries used:** `numpy`, `networkx`, `matplotlib` (no `pandas` or `seaborn` required).  
- Central nodes and modularity are computed and saved to `discussion_summary.txt` and `metrics_over_iterations.json`.
- The notebook includes functions to compute modularity `Q` for any partition, visualize partitions at each split, compute per-community (induced-subgraph) centrality metrics, plot metric evolution, and save heatmaps.

## Quick summary of results (automated)
- Top nodes by frequency in top-3 across iterations per metric are saved in `karate_modularity_outputs/discussion_summary.txt` and `.json`.
- Heatmaps and metric-evolution plots are provided for degree, betweenness, closeness, and clustering.


