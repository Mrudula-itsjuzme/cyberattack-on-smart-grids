# Cyberattack Detection on Smart Grids

An intrusion-detection and analysis pipeline for smart-grid communication traffic, focused on IEC 60870-5-104 / IEC-104 network data, supervised attack classification, feature analysis, and model benchmarking.

This repository represents the engineering side of a research-oriented project on securing critical power-grid communication systems.

---

## Problem statement

Smart grids depend on communication protocols that connect substations, control centers, and field devices. If malicious traffic is not detected early, attacks can affect grid monitoring, control decisions, and operational reliability.

This project builds a machine-learning pipeline to classify normal and attack traffic patterns from smart-grid communication data.

---

## What this project covers

- IEC-104 smart-grid traffic analysis
- preprocessing and feature engineering
- supervised attack detection
- baseline model comparison
- ensemble evaluation
- confusion-matrix and metric generation
- publication-oriented plots and result artifacts

---

## Pipeline

```text
Raw IEC-104 Traffic / Logs
          ↓
Preprocessing + Cleaning
          ↓
Feature Engineering
          ↓
Model Training
          ↓
Evaluation + Explainability
          ↓
Result Tables, Plots, and Reports
```

---

## Model benchmarks

| Model | Accuracy | Notes |
|---|---:|---|
| Decision Tree | 91.16% | Fast and interpretable baseline |
| Random Forest | 91.66% | Strong classical ML baseline |
| SVM | 76.65% | Sensitive to feature scaling and dimensionality |
| KNN | 76.65% | Simple but memory-heavy for larger traffic data |
| Ensemble | 91.81% | Best overall benchmark in this repo |

---

## Repository structure

```text
cyberattack-on-smart-grids/
├── ids.py / ids1.py        # IDS model training and analysis scripts
├── honey*.py               # security and honeypot-related experiments
├── results/                # generated outputs and analysis results
├── IEEE_Plots/             # publication-style visualizations
├── Graphs/                 # exploratory data-analysis plots
├── docs/                   # architecture notes and screenshots
└── README.md
```

---

## How to run

1. Clone the repository.

```bash
git clone https://github.com/Mrudula-itsjuzme/cyberattack-on-smart-grids.git
cd cyberattack-on-smart-grids
```

2. Install the required Python libraries used by the scripts.

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

3. Update dataset paths inside the relevant scripts.

4. Run a training or evaluation script.

```bash
python ids.py
```

5. Check generated metrics, plots, and outputs under the result folders.

---

## Paper context

This work is connected to a smart-grid cybersecurity research direction and references the IEEE paper available here:

- https://ieeexplore.ieee.org/document/11083563

---

## Tech stack

- Python
- Pandas / NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Classical ML models
- Smart-grid / IEC-104 traffic analysis

---

## Current status

Research/prototype implementation. The repository contains multiple experiment scripts and result artifacts. The next improvement would be consolidating the scripts into a single configurable training pipeline with cleaner dataset-path management.

---

## Author

Built by [Pedamallu Sai Mrudula](https://github.com/Mrudula-itsjuzme) as part of an applied AI, cybersecurity, and smart-grid analytics portfolio.
