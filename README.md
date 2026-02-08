## Tisya Sharma

I'm currently a 4th year Data Science student at Northeastern University (5 year program, graduating 2027). I've worked on applied data science projects spanning time-series forecasting, biological data analysis, and model-driven applications. I really enjoy building and evaluating predictive models, designing data pipelines, and developing full-stack tools to explore and communicate results.

I’m excited to continue working with real-world, high-dimensional data and to contribute to projects where data science can support meaningful analysis and decisions!

---

## Projects

### **Flight Delay Forecasting**
Route-level time-series forecasting using U.S. flight data (2019–2025) and ERA5 weather reanalysis.
- Evaluated XGBoost, LightGBM, LSTM, and TCN models using **4-fold walk-forward validation**
- Best performance achieved by **XGBoost / LightGBM** (**11.25 min MAE, ~77.7% hit rate**)
- Removing weather features increased error by **10.3%**
- Built an interactive **React + D3 dashboard** for exploring forecasts, residuals, model comparisons, and performance diagnostics across routes and time  
- **Repo:** https://github.com/tisyasharma/flight-delay-forecasting
- **Live Demo:** https://tisyasharma.github.io/flight-delay-forecasting/ 

---

### **AON Single-Nucleus RNA-Seq Analysis**
Single-nucleus RNA sequencing analysis of the mouse Anterior Olfactory Nucleus integrating 10x Genomics data with the Allen Brain Cell Atlas.
- Applied **PCA-based dimensionality reduction and clustering** to analyze high-dimensional gene expression data.
- Analyzed **36,863 nuclei**, retaining **8,885 high-quality cells across 28 clusters**
- Identified spatial segregation of excitatory AON neurons into dorsolateral and ventromedial populations
- Discovered **Abi3bp** as the top marker of contralaterally-projecting neurons using FDR-corrected testing  
- **Repo:** https://github.com/tisyasharma/AON_snRNAseq_TS

---

### **Pocket Protectors**
Full-stack personal finance application with an ML-assisted receipt categorization pipeline.
- Flask API, React frontend, and MySQL backend
- Implemented a multi-stage categorization system with confidence-based routing
- Supports on-demand model retraining from user-corrected labels  
- **Repo:** [https://github.com/tisyasharma/pocket-protectors](https://github.com/tisyasharma/pocket-protector)
- **Live Demo:** https://pocketprotectors.up.railway.app/ -- Demo login accounts listed in project README.md

---

### **Twitter Storage Comparison**
Systems comparison of PostgreSQL and Redis for Twitter-style workloads.
- Benchmarked **~1M tweets** and **~10K follow relationships**
- PostgreSQL achieved higher write throughput; Redis provided faster timeline reads
- Explored architectural tradeoffs in fan-out strategies  
- **Repo:** https://github.com/tisyasharma/twitter-storage-comparison
