# xenopus-frog-roc-analysis
Single-cell RNA-seq analysis identifying Regeneration-Organizing Cells in Xenopus laevis
# Identification of Regeneration-Organizing Cells in Xenopus laevis

Single-cell RNA-seq analysis identifying and characterizing ROCs in tadpole tail regeneration.

## Project Overview

This project computationally identifies Regeneration-Organizing Cells (ROCs) in *Xenopus laevis* tadpole tail using single-cell RNA sequencing data from [Aztekin et al., 2019](https://science.sciencemag.org/content/364/6441/653).

Key Findings:
- Identified 249 ROC cells (1.89% of total)
- Characterized by TP63+/LEF1+ co-expression
- Discovered 199 ROC-specific marker genes
- Validated 4 markers from original publication
- Identified 169 novel ROC markers

Methods

- **Clustering:** Leiden & Louvain algorithms (ARI=0.915)
- **Marker Selection:** Wilcoxon, t-test, logistic regression
- **Quality Control:** Cell/gene filtering, batch correction (Combat & Harmony)
- **Analysis Tools:** Python, scanpy, pandas, scikit-learn

Data Source
Data from: Aztekin, C., et al. (2019). "Identification of a regeneration-organizing cell in the Xenopus tail." Science 364(6441), 653-658.
Note: Data file not included due to size. Download from GEO or original publication.

Citation
Rimjhim Singh. (2025). Identification of Regeneration-Organizing Cells in Xenopus laevis. 
GitHub repository: https://github.com/RimjhimSingh20/xenopus-roc-analysis
