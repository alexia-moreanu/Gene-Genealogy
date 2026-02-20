# Gene-Genealogy
Implemented local and global optimization algorithms to reconstruct genealogical relationships between mutated DNA sequences.
1. Problem Definition

Given a set of mutated DNA sequences, the goal of this project is to reconstruct their genealogy — identifying grandparent, parent, and child relationships — using algorithmic reasoning.

The challenge is to infer evolutionary structure purely from sequence similarity, and to compare how different algorithmic strategies affect the inferred genealogy.

⸻

2. Solution Specification

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
