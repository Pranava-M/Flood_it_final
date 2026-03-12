# Flood_it
# Flood-It Algorithm Solver 🎮

A Java-based visual simulator for the **Flood-It puzzle**, demonstrating multiple algorithmic approaches used to solve the game automatically.

This project compares **four different algorithm design techniques** and shows how each algorithm solves the same grid.

The project is implemented using **Java Swing** to provide a visual interface.

---

## 📌 Project Objective

The goal of the project is to demonstrate how different algorithmic strategies behave when solving the **Flood-It puzzle**.

The algorithms implemented are:

1. Bucket Sort + BFS (Greedy)
2. Divide and Conquer
3. Backtracking
4. Dynamic Programming

Each algorithm runs on a **separate grid**, allowing direct comparison of their solving strategies.

---

## 🎯 About the Flood-It Game

Flood-It is played on an **N × N grid** containing multiple colors.

Rules:

- The flood starts at the **top-left cell (0,0)**.
- Each move selects a new color.
- The selected color **expands the flooded region** to adjacent cells of the same color.
- The objective is to **make the entire grid one color using minimum moves**.

---

## 🧠 Algorithms Implemented

### 1️⃣ Bucket Sort + BFS (Greedy)

This method uses **Breadth First Search** to identify the flooded region and counts neighboring colors.

The algorithm chooses the color that appears **most frequently around the flood boundary**.

**Steps:**

1. Use BFS to detect the current flooded region.
2. Count neighboring colors.
3. Sort the counts using bucket sorting.
4. Select the color with the highest count.

**Advantages**
- Fast execution
- Simple logic

**Disadvantages**
- Not guaranteed to find the optimal solution.

---

### 2️⃣ Divide and Conquer

This approach divides the grid into conceptual regions and selects colors that expand toward **dominant color clusters**.

**Steps:**

1. Divide the grid into smaller logical regions.
2. Analyze color distribution.
3. Greedily select the color that expands toward larger clusters.

**Advantages**
- Faster than exhaustive search
- Efficient for structured boards

**Disadvantages**
- Heuristic based.

---

### 3️⃣ Backtracking

Backtracking explores **all possible color sequences recursively**.

**Steps:**

1. Try each possible color.
2. Simulate flood expansion.
3. Recursively search for the best sequence.
4. Track the minimum number of moves.

**Advantages**
- Can find optimal solutions.

**Disadvantages**
- Exponential time complexity.

---

### 4️⃣ Dynamic Programming

Dynamic programming avoids recomputation by storing **previously solved board states**.

**Steps:**

1. Encode the grid state.
2. Store solutions in a memoization table.
3. Reuse stored solutions when the same state appears.

**Advantages**
- Reduces repeated computation
- Faster than pure backtracking.

**Disadvantages**
- Requires additional memory.

---

## 🖥️ Technologies Used

- **Java**
- **Java Swing** (GUI)
- **BFS Algorithm**
- **Recursion**
- **Dynamic Programming**
- **Greedy Strategy**

---

## 📂 Project Structure
