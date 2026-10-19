# Lab Report 1: Interactive BFS & DFS Search Algorithms

**Course:** BSD3513 Introduction to Artificial Intelligence  
**Student:** Lau Yu Yang (SD24045)  
**Lecturer:** Assoc. Prof. Dr. Ku Muhammad Naim Ku Khalif  
**Institution:** Universiti Malaysia Pahang Al-Sultan Abdullah (UMPSA)

---

## Overview
This repository contains an interactive Python web application built with **Streamlit** for **Lab #1**. The application visualizes and compares two fundamental uninformed search algorithms on directed graphs with alphabetical tie-breaking:
* **Breadth-First Search (BFS):** Explores the graph level by level using a First-In, First-Out (FIFO) queue[cite: 3]. Guarantees the shortest path (minimum hops) in unweighted graphs.
* **Depth-First Search (DFS):** Explores deeply along each branch before backtracking using a Last-In, First-Out (LIFO) stack[cite: 2, 5].

---

## Features
* **Live Directed Graph Editor:** Add, remove, or modify directed edges and isolated nodes directly from the sidebar.
* **Custom Search Controls:** Select any starting node, an optional goal node, and choose to run **BFS**, **DFS**, or **Both** simultaneously.
* **Step-by-Step Interactive Visualization:** Inspect the exact state of the graph at every expansion step using an interactive slider, with color-coded nodes (current, visited, and unvisited)[cite: 1].
* **Level & Trace Breakdown:** View total levels reached, node groupings per level (`L0`, `L1`, `L2`, ...), step-by-step trace tables, and live frontier states[cite: 3].
* **BFS vs. DFS Comparison Table:** Side-by-side summary comparing data structures, expansion orders, expanded node counts, maximum frontier sizes, deepest levels reached, and goal paths[cite: 2, 5].

---

## Default Graph Structure
* **Edges:** `A → B, D` | `B → C, E, G` | `C → A` | `D → C` | `E → H` | `G → F` | `H → F, G` | `F → None`
* **Default BFS Order (from A):** `A → B → D → C → E → G → H → F`[cite: 2, 3, 5]
* **Default DFS Order (from A):** `A → B → C → E → H → F → G → D`[cite: 2, 5]

---

## Installation & How to Run Locally

1. **Clone this repository:**
   ```bash
   git clone <your-github-repo-url>
   cd "Lab Report 1"
