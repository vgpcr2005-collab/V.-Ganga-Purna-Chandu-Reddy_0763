# Journey to the Moon – HackerRank

## 📌 Problem Description

The **Journey to the Moon** problem is about finding the number of possible pairs of astronauts who can be selected for a space mission such that the two astronauts belong to **different countries**.

Astronauts from the same country are connected through the given pairs. The task is to identify all country groups and then count the possible pairs between different groups.

## 💡 Approach

This solution uses **Disjoint Set Union (DSU)**, also called **Union-Find**, to group astronauts belonging to the same country.

### Steps

1. Initially, every astronaut is treated as a separate group.
2. For every given astronaut pair, `union()` joins them into the same group.
3. `find()` identifies the root parent of each astronaut.
4. The size of each connected component represents the number of astronauts from that country.
5. Finally, pairs between different countries are calculated.

### DSU Optimizations Used

* **Path Compression** in `find()`
* **Union by Size** in `union()`

These optimizations make the operations efficient.

## 🧮 Pair Calculation

If the country sizes are:

```text
A = 3
B = 2
C = 4
```

The valid pairs are:

```text
A × B = 3 × 2
A × C = 3 × 4
B × C = 2 × 4
```

Total:

```text
6 + 12 + 8 = 26
```

The code calculates this efficiently using:

```python
answer += previous * count
previous += count
```

## ⏱️ Complexity

* **Time Complexity:** `O((n + p) × α(n))`
* **Space Complexity:** `O(n)`

Where:

* `n` = number of astronauts
* `p` = number of astronaut pairs
* `α(n)` = inverse Ackermann function, which grows extremely slowly.

## 🛠️ Technologies Used

* Python 3
* Disjoint Set Union (DSU)
* Union-Find
* Path Compression
* Union by Size

## ▶️ Input Format

```text
n p
a1 b1
a2 b2
...
ap bp
```

Where:

* `n` is the total number of astronauts.
* `p` is the number of astronaut pairs belonging to the same country.
* Each pair `a b` represents two astronauts from the same country.

## 📥 Example Input

```text
5 3
0 1
2 3
0 4
```

## 📤 Example Output

```text
6
```

## 📂 Files

```text
Journey-To-The-Moon/
│
├── journey_to_moon.py
└── README.md
```

## 🎯 Key Learning

This problem demonstrates how **Union-Find / DSU** can be used to efficiently find connected components and calculate combinations between different groups.
