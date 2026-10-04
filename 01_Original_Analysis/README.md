# Project 1: Original Analysis (GSE39582)

Bioinformatics analysis of KRAS mutations in colorectal cancer using the GSE39582 dataset.

## What I did
- Analyzed 585 patient samples
- Identified 38 differentially expressed genes (DEGs)
- Built a PPI network using STRING
- Identified 5 hub genes: CLCA1, SPINK4, MUC2, REG4, TFF1
- Ran KEGG and GO pathway enrichment

## Tools
Python, Biopython, GEOparse, gseapy, NetworkX, pandas, scipy

## Files
- `KRAS_analysis.ipynb` — Full analysis notebook
- `KRAS_DEGs_final.csv` — Differentially expressed genes
- `hub_genes.csv` — Identified hub genes
- `PPI_network.csv` — Protein-protein interactions
- `KEGG_results.csv`, `GO_results.csv` — Pathway enrichment
