# Enji_ProblemSet1_STATS201
# Problem Set 2 – Revised Proposal

## Acknowledgment
I am grateful to Professor **Luyao Zhang** and my peer reviewer, **Undran Enkhbaatar**, for thoughtful and constructive feedback on Problem Set 1. Their comments helped me sharpen the research question, justify methodological choices with credible sources, and improve the coherence of the narrative.

---

## Point-by-Point Response to Feedback
- **Professor Zhang**: Requested clearer definitions, novelty statement, reproducibility, and reflexivity.  
  ✅ Added method definitions, cited best practices, clarified contribution, documented imputation/weighting, and included uncertainty bands.  

- **Peer Reviewer (Undran)**: Asked why equal vs PCA weighting, how imputation bias is handled, and requested figures.  
  ✅ Explained equal vs PCA rationale, tested both imputation methods, and committed to visualizations (time-series plots, heatmap, forecasts).
  
flowchart TD
  A[Background & Motivation]
  B[Research Question]
  C[Indicators]
  D[Methodology]
  D1[Data & Preprocessing]
  D2[Mini-Index Construction]
  D3[Forecasting to 2030]
  E[Anticipated Results & Visualizations]
  F[Ethical & Practical Considerations]
  G[Policy Implications: Lessons from China]

  A --> B
  B --> C
  C -->|Renewable Share + Energy Intensity| D
  D --> D1
  D1 --> D2
  D2 --> D3
  D3 --> E
  E --> F
  F --> G

  %% cross-links / annotations
  A -.->|Comparative context| B
  D2 -.->|Equal vs PCA Weights| E
  D3 -.->|ARIMA / ETS / DirectTabular| E


---

## Background and Motivation
- Composite indicators are sensitive to **scaling, imputation, weighting** → need transparency (OECD 2008).  
- ESG research shows divergence across methodologies (Berg, Kölbel, and Rigobon 2022).  
- **Mongolia**: highly energy-intensive, lagging renewable uptake, but 2030 policy targets for efficiency & diversification.  
- **China**: benchmark case of successful energy intensity reduction and renewable scale-up (IEA 2020).  

---

## Research Question
**How have Mongolia’s renewable energy share and energy intensity evolved since 1990, how sensitive are conclusions to alternative imputation and weighting choices in a simple mini-index, and what lessons from China’s experience could inform Mongolia’s path to meeting its 2030 energy policy goals?**

---

## Literature Review
- Composite indicators: need transparency, sensitivity checks (OECD 2008).  
- ESG ratings divergence motivates robustness (Berg et al. 2022).  
- EPI audits show aggregation/weighting can reshape narratives (Wendling et al. 2020).  
- IEA: China’s efficiency programs → benchmark for Mongolia.  

---

## Indicators
- **Renewable Energy Share (EG.FEC.RNEW.ZS)** – measures diversification from coal.  
- **Energy Intensity of GDP (EG.EGY.PRIM.PP.KD)** – SDG 7.3 efficiency indicator.  
- Both are **World Bank** indicators → reproducible and comparable.  

---

## Methodology
1. **Data & Preprocessing**  
   - World Bank (1990–2021).  
   - Imputation: forward-fill for short gaps, mean for long gaps.  
   - Standardized to z-scores.  

2. **Mini-Index Construction**  
   - Equal weights (transparent baseline).  
   - PCA weights (variance-driven alternative).  
   - Compare robustness across imputation + weighting choices.  

3. **Forecasting (to 2030)**  
   Models applied separately to each indicator:  
   - **ARIMA** (Box–Jenkins).  
   - **Random Forest** (nonlinear).  
   - **AutoGluon-Tabular** (AutoML ensemble).  
   - Metrics: RMSE & MAE.  
   - Forecasts: 2026–2030 with prediction intervals.  

---

## Anticipated Results & Visualizations
- Energy intensity: gradual decline but still high.  
- Renewable share: modest growth from low base.  
- Index differences: slope/level shifts highlight sensitivity.  

**Figures planned:**  
- Time-series plots (1990–latest).  
- Sensitivity heatmap (weighting vs imputation).  
- Forecast plots (2026–2030 with uncertainty bands).  

---

## Ethical & Practical Considerations
- Descriptive (not causal).  
- Transparent about assumptions & uncertainty.  
- FAIR: findable & accessible, but limited interoperability.  
- CARE: avoid deficit framing, acknowledge governance biases.  

---

## References
- Berg, Florian, Julian F. Kölbel, and Roberto Rigobon. 2022. *Aggregate Confusion: The Divergence of ESG Ratings.* Review of Finance 26 (6): 1315–44.  
- Box, George E. P., Gwilym M. Jenkins, and Gregory C. Reinsel. 2015. *Time Series Analysis: Forecasting and Control.* 5th ed.  
- Breiman, Leo. 2001. “Random Forests.” *Machine Learning* 45 (1): 5–32.  
- Erickson, Nick, et al. 2020. *AutoGluon-Tabular: Robust and Accurate AutoML for Structured Data.* arXiv:2003.06505.  
- IEA. 2020. *Energy Efficiency 2020.* Paris: IEA.  
- Jolliffe, Ian T., and Jorge Cadima. 2016. “Principal Component Analysis: A Review and Recent Developments.” *Philosophical Transactions of the Royal Society A* 374.  
- OECD. 2008. *Handbook on Constructing Composite Indicators.* Paris: OECD.  
- Wendling, Z.A., et al. 2020. *2020 Environmental Performance Index.* Yale Center for Environmental Law & Policy.  

---


## System Configuration
- **Local:** Python 3.12, Jupyter Notebook, pandas, scikit-learn, statsmodels, matplotlib, seaborn  
- **Cloud:** Google Colab (GPU optional)  
- **Version Control:** Git + GitHub  
- **Reproducibility:** Deterministic seeds, requirements.txt to be added



