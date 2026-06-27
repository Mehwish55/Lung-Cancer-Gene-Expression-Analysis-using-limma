# Lung Cancer Gene Expression Analysis using limma

## Project Overview

This project performs differential gene expression analysis on a public lung cancer microarray dataset using the Bioconductor `limma` package.

The analysis compares lung adenocarcinoma samples with normal lung tissue samples to identify significantly differentially expressed genes.

This project demonstrates a complete microarray gene expression workflow including data acquisition, preprocessing, statistical analysis, visualization, and result export.

---

## Dataset

**GEO Accession:** GSE10072

**Platform:** GPL96 (Affymetrix Human Genome U133A Array)

**Samples**

- Lung Adenocarcinoma: 58
- Normal Lung Tissue: 49

Total Samples: 107

Source:

https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE10072

---

## Objectives

- Download public gene expression data
- Create sample groups
- Perform differential expression analysis
- Identify significant genes
- Generate publication-quality visualizations
- Export results

---

## Tools and Packages

- R
- Bioconductor
- limma
- GEOquery
- ggplot2
- pheatmap

---

## Workflow

1. Download GSE10072 from GEO
2. Extract expression matrix
3. Create Cancer and Normal sample groups
4. Build design matrix
5. Fit linear model using limma
6. Apply empirical Bayes statistics
7. Identify differentially expressed genes
8. Generate Volcano Plot
9. Generate PCA Plot
10. Generate Heatmap
11. Export differential expression results

---

## Results

The analysis identified differentially expressed genes between lung adenocarcinoma and normal lung tissue.

Generated outputs include:

- Differential expression results (.csv)
- Volcano Plot
- PCA Plot
- Heatmap of Top 50 Genes

---

## Project Structure

```
Lung-Cancer-Gene-Expression-limma/
│
├── data/
├── figures/
│   ├── volcano_plot.png
│   ├── pca_plot.png
│   └── heatmap.png
│
├── results/
│   └── lung_cancer_limma_results.csv
│
├── scripts/
│   └── lung_cancer_limma_analysis.R
│
├── README.md
└── Lung-Cancer-Gene-Expression-limma.Rproj
```

---

## Skills Demonstrated

- Bioinformatics
- Microarray Analysis
- Differential Gene Expression
- limma
- Data Visualization
- R Programming
- Bioconductor
- Scientific Data Analysis

---

## Author

Mehwish
## Results

### Volcano Plot

![Volcano Plot](figures/volcano_plot.png)

---

### PCA Plot

![PCA Plot](figures/pca_plot.png)

## Key Findings

- Analyzed 22,283 genes across 107 lung tissue samples.
- Compared 58 lung adenocarcinoma samples with 49 normal lung tissue samples.
- Identified 10,884 significantly differentially expressed genes (adjusted p-value < 0.05).
- Generated volcano plot, PCA plot, and heatmap to visualize gene expression differences.

---

### Heatmap

![Heatmap](figures/heatmap.png)
