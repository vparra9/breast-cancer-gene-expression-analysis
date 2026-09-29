# Breast Cancer Gene Expression Analysis

A python-based bioinformatics and data science project analyzing gene expression patterns in primary and metastatic breast cancer.

## Project Goal

This project investigates whether gene expression patterns can distinguish primary breast tumors from metastatic tumors and explores which genes may contribute most strongly to those differences

## Technologies
- Python
- Jupyter Notebook / IPython

## Status 
In progress

## Dataset

![Breast cancer gene expression dataset](images/breast_cancer_table.png)

The dataset used in this project is the **GSE191230** RNA-seq dataset from the NCBI Gene Expression Omnibus (GEO).

The study contains gene expression data from **20 breast cancer tumor samples**, including primary breast tumors and distant metastatic tumors.

The processed dataset contains TPM-normalized gene expression measurements, allowing gene expression levels to be compared across tumor samples.

- **M samples** represent metastatic tumors.
- **P samples** represent primary tumors.
- Each row represents a gene identified using an Ensembl gene ID.
- Each numerical value represents the expression level of that gene within a particular tumor sample.

### Understanding the Dataset

- **M samples (Metastatic tumors):** Samples taken from tumors that have spread from the original breast cancer site to another part of the body.

- **P samples (Primary tumors):** Samples taken from the original tumor located in the breast, before considering spread to distant parts of the body.

- **Ensembl Gene ID:** A standardized identifier assigned to a gene by the Ensembl genome database. For example, `ENSG00000186827` identifies a specific human gene.

- **Gene expression:** A measurement of how actively a gene is being used within a biological sample. In this dataset, higher values generally indicate higher measured expression of that gene.

- **TPM (Transcripts Per Million):** A normalization method used with RNA sequencing data that adjusts gene expression measurements so expression levels can be compared more meaningfully across samples.

Therefore, each **row** represents a gene, each **M or P column** represents a tumor sample, and each **numerical value** represents the TPM-normalized expression level of a particular gene within a particular tumor sample.

## Initial Data Exploration

The dataset was loaded and explored using Python and pandas.

The first inspection of the dataset shows that:

- Rows represent individual genes.
- The first column contains Ensembl gene identifiers.
- The remaining columns represent individual tumor samples.
- Gene expression values are represented using TPM (Transcripts Per Million) normalized measurements.
