# Tisya Sharma

I'm a senior Data Science and Biology student at Northeastern University, graduating in December 2026. This summer, I've been working as an AI Engineering Intern at the Institute for Protein Innovation.

I'm especially interested in machine learning, data science, and building reliable systems that turn complex, real-world data into useful insights and tools.

### A Little More About Me

Music and food are two of my favorite things. I love going to concerts, discovering new music, and making or trying new food with my friends. I’m also always looking forward to the next opportunity to travel and explore somewhere new!

## Projects

### Machine Learning Systems

#### **Flight Delay Forecasting** | [Repo](https://github.com/tisyasharma/flight-delay-forecasting) | [Live Demo](https://tisyasharma.github.io/flight-delay-forecasting/)

Live route-level forecasting system that publishes daily seven-day forecasts of average arrival delay, with calibrated 80% prediction intervals, for the 50 busiest U.S. routes.

- Built a recursive **LightGBM quantile forecasting** pipeline that bridges the five-to-ten-week lag in published flight outcomes by rolling predictions forward with current weather data; validated serving depths through 90 recursive days
- Across four half-year walk-forward folds, the evaluated q50 model achieved **10.80-minute MAE**, while conformal calibration brought interval coverage to **79.6%** and the bad-delay-day classifier reached **0.61 PR-AUC**
- Automated daily weather assembly, forecasting, append-only prediction logging, and **React + D3** dashboard publishing with **GitHub Actions**, supported by pytest, MLflow, data-quality and drift gates, and model and dataset cards


### Statistical Machine Learning

#### **Volatility Regime Forecasting** | [Repo](https://github.com/tisyasharma/volatility-regime-forecasting)

Leakage-aware time-series machine learning study forecasting whether 14 U.S. equities will enter a high-volatility regime over the following 10 trading days.

- Evaluated logistic regression, LightGBM, XGBoost, a HAR volatility benchmark, and matched naive baselines over **37,002 equity-day observations** using 28 expanding-window validation folds
- Identified nine days of feature-label overlap in an initial target, then redesigned the task using a forward-disjoint label, past-only thresholds, horizon-exact purging, and training-fold-only scaling
- Logistic regression achieved **0.368 average precision** versus **0.334** for the matched naive baseline, an exact **0.0335 lift** that remained significant after dependence-aware resampling and multiple-comparison correction


### Computational Biology

#### **Mouse AON Transcriptomics** | [Repo](https://github.com/tisyasharma/mouse-aon-transcriptomics)

Reproducible single-nucleus RNA-seq and spatial transcriptomics workflow integrating an in-house 10x Genomics AON library with Allen Brain Cell Atlas references to characterize cell populations and evaluate a predefined dorsolateral glutamatergic marker signature.

- Processed **32,952 QC-filtered nuclei** into 22 Leiden clusters, including eight excitatory clusters, thirteen inhibitory clusters, and one cluster retained as unassigned
- Integrated Allen Brain Cell Atlas 10x and MERFISH references and performed paired donor-level pseudobulk differential expression across ten donors, identifying **1,347 genes** meeting FDR and effect-size thresholds
- Built the analysis with **Scanpy, DESeq2, Snakemake, Docker, and GitHub Actions**, with independent reference-concordance checks, an optional scANVI label-transfer analysis, curated figures, and machine-readable results


### Full-Stack Applications

#### **Pocket Protectors** | [Repo](https://github.com/tisyasharma/pocket-protector) | [Live Demo](https://pocket-protector.vercel.app/)

Team-built personal finance application for tracking receipts, budgets, spending patterns, and financial goals.

- Co-developed a deployed architecture using a **React** frontend, **Flask** API, and **MySQL-compatible TiDB Cloud** database, with Docker Compose for local development
- Implemented a tiered receipt-categorization flow combining merchant rules, keyword matching, and a character n-gram **TF-IDF + logistic regression** classifier for stores not covered by deterministic rules
- Added confidence-gated predictions, categorization provenance, low-confidence fallback behavior, and API-based model retraining from categorized receipt data
