# Project Title: Bioinformatics-Based Screening of Hub Genes for Prostate Cancer Bone Metastasis

## Description

This project, undertaken as part of an Introduction to Bioinformatics course, successfully replicated the methodologies and findings of the research paper, **"Bioinformatics-based screening of hub genes for prostate cancer bone metastasis and analysis of immune infiltration."** The project demonstrates the application of bioinformatics tools and techniques to identify key genes and pathways involved in prostate cancer (PCa) bone metastasis, validating the original study's results through independent analysis.

## Objectives

*   To identify differentially expressed genes (DEGs) associated with prostate cancer bone metastasis using the Gene Expression Omnibus (GEO) database (GSE32269).
*   To perform gene set enrichment analysis (GSEA) to identify significantly enriched biological pathways.
*   To construct and analyze protein-protein interaction (PPI) networks to identify hub genes potentially driving metastasis.
*   To analyze immune cell infiltration patterns in PCa samples and correlate them with hub gene expression.

## Tools and Resources

The following tools, databases, and programming languages were utilized:

*   **R Programming Language:**  The primary tool for data analysis, statistical computing, and visualization.
*   **Gene Expression Omnibus (GEO):** A public repository for gene expression data, providing the dataset GSE32269 for analysis.
*   **GEO2R:** Used for identifying Differentially Expressed Genes (DEGs) based on statistical significance.
*   **DAVID (Database for Annotation, Visualization and Integrated Discovery):** Used for functional annotation and enrichment analysis of DEGs.
*   **Cytoscape:** An open-source software platform for visualizing complex networks, particularly PPI networks.
*   **CytoHubba:** A Cytoscape plugin used to identify important nodes (hub genes) in biological networks.
*   **GEPIA2 (Gene Expression Profiling Interactive Analysis):** Used for validating mRNA expression and performing survival analysis of key genes.
*   **CIBERSORTx:** A tool for estimating the proportions of different immune cell types within a mixed cell population, used to analyze immune infiltration in PCa samples.
*   **STRING Database:** Used for constructing protein-protein interaction networks based on known and predicted protein interactions.

## Methodology

1.  **Data Acquisition:** Obtained the gene expression dataset GSE32269 from the Gene Expression Omnibus (GEO). This dataset includes mRNA samples from localized primary prostate cancers and bone metastases associated with prostate cancer.

2.  **Differential Expression Analysis:** Used GEO2R to identify differentially expressed genes (DEGs) between primary prostate cancer and bone metastasis samples, using thresholds of adjusted p-value < 0.05 and |logFC| >= 1.

3.  **Visualization:** Generated volcano plots (using `ggplot2` and `ggrepel`) to visualize DEGs and heatmaps (using `pheatmap`) to display the expression patterns of the top DEGs.

4.  **Functional Enrichment Analysis:** Performed Gene Ontology (GO) and KEGG pathway enrichment analysis using the DAVID database to identify significantly enriched biological processes and pathways.

5.  **Protein-Protein Interaction (PPI) Network Construction:** Constructed a PPI network using the STRING database with a confidence score > 0.4 and visualized it using Cytoscape.  The CytoHubba plugin was used to identify hub genes.

6.  **Hub Gene Identification:**  Identified hub genes based on their connectivity in the PPI network using CytoHubba.

7.  **Survival Analysis:**  Performed survival analysis using GEPIA2 to assess the prognostic significance of identified hub genes.

8.  **Immune Infiltration Analysis:**  Analyzed immune cell infiltration patterns in the tumor microenvironment using CIBERSORTx and correlated infiltration levels with hub gene expression.

## Key Findings

*   Identified a set of differentially expressed genes (DEGs) associated with prostate cancer bone metastasis.
*   Functional enrichment analysis revealed key biological pathways involved in metastasis, such as cell cycle regulation and immune response.
*   Protein-protein interaction network analysis identified several hub genes with high connectivity, suggesting their central roles in the metastatic process. CCNA2, NUSAP1, and PBK were validated as key hub genes through survival analysis.
*   Immune infiltration analysis showed that regulatory T cells (Tregs) and M0 macrophages may play a significant role in the metastatic process of PCa.


## Conclusion

This project successfully replicated the core findings of the original research paper, demonstrating the power of bioinformatics approaches in understanding the molecular mechanisms underlying prostate cancer bone metastasis. By integrating various bioinformatics tools and databases, the project identified key genes and pathways that may serve as potential therapeutic targets for combating PCa bone metastasis. The results contribute to the growing body of knowledge in cancer research and may inform future strategies for diagnosis and treatment.

