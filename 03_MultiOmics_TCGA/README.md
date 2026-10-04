# Project 3: Multi-Omics Validation (TCGA)

Validated hub gene findings in an independent TCGA cohort using cBioPortal API.

## What I did
- Queried TCGA colorectal cancer data via cBioPortal API
- Retrieved mRNA expression and KRAS mutation data
- Compared hub gene expression between KRAS-Mutant and WildType
- Validated findings from GSE39582 in an independent cohort

## Tools
Python, cBioPortal API, pandas, matplotlib, seaborn

## Key Findings
- Hub genes (MUC2, REG4, TFF1) show higher expression in KRAS-mutant tumors
- Cross-validation confirms KRAS drives a distinct transcriptional program

## Files
- `TCGA_analysis.ipynb` — Full analysis notebook
- `tcga_hub_genes_boxplot.png` — Boxplot of hub genes
- `tcga_mrna_clean.csv` — mRNA expression matrix
- `tcga_kras_mutations.csv` — KRAS mutation data
