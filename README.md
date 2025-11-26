# 🤖 Artificial Intelligence Course Projects

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

> **Course:** Artificial Intelligence
> **Status:** Complete

This repository contains three distinct projects exploring fundamental AI concepts: **Search Algorithms**, **Constraint Satisfaction**, and **Adversarial Game Playing**.

## 📂 Project Overview

| Project | Concept | Description |
| :--- | :--- | :--- |
| **1. Butter Robot** | Pathfinding & Search | Implements uninformed (BFS, DFS, IDS) and informed (A*, Best-First) search algorithms to navigate a grid world. |
| **2. CSP Solver** | Constraint Satisfaction | Solves complex scheduling/grouping problems using backtracking with MRV and LCV heuristics. |
| **3. Othello AI** | Adversarial Search | An AI agent that plays Othello (Reversi) using Minimax and Alpha-Beta pruning. |

---

## 1️⃣ Butter Robot (Search)
Located in: `/Butter-Robot`

A simulation where a robot must find the optimal path to its goal in a grid environment.

### Key Algorithms
* **Uninformed:** Breadth-First Search (BFS), Depth-First Search (DFS), Iterative Deepening Search (IDS), Uniform Cost Search (UCS).
* **Informed:** A* Search, Best-First Search (Greedy).

### How to Run
```bash
cd Butter-Robot/src
python Main.py