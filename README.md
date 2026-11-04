# Hands-On Machine Learning — Working Repo

Chapter-by-chapter implementation and exercises from *Hands-On Machine
Learning with Scikit-Learn and PyTorch* (Géron), done as part of a
self-directed ML track alongside my B.Tech (CSE, AI & Data Science) at
Jamia Millia Islamia.

## Why this repo exists

Each chapter is treated as a set of milestones, not a standalone
tutorial run-through: conceptual answers to the book's own exercises,
a from-scratch NumPy/Python implementation of the chapter's core method
before reaching for the library version, and a short synthesis check
tying the chapter back to generalization, leakage, and evaluation —
the three things that break real ML systems most often.

## Structure

Each chapter gets its own folder:

CH<n>/
├── questions.md # back-of-chapter exercise answers, in my own words
├── gate-check.md # synthesis questions connecting this chapter
│ # to prior ones (not from the book)
├── <topic>.py # from-scratch implementation, no ML library
└── README.md # (if the chapter has a non-trivial deliverable
# beyond the two files above)


One commit per milestone within a chapter, so the commit history itself
shows the order concepts were built in, not just the final state.

## Progress

| Chapter | Topic | Status |
|---|---|---|
| 1 | The Machine Learning Landscape | ✅ Done — exercises, overfitting experiment (degree-1 vs degree-15 polynomial fit), gate check |
| 2 | End-to-End ML Project | 🔲 Not started |
| 3 | Classification | 🔲 Not started |
| 4 | Training Models (linear/poly regression, GD, regularization) | 🔲 Not started |
| 5 | Support Vector Machines | 🔲 Not started |
| 6 | Decision Trees | 🔲 Not started |
| 7 | Ensemble Learning, Random Forests | 🔲 Not started |
| 8 | Dimensionality Reduction | 🔲 Not started |
| 9 | Unsupervised Learning (Clustering, GMM) | 🔲 Not started |

(Part II — neural networks and deep learning — added once Part I is complete.)

## Environment

- Python 3.14
- NumPy, (Scikit-Learn / PyTorch added per chapter as needed)
- Run via GitHub Codespaces / local VS Code

## Notes on method

Where an exercise or experiment uses randomness, the seed is fixed and
stated explicitly in the script, so results are reproducible.