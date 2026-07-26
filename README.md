# AnDet: ML-Based Anomaly Detection of UEs in a Multi-cell B5G Mobile Network for Improved QoS

[![IEEE ICNC 2024](https://img.shields.io/badge/IEEE-ICNC%202024-blue)](https://doi.org/10.1109/ICNC59896.2024.10556379)
![Python](https://img.shields.io/badge/Python-3.10+-green)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Anomaly%20Detection-orange)
![XAI](https://img.shields.io/badge/Explainable-AI-red)

This repository contains the implementation, datasets, trained models, and evaluation scripts for the paper:

> **AnDet: ML-Based Anomaly Detection of UEs in a Multi-cell B5G Mobile Network for Improved QoS**
>
> **IEEE International Conference on Computing, Networking and Communications (ICNC 2024)**

📄 **Paper:** https://doi.org/10.1109/ICNC59896.2024.10556379 :contentReference[oaicite:0]{index=0}

---

# Overview

As Beyond 5G (B5G) mobile networks continue to support increasingly diverse applications, maintaining high Quality of Service (QoS) becomes a significant challenge. Network anomalies such as congestion, degraded radio conditions, and abnormal User Equipment (UE) behavior can severely affect throughput, latency, and service reliability.

**AnDet** is a Machine Learning-based anomaly detection framework designed for **SDN-enabled multi-cell B5G mobile networks**. The framework proactively identifies anomalous UE behavior using network KPIs and Explainable AI (XAI), enabling network operators to improve reliability and user experience. The reported implementation achieves **97.2% anomaly detection accuracy**. :contentReference[oaicite:1]{index=1}

---

# Key Features

- Machine Learning-based anomaly detection
- Multi-cell B5G network analysis
- User Equipment (UE) behavior monitoring
- SDN-enabled deployment
- Explainable AI (SHAP/LIME) integration
- Automated model training
- Performance evaluation
- Result visualization

---

# Repository Structure

```
.
├── data/                   # Training and testing datasets
├── preprocessing/          # Data preprocessing scripts
├── models/                 # ML models
├── training/               # Model training
├── inference/              # Prediction scripts
├── xai/                    # Explainable AI
├── notebooks/              # Jupyter notebooks
├── results/                # Experimental results
├── figures/                # Paper figures
├── requirements.txt
└── README.md
```

---

# System Architecture

```
                  +--------------------------------+
                  |      Multi-cell B5G Network    |
                  +--------------------------------+
                               |
          ---------------------------------------------
          |                  |                  |
      +-------+          +-------+          +-------+
      | gNB 1 |          | gNB 2 |   ...    | gNB N |
      +-------+          +-------+          +-------+
           \                  |                  /
            \                 |                 /
             \                |                /
              +------------------------------+
              |      User Equipments (UEs)   |
              +------------------------------+
                            |
                            v
                 Network KPI Collection
                            |
                            v
                 Feature Engineering
                            |
                            v
              Machine Learning Classifier
                            |
              +-------------+-------------+
              |                           |
         Normal UE                 Anomalous UE
              |                           |
              +-------------+-------------+
                            |
                            v
                 Explainable AI (XAI)
                            |
                            v
             QoS Improvement & SDN Actions
```

---

# Dataset Features

Typical network features include:

- RSRP
- RSRQ
- SINR
- CQI
- Throughput
- Packet Loss
- Latency
- Jitter
- UE Speed
- Cell Load
- Handover Count
- Signal Strength
- Resource Utilization

---

# Machine Learning Pipeline

```
Raw Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Feature Engineering
      │
      ▼
Feature Selection
      │
      ▼
Train/Test Split
      │
      ▼
Model Training
      │
      ▼
Anomaly Detection
      │
      ▼
Explainable AI
      │
      ▼
Performance Evaluation
```

---

# Technologies Used

- Python
- Scikit-learn
- Pandas
- NumPy
- XGBoost
- LightGBM
- CatBoost
- Matplotlib
- SHAP
- LIME
- Jupyter Notebook

---

# Installation

Clone the repository

```bash
git clone https://github.com/amarcrj/AnDet.git
cd AnDet
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# Training

```bash
python training/train.py
```

---

# Inference

```bash
python inference/predict.py
```

---

# Explainability

Generate SHAP explanations

```bash
python xai/shap_analysis.py
```

Generate LIME explanations

```bash
python xai/lime_analysis.py
```

---

# Performance Metrics

The framework evaluates:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix
- Detection Time
- False Positive Rate
- False Negative Rate

---

# Experimental Results

The proposed AnDet framework demonstrates:

- **97.2% anomaly detection accuracy**
- High Precision and Recall
- Low False Positive Rate
- Fast inference suitable for near real-time deployment
- Improved QoS through proactive anomaly detection :contentReference[oaicite:2]{index=2}

---

# Applications

- B5G Mobile Networks
- SDN-enabled Cellular Networks
- Network Monitoring
- Self-Organizing Networks (SON)
- Intelligent Network Management
- QoS Optimization
- Telecom Analytics
- AI-driven Network Automation

---

# Citation

If you use this repository in your research, please cite:

```bibtex
@inproceedings{sinha2024andet,
  author={Amar Sinha and Anmol Agrawal and Sandip Roy and
          Venkanna Uduthalapally and Debanjan Das and
          Rajarshi Mahapatra and Sachin Shetty},
  title={AnDet: ML-Based Anomaly Detection of UEs in a Multi-cell B5G Mobile Network for Improved QoS},
  booktitle={IEEE International Conference on Computing, Networking and Communications (ICNC)},
  year={2024},
  pages={500--505},
  doi={10.1109/ICNC59896.2024.10556379}
}
```

---

# Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Submit a Pull Request

---

# License

This project is licensed under the MIT License.

---

# Contact

**Amar Sinha**

🌐 Website: https://www.amarsinha.in

💻 GitHub: https://github.com/amarcrj

📧 Email: amaraec1720@gmail.com

---

# Acknowledgements

- IEEE ICNC 2024
- IIIT Naya Raipur
- Old Dominion University
- Scikit-learn Community
- SHAP
- LIME

---

⭐ If you find this repository useful, please consider giving it a **Star**.
