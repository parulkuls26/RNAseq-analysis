**RNA-seq Analysis: Tumor vs Normal Tissue**

Introduction
This analysis examines RNA-seq data from matched tumor and normal tissue samples collected from 5 patients (S02, S03, S05, S06, S10), yielding a total of 10 samples. The raw count matrix contains expression data for 19,701 genes across these samples.
Since each patient contributed both a tumor and normal sample, this represents a paired experimental design. This pairing is statistically advantageous because it allows us to control for patient-to-patient variability (due to age, genetics, lifestyle, etc.) and focus on the true biological differences between tumor and normal tissue within each individual.

**Analysis Report**
📊 View the full interactive analysis report :
https://parulkuls26.github.io/RNAseq-analysis/RNAseq_github.html

**Analysis Objectives**

1. Implement a complete RNA-seq analysis workflow from raw counts to differential expression results
2. Visualize normalized gene expression and sample relationships
3. Identify top differentially expressed genes between tumor and normal groups
4. Perform Gene Set Enrichment Analysis (GSEA) to identify dysregulated biological pathways

## Pipeline

1. Gene filtering (remove low-expressed genes)
2. Normalization
3. Quality visualization (boxplot, PCA)
4. Differential expression analysis (paired design)
5. GSEA analysis (C5 GO BP gene sets)

**Key Outputs**

R Workflow - Complete code from raw counts to DE results
Boxplot - Normalized gene expression across all 10 samples
PCA Plot - Sample relationships and clustering
DE Table - Top 10 differentially expressed genes with statistics
GSEA Table - Top 10 GO Biological Process pathways
Enrichment Plots - Top 2 upregulated and top 2 downregulated pathways

**Tools & Packages**

R - Statistical computing
DESeq2 - Differential expression analysis (paired design)
fgsea / clusterProfiler - Gene set enrichment analysis
ggplot2 - Data visualization
C5 GO BP - Gene set collection for GSEA

**How to Reproduce**
1. Clone this repository:
git clone https://github.com/parulkuls26/RNAseq-analysis.git
2. Open RNAseq_github.Rmd in RStudio
3. Install required packages 
4. Knit the document to reproduce the analysis

