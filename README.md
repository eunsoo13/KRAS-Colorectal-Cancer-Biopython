# KRAS-Colorectal-Cancer-Biopython
Bioinformatics Analysis of KRAS Mutation in Colorectal Cancer: Identification of Hub Genes and Signaling Pathways
# Identification of Hub Genes and Signaling Pathways Associated with KRAS Mutation in Colorectal Cancer

# Project Overview
Bioinformatics analysis to identify hub genes and signaling pathways associated with KRAS mutation in colorectal cancer using gene expression data.

# Data Source
- **Dataset:** GSE39582
- **Samples:** 585 colorectal cancer samples
- **Source:** GEO (Gene Expression Omnibus)
- **Platform:** Affymetrix Microarray

# Methods
1. Data download and preprocessing using `GEOparse`
2. Sample grouping: KRAS-Mutant (217) vs KRAS-WildType (328)
3. Differential Expression Analysis (DEGs) using t-test with FDR correction
4. Protein-Protein Interaction (PPI) network construction using STRING
5. Hub gene identification using NetworkX centrality measures
6. KEGG and GO pathway enrichment analysis using `gseapy`

# Results
- **38 significant DEGs** identified (adj.p < 0.05 and |log2FC| > 0.58)
- **Top 5 hub genes:** CLCA1, SPINK4, MUC2, REG4, TFF1
- **Key pathways:** Gastric cancer, Renin secretion, Innate immune response

# Key Findings
- KRAS mutation is associated with altered expression of genes involved in **mucin production** (MUC2, TFF1)
- **REG4** and **SPINK4** show significant upregulation in KRAS-mutant tumors
- Enriched pathways suggest involvement in **immune response** and **cellular secretion**

# Limitations
- The analysis was performed on a single microarray dataset (GSE39582) from the Affymetrix platform, which may not fully capture all transcriptomic changes.
- The KRAS-mutant group (n=217) was smaller than the WildType group (n=328), which could affect statistical power.
- Microarray data provide relative expression levels and may have lower sensitivity compared to RNA-seq.
- All findings are based on *in silico* analysis and require experimental validation (e.g., qPCR, Western blot).
- Some clinical annotations were incomplete (40 samples with unknown KRAS status).
- The study focused only on KRAS mutation and did not account for co-occurring mutations (e.g., TP53, BRAF, PIK3CA).

# Future Work
- Validate the identified hub genes using independent datasets (e.g., TCGA-COAD, GEO RNA-seq datasets).
- Perform survival analysis (Kaplan-Meier, Cox regression) to assess the prognostic value of hub genes.
- Investigate the role of hub genes in drug response and potential drug repurposing.
- Apply single-cell RNA-seq analysis to explore tumor heterogeneity in KRAS-mutant colorectal cancer.
- Conduct functional enrichment with more comprehensive databases (e.g., Reactome, WikiPathways).
- Experimental validation of hub genes using cell lines and patient samples.
- Integrate multi-omics data (genomics, proteomics, metabolomics) for a systems-level understanding.

# Tools & Technologies
- **Language:** Python 3
- **Libraries:** Biopython, GEOparse, gseapy, NetworkX, pandas, scipy, statsmodels
- **Platform:** Google Colab

# Files
- `KRAS_analysis.ipynb` — Complete analysis notebook
- `KRAS_DEGs_final.csv` — Differentially expressed genes
- `PPI_network.csv` — Protein-protein interaction network
- `hub_genes.csv` — Identified hub genes
- `KEGG_results.csv` — KEGG pathway enrichment results
- `GO_results.csv` — GO enrichment results

# References
- Marisa et al. (2013) — GSE39582 dataset
- STRING database — PPI network
- Enrichr — Pathway enrichment analysis

# Author
- Nargess Soleimany _ Lee Eunsoo
[اسم خودت رو اینجا بنویس]
