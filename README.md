# Gene-Genealogy

🧬 Decoding the Relationship Between Genes

Reconstructing genealogy relationships between mutated DNA sequences using local and global algorithmic strategies.

⸻

📌 Problem Definition

Given a set of mutated gene sequences, the goal of this project is to reconstruct their genealogy (grandparent → parent → child relationships) using only sequence similarity.

The challenge is to determine how different algorithmic strategies influence the inferred evolutionary structure.

⸻

⚙️ Solution Specification

I implement two distinct approaches:

🔹 Local Strategy (Greedy, Pairwise-Based)
	•	Compute pairwise similarity using Longest Common Subsequence (LCS)
	•	Convert similarity into a normalized distance matrix
	•	Construct a genealogy tree using greedy, local decisions
	•	Score the tree based on edge distances

This approach prioritizes efficiency and immediate proximity.

⸻

🔹 Global Strategy (Optimization-Based)
	•	Compute global alignment scores using Needleman–Wunsch dynamic programming
	•	Convert alignment scores into distances
	•	Evaluate all valid tree configurations
	•	Select the tree minimizing a global objective

This approach evaluates the genealogy holistically, prioritizing overall consistency.

⸻

🔬 Additional Analysis
	•	Experimental complexity analysis (Θ(N²M²) dynamic programming scaling)
	•	Log–log runtime comparisons
	•	Mutation probability estimation (insertions, deletions, substitutions)
	•	Laplace smoothing for small-sample robustness
	•	Deterministic traceback for reproducibility

⸻

📂 What You’ll Find in This Repository
	•	LCS implementation (CLRS-based DP)
	•	Needleman–Wunsch global alignment
	•	Pairwise similarity + distance matrices
	•	Greedy local genealogy inference
	•	Global tree optimization
	•	Tree scoring functions
	•	Runtime scaling experiments
	•	Mutation probability estimation pipeline

⸻

🎥 Project Walkthrough Videos
	•	🎥 [Video 1]([url](https://www.loom.com/share/52436fdb527441778123f5f3994ac6f1)) – Local vs Global Strategy Explanation
	•	🎥 [Video 2]([url](https://www.loom.com/share/9771c7fa796d45159f990d32a9425a25)) – Mutation Probability Estimation

⸻

🚀 Why This Project?

This project explores the trade-off between local decision-making and global optimization in structured inference problems.

It connects:
	•	Dynamic programming
	•	Graph/tree reasoning
	•	Optimization
	•	Biological interpretation

It reflects my interest in building computational systems that translate raw biological data into interpretable structure.

⸻

If you’d like, I can also:
	•	Make a shorter version for quick recruiter scanning
	•	Make a more research-heavy academic framing
	•	Or make a more SWE-focused technical README

Just tell me the audience.
I implement two strategies:

Local Strategy (Greedy)
	•	Computes pairwise similarity using Longest Common Subsequence (LCS).
	•	Converts similarity into normalized distances.
	•	Builds a genealogy tree using greedy, local decisions based only on nearest neighbors.

Global Strategy (Optimization-Based)
	•	Uses Needleman–Wunsch global alignment to compute sequence distances.
	•	Evaluates all valid tree configurations.
	•	Selects the tree minimizing a global distance objective.

I then:
	•	Compare the inferred trees
	•	Analyze computational complexity (Θ(N²M²) DP scaling)
	•	Estimate mutation probabilities (insertions, deletions, substitutions) using alignment tracebacks and Laplace smoothing.

⸻

3. What You’ll Find in This Repo
	•	Dynamic programming implementation of LCS and Needleman–Wunsch
	•	Pairwise similarity and distance matrix construction
	•	Local greedy genealogy inference
	•	Global tree optimization
	•	Complexity analysis with experimental scaling plots
	•	Mutation probability estimation from inferred genealogies

⸻

4. Why This Project?

This project connects algorithm design with biological interpretation.

It explores:
	•	Local vs. global optimization trade-offs
	•	Dynamic programming in real biological contexts
	•	How computational models can reveal evolutionary structure

It reflects my interest in working at the intersection of algorithms, systems thinking, and computational biology.
