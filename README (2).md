# Evaluating Weighted Conformal Prediction With Estimated Density Ratios

Submission package for the *Journal of Machine Learning Research*.

**Authors:** Kuntapalli Vasist, Polu Ruthvik Reddy (Independent Researchers, Hyderabad, Telangana 500047, India)
**Contact:** learningwithvashistkuntapalli@gmail.com, ruthvik1029@gmail.com
**Status:** Submission draft, October 2026 (no volume, pages or editor assigned)

## Contents

| File | Description |
|---|---|
| `Weighted_CP_Estimated_Density_Ratios_JMLR_updated.pdf` | Manuscript (16 pages, JMLR format) |
| `Cover_Letter.pdf` | Cover letter to the editors |
| `README.md` | This file |

## Summary

Controlled study of weighted split conformal prediction (LAC scores, alpha = 0.1) when the
test/calibration likelihood ratio is estimated rather than known. Ten methods are compared:
unweighted split CP, oracle weights, domain-classifier weights (LR-W), KLIEP, uLSIF, RuLSIF,
nexCP, ESS-adaptive tempering, and two ACI variants.

- **Data:** 21 Kaggle tabular classification data sets (14 binary, 7 multiclass), listed in Appendix A
- **Setup:** 3 base learners (logistic regression, histogram gradient boosting, MLP), 5 exponential-tilt strengths (gamma = 0 to 2), 10 seeds = 31,500 runs
- **Metrics:** coverage, absolute gap to 0.90, set size, under-coverage rate, ESS ratio, weight error
- **Statistics:** data-set-level averaging, Friedman test, paired Wilcoxon tests (uncorrected, descriptive)

## Reproducibility

Implementation details (estimator settings, bandwidth grids, seeds 0 to 9, model hyperparameters)
are in Appendix B. Code and raw results for all runs are available from the authors on
reasonable request. Data sets are public on Kaggle (handles in Table 5).

## Declarations

- **Funding:** none
- **Generative AI:** Claude (Anthropic) was used as a writing and editing assistant; the authors reviewed all output and take full responsibility for the content
- **License:** CC-BY 4.0

## Notes

- Front-matter metadata (volume, year, pages, dates, editor) is intentionally omitted; it is assigned by JMLR at acceptance.
- The final camera-ready version should be compiled from LaTeX with the official `jmlr2e.sty`.
