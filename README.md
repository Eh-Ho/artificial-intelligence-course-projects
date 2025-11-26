# 🤖 Artificial Intelligence Course Projects

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

> **Course:** Artificial Intelligence  
> **Status:** Complete  

This repository contains a collection of three distinct projects exploring fundamental AI concepts: **Search Algorithms**, **Constraint Satisfaction**, and **Adversarial Game Playing**.

## 📂 Project Overview

| Project | Concept | Description |
| :--- | :--- | :--- |
| **1. Butter Robot** | Pathfinding & Search | Implements uninformed (BFS, DFS, IDS) and informed (A*, Best-First) search algorithms to navigate a grid world. |
| **2. CSP Solver** | Constraint Satisfaction | Solves complex scheduling/grouping problems using backtracking with MRV and LCV heuristics. |
| **3. Othello AI** | Adversarial Search | An AI agent that plays Othello (Reversi) using Minimax and Alpha-Beta pruning. |

---

## 1️⃣ Butter Robot (Search Algorithms)
**Location:** `/Butter-Robot`

A simulation where a robot must find the optimal path to its goal in a grid environment. The project models the environment as a graph and applies various search strategies to find the solution.

### Key Algorithms Implemented
* **Uninformed Search:**
    * Breadth-First Search (BFS)
    * Depth-First Search (DFS)
    * Iterative Deepening Search (IDS)
    * Uniform Cost Search (UCS)
* **Informed (Heuristic) Search:**
    * A* Search (A-Star)
    * Greedy Best-First Search

### 💻 How to Run
```bash
cd Butter-Robot/src
python Main.py
````

*Note: The program reads the map configuration from `test/input*.txt` files.*

-----

## 2️⃣ CSP Solver (Constraint Satisfaction)

**Location:** `/CSP`

A generic Constraint Satisfaction Problem (CSP) solver designed to handle constraints between different groups and halls (e.g., allocation problems). It attempts to assign values to variables while satisfying all defined constraints.

### Key Concepts

  * **Backtracking:** Recursive search that builds candidates and abandons them ("backtracks") as soon as it determines they cannot lead to a valid solution.
  * **Heuristics:**
      * **MRV (Minimum Remaining Values):** Selects the variable with the fewest remaining legal values to spot failures early.
      * **LCV (Least Constraining Value):** Selects the value that rules out the fewest choices for neighboring variables to maximize flexibility.

### 💻 How to Run

```bash
cd CSP/src
python Main.py
```

-----

## 3️⃣ Othello AI (Game Theory)

**Location:** `/Othello-minimax`

A fully playable implementation of the board game **Othello (Reversi)** featuring an AI opponent. The AI evaluates the board state to make optimal moves against a human player.

### Key Algorithms Implemented

  * **Minimax:** A decision rule used for minimizing the possible loss for a worst-case scenario (maximum loss).
  * **Alpha-Beta Pruning:** An optimization technique for the minimax algorithm that reduces the number of nodes evaluated by the search tree.
  * **Heuristic Evaluation:** A custom function that scores board states based on:
      * **Corner Control:** Corners are stable and valuable.
      * **Mobility:** The number of available moves.
      * **Stability:** Discs that cannot be flipped.

### 💻 How to Run

```bash
cd Othello-minimax/src
python Main.py
```

*This command launches the `GameManager` loop.*

-----

## 🛠 Tech Stack

  * **Language:** Python 3
  * **Libraries:** Standard Python libraries (`collections`, `math`, `random`, `copy`).
  * **Approach:** implementations are built from scratch without external ML frameworks (like TensorFlow or PyTorch) to demonstrate core algorithmic understanding.
