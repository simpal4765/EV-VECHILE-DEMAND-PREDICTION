# ⚡ EV Charging Demand Prediction & Forecasting Dashboard

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python\&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-1.x-red?logo=streamlit\&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-orange?logo=scikitlearn\&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![GitHub Stars](https://img.shields.io/github/stars/tanishka234/EV_VEHICLE_DEMAND_PREDICTION?style=social)

*An AI-powered interactive dashboard that forecasts Electric Vehicle (EV) adoption trends at the county level using machine learning. Built with Streamlit and scikit-learn for planners, researchers, and smart mobility solutions.*

[🚀 Quick Start](#-quick-start) • [📖 Features](#-features--use-cases) • [🧠 ML Pipeline](#-machine-learning-pipeline) • [📊 Deployment](#-deployment-options) • [🤝 Contributing](#-contributing)

</div>

---

## 📑 Table of Contents

* [🌟 Overview](#-overview)
* [🚀 Quick Start](#-quick-start)
* [✨ Features & Use Cases](#-features--use-cases)
* [📊 Dataset](#-dataset)
* [🧠 Machine Learning Pipeline](#-machine-learning-pipeline)
* [🛠️ Technical Details](#-technical-details)
* [📅 Setup & Installation](#-setup--usage)
* [🌚 Forecast Examples](#-example-forecasts)
* [📊 Visualization Outputs](#-visualization-outputs)
* [🚀 Deployment Options](#-deployment-options)
* [🤝 Contributing](#-contributing)
* [📄 License](#-license)
* [📧 Contact](#-contact)

---

## 🌟 Overview

This AI-powered tool forecasts **EV demand across counties** in Washington State using machine learning and displays results in a user-friendly dashboard.

**Capabilities:**

* 🔮 Predicts 36-month EV growth trends
* 📈 Helps city planners optimize infrastructure
* 🖥️ Streamlit-based dashboard for visualization and interaction

---
## DEMO Screen Shots
<img width="894" height="795" alt="Screenshot 2025-08-02 211551" src="https://github.com/user-attachments/assets/9abbb866-e9d3-492d-a726-3254f5b81569" />
<img width="828" height="709" alt="Screenshot 2025-08-02 211617" src="https://github.com/user-attachments/assets/2a6164ed-fcfd-430f-afbb-9e27989e91f8" />
<img width="830" height="567" alt="Screenshot 2025-08-02 211627" src="https://github.com/user-attachments/assets/135d194a-28fd-40af-9c55-c98ac348fc28" />



---

## 🚀 Quick Start

### Prerequisites

* Python 3.8+
* pip installed

### Installation

```bash
# Clone the repository
git clone https://github.com/tanishka234/EV_VEHICLE_DEMAND_PREDICTION.git
cd EV_VEHICLE_DEMAND_PREDICTION

# Install dependencies
pip install -r requirements.txt

# Run the application
streamlit run app.py
```

🌐 App URL: [http://localhost:8501](http://localhost:8501)

---

## ✨ Features & Use Cases

| Feature                | Description                              |
| ---------------------- | ---------------------------------------- |
| 📅 3-Year Forecast     | Predict EV adoption for each county      |
| 📊 Visual Dashboard    | Interactive Streamlit UI                 |
| 🔄 Compare Counties    | Analyze demand side-by-side              |
| 🏢 Planning Tool       | Guide infrastructure investment          |
| ⚡ Time Series Modeling | ML-based forecasting using Random Forest |

---

## 📊 Dataset

**Source:** [Washington State EV Population](https://catalog.data.gov/dataset/electric-vehicle-population-data)

**Input CSV:** `Electric_Vehicle_Population_By_County.csv`  → `preprocessed_ev_data.csv`

| Column          | Description                     |
| --------------- | ------------------------------- |
| County          | Washington counties             |
| Model Year      | Registration year               |
| EV Type         | Battery/Plug-in Hybrid          |
| Forecast Target | Vehicle counts by county & year |

---

## 🧠 Machine Learning Pipeline

**Model:** `RandomForestRegressor` (via scikit-learn)

```
Input Features: County, Year, EV type
↓
Data Preprocessing: Encoding + Aggregation
↓
Model Training: EV_Adoption_Forecasting.ipynb
↓
Model Output: EV growth for next 36 months
↓
Saved Model: forecasting_ev_model.pkl
```

---

## 🛠️ Technical Details

| Component        | Tool/Library Used          |
| ---------------- | -------------------------- |
| ML Model         | scikit-learn               |
| Dashboard        | Streamlit                  |
| Deployment       | Heroku / Streamlit Cloud   |
| Environment Mgmt | requirements.txt, Procfile |

---

## 📅 Setup & Usage

### Step 1: Clone & Install

```bash
git clone https://github.com/tanishka234/EV_VEHICLE_DEMAND_PREDICTION.git
cd EV_VEHICLE_DEMAND_PREDICTION
pip install -r requirements.txt
```

### Step 2: Launch Dashboard

```bash
streamlit run app.py
```

> Open [http://localhost:8501](http://localhost:8501) in your browser

---

## 🌚 Example Forecasts

### 1. **King County**

* 2025: \~42,000 EVs
* 2026: \~51,000 EVs
* 2027: \~61,000 EVs

### 2. **Spokane County**

* 2025: \~5,600 EVs
* 2026: \~7,000 EVs
* 2027: \~8,700 EVs

---

## 📊 Visualization Outputs

* 📈 Line Graph: Growth per county
* 📊 Bar Chart: Annual comparisons
* 🥧 Pie Chart: EV Type breakdown

---

## 🚀 Deployment Options

| Platform          | Instructions                |
| ----------------- | --------------------------- |
| ✅ Localhost       | `streamlit run app.py`      |
| ✅ Streamlit Cloud | Connect repo & deploy       |
| ✅ Heroku          | Add `Procfile`, auto-deploy |
| 🔜 Docker         | (Optional, not included)    |

---

## 🤝 Contributing

### 🚀 How to Contribute

1. Fork this repository
2. Create a branch: `feature/your-feature`
3. Commit your changes
4. Push and submit a Pull Request

### 🧠 Development Ideas

* Add forecasting by fuel type
* Integrate population & income features
* Add Prophet/XGBoost model option
* Enhance UI with charts or filters

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## 📧 Contact

**Author:** Tanishka Jain
**GitHub:** [@tanishka234](https://github.com/tanishka234)

> ✨ Empowering sustainable mobility with data and machine learning.


