# Enji_ProblemSet1_STATS201
# Clustering and Forecasting Country-Level ESG Trajectories (1990–2023)

## Abstract
This project constructs transparent Environmental, Social, and Governance (ESG) pillar scores from World Bank indicators (1990–2023) and applies machine learning to cluster countries by ESG profiles and forecast pillar trajectories to 2030. The goal is to provide a reproducible, FAIR/CARE-aligned data descriptor and baseline ML workflow for global sustainability benchmarking.

## System Configuration
- **Local:** Python 3.12, Jupyter Notebook, pandas, scikit-learn, statsmodels, matplotlib, seaborn  
- **Cloud:** Google Colab (GPU optional)  
- **Version Control:** Git + GitHub  
- **Reproducibility:** Deterministic seeds, requirements.txt to be added  

## Conceptual Flowchart
```mermaid
flowchart TD
    A[Background & Motivation] --> B[Research Question]
    B --> C[Data Preparation]
    C --> D[Composite ESG Pillars]
    D --> E[Clustering Countries]
    E --> F[Forecasting to 2030]
    F --> G[Anticipated Results]
    G --> H[Intellectual Merit & Practical Impacts]
