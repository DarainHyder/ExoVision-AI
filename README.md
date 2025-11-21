# 🌌 ExoVision-AI  
**AI-Powered Exoplanet Detection System | NASA Space Apps Hackathon 2025**

> *“When the stars speak in data, we listen with algorithms.”*  
> _Bridging space exploration and machine learning to uncover distant worlds._

---

![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python)
![Flask](https://img.shields.io/badge/Flask-Framework-black?logo=flask)
![License](https://img.shields.io/badge/License-Apache_2.0-green?logo=open-source-initiative)
![Hackathon](https://img.shields.io/badge/NASA_Space_Apps-2025-orange?logo=nasa)
![ML](https://img.shields.io/badge/Machine_Learning-XGBoost%20%7C%20DecisionTree-red?logo=scikitlearn)

---

## 🚀 Overview

**ExoVision-AI** is a machine learning–driven web application that automatically classifies celestial objects as **Confirmed Exoplanets** or **Planetary Candidates** using NASA's open **K2 Planets and Candidates Catalog**.  
Developed by a team of passionate space and AI enthusiasts for the **NASA Space Apps Hackathon 2025**, this project bridges **data science** and **astrophysics** through real-time predictive modeling.

---

## 🌠 Key Highlights

-  **Intelligent ML Pipeline** – Preprocessing, feature engineering, and optimized Decision Tree + XGBoost models.  
-  **Interactive Web App (Flask)** – Upload datasets or manually enter parameters for instant classification.  
-  **Dynamic Visualizations** – Distribution charts, correlation heatmaps, ROC curves, and performance metrics.  
-  **End-to-End Reproducibility** – Ready-to-run environment with NASA data integration and trained models.  
-  **Hackathon-Optimized** – Lightweight, interpretable, and deployable in under 10 minutes.

---

## 🧬 System Architecture

```text
ExoVision-AI/
│
├── app/
│   ├── static/uploads/         # Uploaded CSVs
│   ├── templates/              # Front-end HTML pages
│   │   ├── index.html
│   │   ├── upload.html
│   │   ├── results.html
│   │   ├── manual_input.html
│   │   ├── manual_results.html
│   │   └── about.html
│   └── app.py                  # Flask web app
│
├── Dataset/
│   └── nasa-archive.csv        # NASA K2 dataset
│
├── Models/
│   ├── decision_tree_model.pkl
│   ├── decision_tree_pipeline.pkl
│   └── xgb_exoplanet_model.pkl
│
├── Notebook/
│   └── nasa-space-app.ipynb    # Full model training & evaluation notebook
│
├── requirements.txt
└── README.md
```

---

## 🧩 Machine Learning Pipeline

- **Preprocessing**
  - Missing-value imputation (`SimpleImputer`)
  - Feature engineering (stellar & orbital parameters)
  - One-hot encoding for categorical features

- **Modeling Strategy**
  - **Parallel Model Development**: Team divided into two sub-teams for comparative analysis
  - **Team A**: Trained XGBoost and Decision Tree models (selected for final implementation)
  - **Team B**: Trained LightGBM model (used for performance benchmarking)
  - 5-Fold **Stratified Cross-Validation**

- **Model Selection**
  - XGBoost selected for superior performance and interpretability
  - Decision Tree maintained as fallback for transparency and comparison
  - Final ensemble approach leverages both models for robust predictions

- **Evaluation Metrics**
  - Accuracy, Precision, Recall, F1-Score, ROC-AUC
  - Confusion Matrix & ROC Curve visualizations

> Example average CV Accuracy: `~99.0%`

---

## 🖥️ Web Application

Built using **Flask**, the interface allows two modes:

1. **📤 CSV Upload:**  
   Upload new K2 data to automatically classify planetary candidates.

2. **🧮 Manual Input:**  
   Enter stellar and planetary parameters via form input to get instant predictions.

**Features include:**
- Real-time visualization of dataset distributions  
- Heatmaps and ROC curves for interpretability  
- Side-by-side comparison of XGBoost vs Decision Tree predictions  

---

## 📸 Suggested Images

- `/app/static/architecture.png` → Model + Flask integration  
- `/app/static/app_preview.png` → Upload & results interface  
- `/app/static/visualizations.png` → Heatmap / ROC curve examples  

```markdown
![Architecture Overview](app/static/architecture.png)
![App Preview](app/static/app_preview.png)
![Visualizations](app/static/visualizations.png)
```

---

## ⚙️ Installation & Setup

```bash
# Clone repository
git clone https://github.com/c0llectorr/ExoVision-AI.git
cd ExoVision-AI

# Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate       # Linux/macOS
venv\Scripts\activate        # Windows

# Install dependencies
pip install -r requirements.txt
```

---

## ▶️ Run the Application

```bash
cd app
python app.py
```

Then open your browser and navigate to:
```
http://127.0.0.1:5000/
```

---

## 📈 Example Outputs

| Metric | Decision Tree | XGBoost |
|--------|----------------|----------|
| Accuracy | 0.99 | 0.993 |
| Precision | 0.98 | 0.99 |
| Recall | 0.99 | 0.99 |
| F1 Score | 0.985 | 0.992 |

---

## 🧑‍🚀 Team ExoVision

| Member | Role | Area |
|---------|------|------|
| Muhammad Ahmad | **Team Leader & Data Scientist** | Project Leadership, Data Strategy, Model Evaluation |
| Syed Darain Hyder Kazmi | ML Engineer | Model working and Training |
| Mansoob-e-Zahra | AI Expert  | Model Training & Deployment |
| Muhammad Ahsan Atiq | Backend Developer | Flask API Integration |
| Muhammad Mohsin | Frontend Developer | HTML Templates & UX |
| Ali Hassan | Research Lead | NASA Data & Validation |

> *A collaboration born from curiosity, teamwork, and love for the stars.*

---

## 📜 License

This project is licensed under the **Apache License 2.0** — free to use, modify, and distribute with attribution.

---

## 🌎 Acknowledgments

- **NASA Exoplanet Archive** – for the K2 Planets and Candidates Catalog  
  [Dataset Link](https://exoplanetarchive.ipac.caltech.edu/cgi-bin/TblView/nph-tblView?app=ExoTbls&config=k2pandc)
- **Scikit-learn**, **XGBoost**, **Flask**, **Seaborn** – core technology stack  
- **NASA Space Apps Hackathon 2025** – for the opportunity to explore the universe with AI  

---

### ⭐ If you like this project...
Give it a **star on GitHub** 🌟 and help us reach more open-source astronomers!
