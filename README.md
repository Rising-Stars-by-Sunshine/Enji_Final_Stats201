# 🟢 Analyzing and Forecasting Mongolia’s Renewable-Energy Trajectory

**Author:** Enkhjin Purevsukh  
**Course:** STATS 201 – Machine Learning for Social Science  
**Instructor:** Prof. Luyao Zhang, Duke Kunshan University (Autumn 2025)

---

## 📘 Abstract
This project evaluates Mongolia’s renewable-energy transition under two major policy interventions—the 2015 **Feed-in Tariff (FIT) Law** and the 2021 **New Recovery Policy (NRP)**—using the World Bank’s ESG dataset (1990–2021).  
Machine-learning and statistical models, including interrupted-time-series regression, exponential-smoothing (ETS) forecasting, and vector-autoregression, are applied to analyze policy effects on renewable-energy consumption and energy intensity.  

Results show that while renewable capacity has expanded to nearly 18 percent of installed power, actual renewable consumption has stagnated. Efficiency improvements continue but remain largely coal-based. The findings suggest that stronger grid investment, competitive renewable-energy auctions, and cross-sectoral integration are necessary to meet Mongolia’s 2030 sustainability goals.

---

## 📂 Repository Structure
├── code/
│ ├── explanation/ # NLP + network analysis (sentiment, TF-IDF, co-occurrence)
│ └── prediction/ # ETS + AutoGluon forecasting notebooks
│
├── data/
│ ├── raw/ # Original World Bank ESG indicators
│ ├── data_dictionary.csv # Variable names and descriptions
│ └── README.md # Data provenance and preprocessing notes
│
├── visualizations/ # Forecast plots, trend lines, network graphs
│
├── docs/
│ ├── STATS201_Final_Report.pdf
│ ├── Poster.pdf
│
└── README.md 

---

## 📊 Navigation Guide

| Task | Folder | Notebook or File |
|------|---------|------------------|
| **1. Data preprocessing** | `data/` | `data` |
| **2. ML for Explanation** | `code/explanation/` | `MLExplanation.ipynb` |
| **3. ML for Prediction** | `code/prediction/` | `Enji_Stats201_Final.ipynb` |
| **4. Visualization outputs** | `visualizations/` | PNG / SVG figures used in report |
| **5. Report and Poster** | `docs/` | Final PDFs and supplementary files |

To reproduce results:
1. Clone the repository.  
2. Open the notebooks in Jupyter or Google Colab.  
3. Run cells sequentially; outputs will match figures in the report.  

---

## 🧠 Method Overview
- **Dataset:** World Bank Global Environment, Social and Governance Indicators (1990–2021)  
- **Key variables:**  
  - `EG.FEC.RNEW.ZS` – Renewable Energy Consumption (% of total final energy)  
  - `EG.EGY.PRIM.PP.KD` – Energy Intensity (MJ per $2017 PPP GDP)  
- **Models used:**  
  - Interrupted Time Series (ITS) regression for policy evaluation  
  - Exponential Smoothing (ETS) forecasting to 2030  
  - Vector Autoregression (VAR) and Gradient Boosting for interdependence testing  

---

## 🙏 Acknowledgments
Guidance and mentorship from **Prof. Luyao Zhang** made this project possible. I thank my classmates for valuable peer feedback and the open-data communities whose resources supported reproducibility. Analytical tools include **AutoGluon**, **statsmodels**, **networkx**, and **matplotlib**.  
This repository adheres to **FAIR** and **CARE** data-governance principles to ensure that the work remains transparent, reusable, and ethically grounded.

---

## ⚖️ Disclaimer
> This repository supports the final research proposal submitted to **STATS 201: Machine Learning for Social Science**, instructed by **Prof. Luyao Zhang** at **Duke Kunshan University** in Autumn 2025.

---

## 🧩 Citation
If referencing this repository, please cite as:  
GitHub: [https://github.com/Rising-Stars-by-Sunshine/Enji_ProblemSet1_STATS201](https://github.com/Rising-Stars-by-Sunshine/Enji_ProblemSet1_STATS201)

---

© 2025 Enkhjin Purevsukh | Duke Kunshan University | Open Research License (CC-BY-4.0)




