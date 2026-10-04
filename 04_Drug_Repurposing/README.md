# Project 4: Network-Based Drug Repurposing (DGIdb)

Built a drug-gene interaction network to identify potential repurposing candidates for KRAS-mutant colorectal cancer.

## What I did
- Queried DGIdb for drug-gene interactions
- Filtered for approved drugs
- Built a drug-gene interaction network using NetworkX
- Identified potential repurposing candidates

## Tools
Python, DGIdb API, NetworkX, matplotlib

## Key Findings
- KRAS is highly druggable with dozens of approved drugs
- MUC2 connected to Mirametinib — a potential repurposing candidate
- CLCA1, SPINK4, REG4, TFF1 represent "drug gaps" for novel discovery

## Files
- `Drug_repurposing.ipynb` — Full analysis notebook
- `drug_gene_network.png` — Drug-gene network visualization
- `drug_gene_interactions.csv` — Raw interaction data
