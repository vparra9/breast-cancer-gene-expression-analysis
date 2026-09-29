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

## Initial Data Exploration

The dataset was loaded and explored using Python and pandas.

The first inspection of the dataset shows that:

- Rows represent individual genes.
- The first column contains Ensembl gene identifiers.
- The remaining columns represent individual tumor samples.
- Gene expression values are represented using TPM (Transcripts Per Million) normalized measurements.
