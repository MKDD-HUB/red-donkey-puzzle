# 🧩 Red Donkey Puzzle — BFS vs A* Algorithm Comparison (Browser Animation)

This project implements the **Red Donkey sliding block puzzle** and solves it using two different Artificial Intelligence search algorithms:

- ✅ Breadth First Search (BFS)
- ✅ A* Search (A-star)

Both algorithms solve the **same hard puzzle configuration**, and their performance is compared based on:

- Execution Time (milliseconds)
- Number of States Explored (used as space complexity approximation)

The solution is visualized using **real-time browser animation** with HTML Canvas and is hosted using **GitHub Pages**.

---

## 🎯 Problem Description

The Red Donkey Puzzle is a sliding block puzzle where:

- Blocks can move only up, down, left, or right
- Blocks cannot overlap
- Blocks must remain inside the board
- Only one block moves at a time
- The goal is to move the **red block** to the exit at the bottom center

The puzzle starts in a **hard configuration** where several blocks block the red block from directly reaching the exit.

Each board arrangement is treated as a **state** in the search space.

---

## 🧠 Algorithms Implemented

### 🔹 1. Breadth First Search (BFS)

File: `bfs.html`

- Explores all states level by level
- Does not use heuristic information
- Guarantees shortest path
- Very high memory usage
- Slower for large state spaces

Time Complexity: **O(b^d)**  
Space Complexity: **O(b^d)**

Where:
- b = branching factor
- d = depth of solution

---

### 🔹 2. A* Search (A-star)

File: `astar.html`

- Uses heuristic guidance
- Heuristic used: Manhattan distance of red block to exit
- Explores fewer states
- Faster and more memory efficient
- Still guarantees optimal solution

Worst-case Time Complexity: **Exponential**  
Practical performance is much better than BFS due to heuristic guidance.

---

## 📊 Performance Comparison

Each program displays:

- Number of states explored during search
- Execution time in milliseconds
- Step-by-step animation of solution

By comparing results from both programs, it can be clearly observed that:

- BFS explores many more states
- BFS takes more time and memory
- A* is significantly more efficient

This demonstrates the advantage of **informed search over uninformed search**.

---

## 🎨 Graphical Representation & Animation

- Board size: **5 × 4 grid**
- Implemented using HTML `<canvas>`
- Blocks drawn as rectangles
- Exit area highlighted
- Each solution step is animated sequentially

Both algorithms use the **same animation system**, ensuring fair visual comparison.

---

## ▶ How to Run

### 🌐 Run Online (GitHub Pages)

After enabling GitHub Pages:

- BFS Solver:
