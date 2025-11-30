# Well Data Analytics Project  
### Oil Well Sensor Anomaly Detection Using 3W Dataset

This repository contains an end-to-end anomaly detection workflow developed on the **3W Dataset**, a realistic multivariate time-series dataset collected from oil well sensors. The project focuses on identifying abnormal production patterns by leveraging both classical machine learning methods and deep learning-based time series models.

The work includes:

- Comprehensive exploratory data analysis (EDA) to understand data quality and challenges  
- Feature engineering tailored for multivariate time series data  
- Baseline anomaly detection models (Isolation Forest, Local Outlier Factor, PCA)  
- Ongoing development of an LSTM Autoencoder for advanced sequence-based anomaly detection  

---

## 🔍 Project Overview

Oil and gas production wells use multiple sensors located both downhole and on the surface to monitor important parameters like pressure, temperature, and gas lift flow. Detecting anomalies in these sensor readings early is essential to avoid production losses, equipment damage, and safety hazards.

The 3W Dataset reflects real-world conditions and challenges, such as missing data, constant sensor readings (frozen values), and imbalanced event classes. These characteristics make it a realistic and difficult benchmark for anomaly detection models.

This project aims to create a clear, flexible, and interpretable anomaly detection pipeline that handles the complexities of the 3W Dataset and can be extended in the future to support real-time monitoring.
---

## 📂 **Repository Structure**

```
project-root/
│
├── data/                     # Raw & processed data
├── notebooks/                # Jupyter workflow
│   ├── 1_exploratory_data_analysis.ipynb
│   ├── 2_feature_engineering_preprocessing.ipynb
│   ├── 3_anomaly_detection_baseline.ipynb
│   ├── 4_lstm_autoencoder_development.ipynb
│   └── 5_model_comparison_evaluation.ipynb
│
├── requirements.txt
├── README.md
```

---

## 🛠 Tech Stack & Methods

### 📚 Core Libraries

Robust data processing & visualization stack:

- **Pandas, NumPy** — efficient numerical and tabular data manipulation  
- **Matplotlib** — exploratory time-series visualization

### 🤖 Classical Machine Learning (Baseline Models)

Initial anomaly-detection models used for benchmarking:

- **Scikit-learn**  
  - Isolation Forest — tree-based anomaly scoring  
  - Local Outlier Factor (LOF) — density-based detection  
  - PCA Anomaly Score — reconstruction-error scoring in reduced dimensions

### 🧠 Deep Learning (Planned & Under Development)

Deep learning will be added as an extendable stage of the pipeline:

- **TensorFlow / Keras**  
- LSTM Autoencoder (Planned)  
  - Design phase completed  
  - Implementation & comparative evaluation in progress  
  - Will be integrated into `4_lstm_autoencoder_dev.ipynb`  
  - Final model will estimate anomalies via sequence reconstruction error

---

## 📊 **Current Project Status**

| Task                             | Status                   |
| -------------------------------- | ------------------------ |
| EDA                              | ✔ Completed              |
| Feature Engineering              | ✔ Completed              |
| Baseline Models   (IF, LOF, PCA) | ✔ Completed              |
| LSTM Autoencoder                 | 🚧 In Progress           |
| Model Comparisons                | 🚧 Planned               |

---

## 🚀 **Setup & Usage**

### 1️⃣ **Install Dependencies**

```bash
pip install -r requirements.txt
```

### 2️⃣ **Run the Workflow in Order**

Notebook Workflow Sequence

1. **exploratory_data_analysis.ipynb**
2. **feature_engineering.ipynb**
3. **anomaly_detection_baseline.ipynb**
4. **lstm_autoencoder_development.ipynb** (Work in progress)
5. **model_comparison_evaluation.ipynb** (in progress)

---
✍️ My Journey & Detailed Write-Up

I also published a detailed Medium article where I share my full journey of building this anomaly-detection pipeline — including motivations, challenges, decisions, and key learnings.

👉 Read the full story on Medium:
🔗 (link will be added soon)
---

## 🤝 Contributions

The project is built with a clean and extendable structure. Contributions, new models, or dataset extensions are welcome.
---

## 📬 Contact
For collaboration or suggestions, feel free to create an issue or open a pull request.
