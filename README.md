# 🏛️ TaxGuard-TN: Deterministic Compliance Intelligence System

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Framework](https://img.shields.io/badge/Architecture-Multi--Agent-orange)](https://github.com/lokesh-poreddy/NLP_MODEL)
[![Deployment](https://img.shields.io/badge/Target-Tamil_Nadu_Revenue_Dept-green)](https://www.tn.gov.in/dept/24)
[![License](https://img.shields.io/badge/License-Proprietary-red)](LICENSE)

> **TaxGuard-TN** is a production-grade, hybrid AI framework designed for the **Tamil Nadu Revenue & Disaster Management Department**. It combines Neuro-Symbolic AI, Multi-Agent Orchestration, and Bilingual NLP to detect financial fraud and tax evasion with deterministic traceability.

---

## 📌 Executive Summary

Modern tax evasion schemes are often hidden within complex narratives and multi-layered financial networks. **TaxGuard-TN** moves beyond traditional black-box machine learning by implementing a **Neuro-Symbolic architecture**. It doesn't just predict risk; it explains it through statutory legal rules and structured intermediate representations (IR).

### 🚀 Key Value Propositions
- **Bilingual Intelligence**: Native support for **Tamil (தமிழ்)** and English document processing.
- **Explainable AI (XAI)**: Every risk score is backed by a logical trace, meeting government transparency standards.
- **Hybrid Engine**: Fuses semantic NLP signals with hard-coded legal overrides and graph-based network analysis.
- **Deterministic Reliability**: Guaranteed reproducibility for audit purposes via locked-seed execution.

---

## 🧠 System Architecture: The Multi-Agent Orchestrator

The system operates through five specialized agents, each providing a unique risk signal ($S$). These signals are fused into a composite score, with the **Legal Agent** acting as a hard override.

| Agent | Signal | Role | Core Technology |
| :--- | :--- | :--- | :--- |
| **Narrator (NLP)** | $S_{sem}$ | Semantic Risk Detection | MuRIL (Indic-BERT), Cosine Similarity |
| **Accountant (Fin)** | $S_{num}$ | Financial Anomaly | Forensic Analytics, Statistical Profiling |
| **Graph (Network)**| $S_{net}$ | Contagion Analysis | NetworkX, Graph Neural Networks (PyG) |
| **Skeptic (Adv)** | $S_{skeptic}$ | Collusion Detection | Adversarial Pattern Matching |
| **Legal (Logic)** | $S_{legal}$ | **Hard Override** | PyDatalog, Symbolic Logic Engine |

---

## 🛠️ Technical Pillars

### 1. The IR (Intermediate Representation) Layer
The system's strongest differentiator. It converts messy free-text from OCR into structured **TaxFactIR** (JSON) using Pydantic validation. This ensures that the logic engine receives "clean" facts, preventing "garbage-in, garbage-out" scenarios.

### 2. Bilingual OCR & NLP
- **Layout-Aware OCR**: Uses Tesseract with custom configurations for Indian invoice formats.
- **Indic NLP**: Leverages `google/muril-base-cased` to handle Tamil Unicode (U+0B80–U+0BFF) and English seamlessly within the same embedding space.

### 3. Symbolic Logic Engine
Statutory rules (e.g., "Offshore evasion under Section X") are defined as logical predicates. If a violation is detected, the **Legal Agent** pins the risk score to 0.99, overriding all probabilistic signals.

---

## 📁 Project Structure

```bash
NLP_Model/
├── 📂 NLP_MODEL_FULL_CODES/   # Core implementation and entry points
│   ├── main_model.py         # Main pipeline execution script
│   ├── NLP_MODEL.pdf         # Comprehensive system documentation
│   ├── NLP_REPORT.pdf        # Final project report
│   └── 📊 Functional_test.xlsx # Test case templates
├── 📂 NLP_V2/                 # Output artifacts and visualizations
│   ├── risk_landscape.html   # Interactive 3D risk visualization
│   ├── network_graph.png     # Entity relationship visualization
│   └── 📄 master_dataset.csv  # Final audit registry with risk scores
├── 📂 TN_Tax_Dataset/         # Processed datasets for Tamil Nadu region
├── 📓 TaxGuard_TN_Kaggle_Notebook.ipynb  # Production-ready Kaggle workflow
└── 📓 TaxGuard_TN_Dataset_Creation_Notebook.ipynb # Synthetic data generation engine
```

---

## ▶️ Getting Started

### Prerequisites
- Python 3.8+
- Tesseract OCR (installed on system)
- GPU (Optional but recommended for MuRIL embeddings)

### Installation
```bash
git clone https://github.com/lokesh-poreddy/NLP_MODEL.git
pip install -r requirements.txt
```

### Running the Pipeline
The entire pipeline can be triggered via the main script:
```bash
python NLP_MODEL_FULL_CODES/main_model.py
```
*Note: Ensure your dataset paths are configured in `system_config.json`.*

---

## 📊 Visualizing Results

TaxGuard-TN generates a suite of interactive and static reports located in the `NLP_V2/` directory:
- **Risk Heatmaps**: Identify geographical clusters of high-risk entities.
- **Temporal Anomalies**: Track revenue shifts and tax credit spikes over a 30-year trend.
- **Explainable Audit Registry**: A CSV export detailing the "Why" behind every high-risk flag.

---

## 👨‍💻 Author & Acknowledgements

**Author**: Poreddy Lokesh Reddy  
**Contact**: [GitHub Profile](https://github.com/lokesh-poreddy)

Special thanks to the open-source community for the `Transformers`, `PyG`, and `pyDatalog` libraries that made this hybrid system possible.

---
*© 2026 TaxGuard-TN. Developed for academic and government research purposes.*
