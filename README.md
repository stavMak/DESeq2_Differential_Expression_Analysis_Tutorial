# DESeq2 Differential Expression Analysis: METTL3 / METTL14 Knockouts

Differential gene expression analysis of **METTL3** and **METTL14** knockout samples using [DESeq2](https://bioconductor.org/packages/DESeq2/). METTL3 and METTL14 form the core catalytic complex responsible for **m6A (N6-methyladenosine)** RNA methylation, so knocking them out lets us explore how loss of m6A writing reshapes the transcriptome.

## 🔗 View the report

**➡️ [Open the full analysis report](https://stavmak.github.io/DESeq2_Differential_Expression_Analysis_Tutorial/index.html)**

The report is a knitted R Markdown document with all code, plots, and results rendered as a web page — no need to run anything to read it.

## Overview

This project walks through a complete RNA-seq differential expression workflow in R:

- Loading and inspecting the count data
- Building the `DESeqDataSet` and setting up the experimental design
- Running the DESeq2 pipeline (size-factor normalization, dispersion estimation, model fitting)
- Extracting and interpreting differentially expressed genes
- Visualizing the results

## Data

- **Organism:**  Drosophila
- **Conditions:** METTL3 knockout, METTL14 knockout, and control (wild-type)
- **Replicates:** 3 per condition

## Methods

The analysis was carried out in **R** with the following main packages:

- `DESeq2` — differential expression testing
- `ggplot2` — visualization


The full, reproducible code lives in [`DESeq2_METTL3_METTL14_KO.Rmd`](DESeq2_METTL3_METTL14_KO.Rmd).

## Key results

See the [full report](https://stavmak.github.io/DESeq2_Differential_Expression_Analysis_Tutorial/index.html) for all plots and tables.

## Repository contents

| File                           | Description                                   |
| ------------------------------ | --------------------------------------------- |
| `DESeq2_METTL3_METTL14_KO.Rmd` | The R Markdown source with all analysis code  |
| `index.html`                   | The knitted report (rendered on GitHub Pages) |
| `README.md`                    | This file                                     |

## How to reproduce

1. Clone the repository:
   ```bash
   git clone https://github.com/stavMak/DESeq2_Differential_Expression_Analysis_Tutorial.git
   ```
2. Open the `.Rmd` file in RStudio.
3. Install the required packages (DESeq2 from Bioconductor, plus the plotting packages listed above).
4. Knit the document to reproduce the report.

## Author

**Stavroula Makri**

