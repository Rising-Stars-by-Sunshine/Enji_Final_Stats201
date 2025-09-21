# Code Folder README

**Notebook:** `code_notebook.ipynb`

## What this notebook does
1. **Loads** the World Bank ESG dataset from Hugging Face (direct `hf://` CSV with a fallback to `datasets.load_dataset`).  
2. **Tidies** the data from wide (years as columns) to long format (`Country_Name`, `Year`, `Indicator_Code`, `Value`).  
3. **Inspects** missingness by indicator and by country (recent decade).  
4. **Visualizes** simple patterns:
   - Time series: Access to electricity (% of population) in the Arab World.  
   - Multi-country comparison: CO₂ per capita (United States, China, Arab World).  
   - Distribution: CO₂ per capita for the latest available year.  
   - (Optional) Correlation matrix across indicators for one country.  

## How to run
- **Google Colab:** Upload the `.ipynb`, run all cells.  
- **GitHub Codespaces:** Open the notebook and run. If `hf://` loading fails, install `datasets` with `pip` and rerun.

## Outputs
- Optional: a small tidy CSV sample is saved to `/mnt/data/esg_tidy_sample.csv` to demonstrate file export.

## Notes
- Plots use **matplotlib only** (per course constraints).  
- This EDA is **descriptive**, not causal. Handle governance indicators (e.g., `CC.EST`, `RL.EST`, `GE.EST`) carefully as they are perception-based standardized scores.
