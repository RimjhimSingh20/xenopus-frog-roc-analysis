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
The moderate overlap (9.1%) with reference markers from Table 3 may reflect several factors. First, our stringent statistical thresholds (padj<0.05, log2FC>0.5) prioritize high-confidence markers over exhaustive discovery. Second, the use of three independent marker selection methods and requirement 
for consensus increases specificity but may reduce sensitivity. Third, differences in preprocessing pipelines, batch structures, and quality control between our analysis and the original study could affect marker detection. Importantly, we successfully validated the four most critical ROC markers (LEF1, EGFL6, FREM2, IGFBP2) that define ROC identity and function, supporting the biological validity of our findings. The 169 novel markers we identified represent potential discoveries that warrant experimental validation.
**
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
