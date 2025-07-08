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

📁/notebooks

└── FYP_Final_Ver.ipynb # Main code (classification + simulation)

📁/visuals

└── graphs/ # Network visualizations & metrics

└── confusion_matrices/ # Classification model outputs

📁/docs

└── Chan Kin Lok Gerald Dissertation.pdf

└── Viva_Presentation.pptx

📁/data

└── processed_data.csv # Cleaned merged dataset (fake/real labels)


---

## 📊 Key Results

| Model                  | Accuracy | Precision | Recall | F1-score |
|------------------------|----------|-----------|--------|----------|
| TF-IDF + Logistic Reg. | 84.0%    | 82%       | 45%    | 0.58     |
| BERT                   | 84.4%    | 82%       | 66%    | 0.68     |

- BA networks showed faster and broader spread of misinformation  
- Nodes with high betweenness & eigenvector centrality were critical to spread  
- Louvain algorithm revealed community structures (echo chambers)

---

## 📌 Future Work

- Add node weights based on classifier confidence scores  
- Extend sensitivity analysis to recovery rate and initial infection size  
- Compare synthetic networks with real Twitter graph data  
- Test targeted interventions on central nodes and communities

---

## 📎 Related Files

-📘 [Dissertation (PDF)](docs/Chan%20Kin%20Lok%20Gerald%20Dissertation.pdf)  
-🎓 [Viva Presentation (PPTX)](docs/Chan%20Kin%20Lok%20Gerald%20Viva.pptx)  
-🧪 [Code Notebook](notebooks/Chan%20Kin%20Lok%20Gerald%20Dissertation%20Code.ipynb)

---

## 👤 Author

**Gerald Chan Kin Lok**  
MSc Data Science, University of Sunderland  
📫 Contact: culerty516@gmail.com

---

## 📄 License

This project is available for academic and non-commercial use. Please cite or credit the repository if you use or reference any part of this work.

---
