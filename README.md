# Electoral Stability Analysis: FPTP vs PR

This repository contains the code and data for the paper:  
**"A Machine Learning Based Analysis of Electoral Stability using Historical Election Data"**  
– comparing the UK (First-Past-the-Post) and Bulgaria (Proportional Representation).

## 📁 Contents
- `data/` – Processed election datasets (UK 1970–2024, Bulgaria 1991–2024)
- `notebooks/` – Jupyter notebooks for preprocessing, clustering, and regression
- `src/` – Python scripts for metric calculation (responsiveness, stability) and models
- `results/` – Outputs (cluster tables, regression coefficients, plots)

## 🔧 Requirements
- Python 3.8+
- pandas, numpy, scikit-learn, statsmodels, matplotlib

Install with:
```bash
pip install -r requirements.txt
🚀 Quick Start
Clone the repo

Run python src/preprocess.py to clean and align datasets

Run python src/analysis.py to reproduce regression and clustering results

📊 Key Metrics
Responsiveness = ΔSeat Share / ΔVote Share (party-level, then weighted avg)

Stability = Years to next election

📈 Main Findings
UK (FPTP): Higher responsiveness → greater stability (coeff +0.08)

Bulgaria (PR): Extreme responsiveness → lower stability (cluster avg 0.38 years)
