# Spectral Modularity Bisection on the Zachary Karate Club Graph  
### Community Detection using Leading Eigenvectors + ΔQ Stopping Rule

This repository contains an in-depth implementation of **spectral modularity bisection** on the classic  
**Zachary Karate Club** social network (34 nodes, 78 edges).

The project uses:
- **Leading eigenvector of the modularity matrix** for bisection  
- **Recursive splitting** to identify communities  
- **Two stopping conditions**:  
  1. Leading eigenvalue ≤ 0  
  2. Modularity gain ΔQ ≤ 0  
- **Node-level metrics** computed after each split  
- **Full visualization** of the community evolution  
- **Detailed discussion and interpretation**

The notebook follows the algorithmic steps typically required for a network science or graph mining assignment.

---

## 📘 Contents of the Notebook

The `.ipynb` file includes:

### **1. Construction of the modularity matrix (B = A − kkᵀ / 2m)**  
We compute the global modularity matrix and extract submatrices for each community during recursion.

### **2. Spectral bisection using the leading eigenvector**  
Nodes with positive eigenvector components → group 1  
Nodes with negative/equal → group 2  

### **3. ΔQ-based stopping rule**  
A split is accepted only if it *increases* modularity.

### **4. Recursive community detection**  
The graph is partitioned until no further modularity-improving splits remain.

### **5. Node-level metrics (computed after each split)**  
Using NetworkX:
- Degree centrality  
- Betweenness centrality  
- Closeness centrality  
- Clustering coefficient  

Each metric is tracked for **every node across all iterations**.

### **6. Visualization**  
- Community structure after each iteration  
- Evolution plots for all four node metrics  
- Embedded provided reference image  
- Final community structure

### **7. Full Discussion Section**  
Covers:
- Interpretation of splits  
- ΔQ behavior  
- Community structure  
- Centrality insights  
- Identification of important nodes

---

## 📂 Repository Structure

