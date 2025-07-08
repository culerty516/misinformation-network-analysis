# 📘 Analysing the Spread of Misinformation in Social Networks  
*Using Random Graph Models, SIR Simulation, and Classification Models*

This repository contains the complete code, data pipeline, and simulation outputs for my MSc Data Science dissertation, titled:

**“Analysing the Spread of Misinformation in Social Networks Using Random Graph Models: Predictive Modelling and Mitigation Strategies for Enhancing Network Resilience.”**

---

## 📌 Overview

This project investigates how fake news spreads across synthetic social networks and how machine learning and graph theory can be used to detect and mitigate its spread. It integrates natural language processing (NLP), network modeling, and epidemic simulation techniques.

---

## 🧠 Key Features

- **Fake News Detection**  
  - Built two classifiers using the FakeNewsNet dataset:
    - TF-IDF + Logistic Regression (baseline)
    - Fine-tuned BERT (transformer-based)
  - BERT achieved more balanced performance across fake and real classes

- **Synthetic Network Modeling**  
  - Constructed Barabási–Albert (BA) and Erdős–Rényi (ER) networks
  - Assigned node attributes from classification outputs

- **Misinformation Spread Simulation (SIR Model)**  
  - Simulated infection spread over BA and ER networks
  - Performed sensitivity analysis over infection probabilities

- **Network Analysis**  
  - Computed centrality metrics: betweenness, closeness, eigenvector
  - Detected communities using the Louvain algorithm
  - Identified high-risk nodes for targeted intervention

---

## 📂 Repository Structure

