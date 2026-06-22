# 📓 Personal Reflection — Data Mining (SECP2753)
---

## Assignment 1 — Business Insights from Student Grading Data

This assignment applied the CRISP-DM framework to a dataset of 5,000 student records to uncover patterns through visualization. The most thought-provoking part was the sleep hours and stress level insights, both of which produced non-linear results that challenged common assumptions — students sleeping exactly 6 hours outperformed those sleeping 8, and students at extreme stress levels outperformed those in the moderate range. Working through those findings taught me the difference between describing what a chart shows and actually interpreting what it means, which is a distinction I want to carry into every analysis going forward.

---

## Assignment 2 — FP-Tree Algorithm for Frequent Pattern Mining

This assignment required manually constructing an FP-Tree from a small electronics transaction dataset, deriving conditional pattern bases and conditional FP-Trees for each item, and comparing FP-Growth against the Apriori algorithm. Tracing the algorithm by hand — especially building the conditional pattern base for items like Charger with multiple branches — was tedious but genuinely useful, because it gave me a concrete understanding of why FP-Growth avoids the expensive candidate generation and repeated database scanning that Apriori requires, and also where its own weaknesses (memory usage, complexity for sparse data) come from.

---

## Project 1 — Classification Using SVM, Random Forest, and Rule-Based Classifiers

This project applied three classification algorithms to the same student dataset across three tasks: predicting grade per department, grade from sleep hours, and stress level from total score. The most important lesson came not from the high-accuracy results (SVM at 96%, Decision Tree at 99.8% on grade classification) but from the stress prediction task, where all three models failed — SVM at 46%, Random Forest at 36%, Decision Tree at 10.5%. That failure is not a model problem; it reflects the reality that stress is influenced by factors far outside the dataset, and learning to read poor model performance as a signal about the problem rather than just the algorithm is a perspective shift this project helped me develop.

---

## Project 2 — Unsupervised Learning on Vehicle Emissions Data

This project applied K-Means and DBSCAN to cluster vehicles by fuel efficiency and engine characteristics, evaluated using Silhouette Score and Davies-Bouldin Index. K-Means produced clean, interpretable clusters — high, moderate, and low emission segments — with solid scores (Silhouette: 0.64–0.67), but what struck me more was what DBSCAN offered that K-Means could not: the ability to formally label outliers as noise rather than forcing every vehicle into the nearest centroid. In an environmental analysis context, those outlier vehicles are exactly what a policymaker would want to identify, which made me think more carefully about choosing algorithms based on what kind of output is actually useful, not just which one scores highest on a metric.

---

## Overall Reflection

Across all four tasks, the clearest through-line for me is that understanding *why* an algorithm works — or fails — matters more than knowing how to run it. Whether it was tracing the FP-Tree by hand, reading the stress prediction failure as a feature problem rather than a model problem, or recognizing that DBSCAN's outlier labels are more actionable than K-Means' forced assignments, the most valuable moments were the ones where a result made me question an assumption rather than confirm one. Data mining has a lot of moving parts — preprocessing, algorithm selection, evaluation metrics, and interpretation — and this course helped me see that each of those stages requires deliberate judgment, not just execution. Going forward, I want to keep building the habit of asking not just "what does the model output?" but "what does this output actually tell me about the problem?"
