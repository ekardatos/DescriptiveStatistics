# Descriptive Statistics
A quantitative corpus linguistics study analyzing the lexical richness and vocabulary structure of a Greek literary text using six statistical indices. The corpus is derived from *"Οι Εθελοντές" (The Volunteers)* by Niovi Lyri — a contemporary Greek novel.

---

## Overview

This project investigates the statistical properties of vocabulary distribution in Modern Greek prose. The source text is split into fixed-size sub-corpora (N > 30), and six lexical richness indices are computed for each segment using QUITA. The distribution of each index across segments is then analyzed statistically and visualized using Python.

---

## Corpus

| Property | Details |
|---|---|
| **Text** | *Οι Εθελοντές* (The Volunteers) |
| **Author** | Niovi Lyri |
| **Language** | Modern Greek |

---

## Lexical Richness Indices

| Index | Description |
|---|---|
| **TTR** (Type-Token Ratio) | Ratio of unique words to total words — measures vocabulary richness |
| **h-Point** | The point on the rank-frequency curve where a word's rank equals its frequency — divides vocabulary into two functional categories |
| **Entropy** | Measures vocabulary concentration — lower entropy indicates a more concentrated, less rich vocabulary |
| **Average Token Length** | Mean character length of tokens in each sub-corpus |
| **R1** | Richness index based on h-Point — covers all words ranked below the h-Point |
| **Λ (Lambda)** | Measures the frequency structure of text, combining richness with the distribution of neighboring frequencies |

---

## Methodology

1. **Text Selection** — one Greek literary text
2. **Corpus Segmentation** — the full text is split into N > 30 equal-length sub-files using Python (punctuation removed, lowercased, tokenized)
3. **Index Computation** — TTR, h-Point, R1, Entropy, Λ, and Average Token Length computed per sub-file using **QUITA** (Quantitative Index Text Analyzer); results exported to CSV
4. **Dominant Value** — modal value identified for the h-Point index
5. **Outlier Detection** — outliers identified and removed for each index
6. **Descriptive Statistics** — mean, median, and standard deviation computed post-outlier removal
7. **Visualization** — histograms with KDE (probability density function) and boxplots generated per index
8. **Distribution Analysis** — skewness assessed for each index and compared against normal distribution

---

## Repository Structure

```
├── descriptive_statistics.ipynb           # Main script
├── Multiple Text Project 1 - Results.csv  # Computed index values per sub-corpus (from QUITA)
├── Εθελοντές - Νιόβη Λύρη.txt             # Source text (Modern Greek, plain text)
├── requirements.txt                       # Python dependencies
└── README.md
```


## Key Findings

- All six indices show **near-symmetric distributions** with skewness values between -0.5 and +0.5.
- **5 out of 6 indices exhibit negative skewness**, meaning most sub-corpus values cluster above the mean — the text segments are relatively homogeneous in vocabulary richness.
- The **R1 index is the sole exception**, showing positive skewness — indicating greater variability in the lower-frequency vocabulary across segments.
- These results suggest that *The Volunteers* maintains a **consistent lexical register** throughout, with limited variance in vocabulary richness across text segments.

---
