# Manish Kallu — Data Science Portfolio

Public portfolio for **Manish R. Kallu**, M.S. Data Science, Willamette University.

## Live portfolio

**https://manishkallu01-wq.github.io/**

Featured capstone: **Forecasting and Explaining U.S. Unemployment Through Macroeconomic Indicators**  
Capstone page: **https://manishkallu01-wq.github.io/capstone.html**

## Capstone summary

The project evaluates whether publicly available U.S. macroeconomic indicators can forecast unemployment 3, 6, and 12 months ahead and separately examines which external indicators show the strongest historical lead–lag relationships with unemployment. The submitted analysis uses monthly data from **April 1956 through December 2025**, a final dataset of **837 rows × 40 columns**, **35 numeric predictors**, six forecasting algorithms, chronological validation, and persistence/unemployment-only baselines.

Selected test results:

| Horizon | Selected model | MAE | RMSE | R² |
|---|---|---:|---:|---:|
| 3 months | Ridge Regression | 0.349 | 1.020 | 0.720 |
| 6 months | Extra Trees | 0.725 | 1.277 | 0.563 |
| 12 months | Extra Trees | 1.195 | 1.729 | 0.205 |

Consumer sentiment showed the strongest overall external historical relationship with future unemployment, reaching Pearson **r = -0.496 at 12 months**, while the analysis also shows that these relationships can change across economic regimes.

Models were selected using the lowest validation RMSE, with validation MAE as a tiebreaker, before a single evaluation on the untouched chronological test period. Reproducibility uses `capstone_plus_final.xlsx` as the common processed input; all Python scripts, including the separate RQ2 correlation analysis, are available under `deliverables/M5-final` in the project repository.

## Final artifacts

- **Portfolio / project landing page:** https://manishkallu01-wq.github.io/capstone.html
- **Project report:** https://manishkallu01-wq.github.io/assets/Project%20Report.pdf
- **Final poster:** https://manishkallu01-wq.github.io/assets/M5%20poster%20Final.pdf
- **Project repository:** https://github.com/manishkallu01-wq/DATA510-Session-2

## Portfolio structure

- `index.qmd` — professional landing page
- `capstone.qmd` — featured capstone landing page, results, reproducibility, ethics, attribution, and artifacts
- `projects/capstone/index.qmd` — detailed capstone summary
- `projects.qmd` — projects listing
- `resume.qmd` — resume and downloadable PDF
- `about.qmd` — professional background and contact information
- `assets/Project Report.pdf` — capstone report
- `assets/M5 poster Final.pdf` — final capstone poster
- `assets/Resume.pdf` — current resume

## Publishing

The site is built with **Quarto** and deployed through GitHub Pages/GitHub Actions. Pushes to `main` trigger publication.

To preview the portfolio locally:

```bash
git clone https://github.com/manishkallu01-wq/manishkallu01-wq.github.io.git
cd manishkallu01-wq.github.io
quarto preview
```

## Responsible use and attribution

The capstone uses aggregate public economic data from the U.S. Bureau of Labor Statistics, Federal Reserve/FRED, U.S. Bureau of Economic Analysis, University of Michigan Surveys of Consumers, and National Bureau of Economic Research. Third-party data remain subject to their original providers' terms and attribution requirements. The analysis is intended for research, scenario planning, and comparative model evaluation; it should not be used as the sole basis for individual employment decisions, benefit allocation, or recession declarations.
