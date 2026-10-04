# Project 2: AI Variant Effect Prediction (ESM-2)

Using the ESM-2 protein language model to predict the impact of KRAS mutations.

## What I did
- Fetched KRAS protein sequence from UniProt (P01116)
- Loaded ESM-2 model from Hugging Face
- Calculated ESM-2 scores for 14 common KRAS mutations
- Visualized predicted impact

## Tools
Python, ESM-2, Hugging Face Transformers, PyTorch, Biopython

## Key Findings
- K117N, G13C, G12D showed the most deleterious scores
- ESM-2 predicts structural impact, not clinical pathogenicity

## Files
- `ESM2_KRAS_analysis.ipynb` — Full analysis notebook
- `kras_esm2_scores.png` — Bar plot of ESM-2 scores
- `kras_mutation_esm2_scores.csv` — Raw scores
