🎬 Item-Based Collaborative Filtering Recommendation System
🚀 Milestone 2 | Z5007 – Programming & Data Structures
---
✨ Why This Project?

Building recommender systems from scratch to deeply understand data structures, algorithms, and system design — without hiding behind ML libraries.

This project implements an Item-Based Collaborative Filtering (IBCF) engine using core programming constructs such as hash tables, graphs, and priority queues.
The emphasis is on algorithmic clarity, sparse data handling, and performance-aware design.

🧭 Project Snapshot
---

| 🔹 Aspect | 🔸 Details                              |
| --------- | --------------------------------------- |
| Course    | Z5007 – Programming and Data Structures |
| Milestone | Milestone 2                             |
| Technique | Item-Based Collaborative Filtering      |
| Language  | Python                                  |
| Dataset   | MovieLens (latest-small)                |

👥 Team
---
IIT Madras – Zanzibar

👩‍💻 Surabhi Gudla (ZDA25M001)
---
👨‍💻 Vineet Joshi (ZDA25M007)
---
🎓 Instructor: Dr. Innocent Nyalala
---

🗂️ Repository Layout
---
📦 item-based-recommender
 ┣ 📂 data
 ┃ ┣ ratings.csv
 ┃ ┗ movies.csv
 ┣ 📂 src
 ┃ ┣ preprocessing.py
 ┃ ┣ data_structures.py
 ┃ ┣ similarity.py
 ┃ ┗ graph_builder.py
 ┣ 📂 notebooks
 ┃ ┗ milestone2_demo.ipynb
 ┣ 📂 screenshots
 ┃ ┗ sample_outputs
 ┣ 📂 report
 ┃ ┗ Milestone_2_Progress_Report.pdf
 ┗ README.md

📊 Dataset Overview
---
🎥 MovieLens (latest-small) — a standard benchmark for recommender systems.
⭐ ~100,000 ratings
👤 ~600 users
🎬 ~9,000 movies

Files used:
ratings.csv → user-movie ratings
---
movies.csv → movie metadata
---

🧱 Core Building Blocks (Milestone-2)
---
🧠 Data Structures
🔹 Hash Tables
---
User → Movies rated with ratings
Movie → Users who rated it

🔹 Graph (Adjacency List)
---
Nodes = movies
Edges = similarity scores

🔹 Priority Queue (Heap)
---
Retains Top-50 similar movies per item
⚡ Enables fast lookup and memory-efficient storage for sparse data

⚙️ Algorithms Implemented
---
🎯 Item-Based Collaborative Filtering
---
Similarity computed between movies, not users

📐 Cosine Similarity
---
Uses overlapping users only
Filters weak/noisy relationships

🧹 Sparsity Handling
---
Minimum co-rating threshold
Similarity ≥ 0.1
Top-K pruning
Sparse adjacency list (no dense matrix)

⏱️ Performance Characteristics
---
| Component                 | Complexity    |
| ------------------------- | ------------- |
| Hash table build          | **O(N)**      |
| Item similarity (offline) | **O(M² × U)** |
| Adjacency list storage    | **O(M × K)**  |
| Lookup                    | **O(1)** avg  |

🖼️ Milestone-2 Outputs
---
✔ Dataset loading & train–test split
✔ Hash table sizes
✔ Sample user → movie mappings
✔ Sample movie → user mappings
✔ Item-item similarity graph
✔ Offline runtime measurement

📸 Screenshots available in /screenshots/
---

🚧 Challenges Solved
---
❗ Sparse User–Item Matrix
---
✔ Similarity only on overlapping users
✔ Thresholding + Top-K pruning

⚡ Performance Constraints
---
✔ Offline similarity computation
✔ Adjacency list instead of dense matrix
Current blockers: None ✅

🔜 What’s Next
---
🚀 Planned for next milestones:
---
Rating prediction
Top-N recommendations
Cold-start handling
Evaluation metrics (Precision@K, Recall@K, NDCG@K)
Class-based refactoring
Final benchmarking

📌 Milestone Status
---
✅ Core data structures implemented
✅ Core algorithm working
✅ Sample outputs generated
✅ On track for final submission
