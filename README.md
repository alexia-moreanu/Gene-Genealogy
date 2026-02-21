# 🧬 Gene-Genealogy  
## Decoding the Relationship Between Genes

Reconstructing genealogy relationships between mutated DNA sequences using local and global algorithmic strategies.

---

## 📌 Problem Definition

Given a set of mutated gene sequences, the goal of this project is to reconstruct their genealogy  
(**grandparent → parent → child relationships**) using only sequence similarity.

The core challenge is understanding how different algorithmic strategies influence the inferred evolutionary structure.

---

## ⚙️ Solution Specification

I implement two distinct approaches to infer genealogical structure:

### 🔹 Local Strategy (Greedy, Pairwise-Based)

- Compute pairwise similarity using **Longest Common Subsequence (LCS)**
- Convert similarity into a normalized distance matrix
- Construct a genealogy tree using greedy, local decisions
- Score the tree based on edge distances

This approach prioritizes efficiency and immediate proximity.

---

### 🔹 Global Strategy (Optimization-Based)

- Compute global alignment scores using **Needleman–Wunsch dynamic programming**
- Convert alignment scores into distances
- Evaluate all valid tree configurations
- Select the tree minimizing a global objective

This approach evaluates the genealogy holistically, prioritizing overall consistency.

---

## 🔬 Additional Analysis

- Experimental complexity analysis (**Θ(N²M²)** dynamic programming scaling)
- Log–log runtime comparisons
- Mutation probability estimation (insertions, deletions, substitutions)
- Laplace smoothing for small-sample robustness
- Deterministic traceback for reproducibility

---

## 📂 What You’ll Find in This Repository

- LCS implementation (CLRS-based dynamic programming)
- Needleman–Wunsch global alignment
- Pairwise similarity and distance matrix construction
- Greedy local genealogy inference
- Global tree optimization
- Tree scoring functions
- Runtime scaling experiments
- Mutation probability estimation pipeline

---

### 🎥 Project Walkthrough Videos

🎥 [Local vs Global Strategy Explanation](https://www.loom.com/share/52436fdb527441778123f5f3994ac6f1)  
🎥 [Mutation Probability Estimation](https://www.loom.com/share/9771c7fa796d45159f990d32a9425a25)

---

## 🚀 Why This Project?

This project explores the trade-off between **local decision-making and global optimization** in structured inference problems.

It connects:

- Dynamic programming
- Graph/tree reasoning
- Optimization
- Biological interpretation

It reflects my interest in building computational systems that translate raw biological data into interpretable evolutionary structure.
