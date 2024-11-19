# Epigene_project

This repository contains the 2 tasks of the Epigene technical challenge. The task 1 is in Jupyter Notebook format and the task 2 is in PDF format.

## Task 1 : Single-Cell RNA-seq Integration and Pre-processing Pipeline

This script is designed to reproduce the integration and pre-processing steps performed on a single-cell RNA-seq dataset. By analyzing a preprocessed reference dataset (referred to as the "targeted dataset"), the script identifies the necessary steps for pre-processing single-cell data and applies them from scratch to raw data, resulting in a processed dataset comparable to the targeted dataset.
### Features

    Raw Data Input:
    The script works with raw single-cell data in the standard 10x Genomics format, including:
        barcodes.tsv.gz
        features.tsv.gz
        matrix.tsv.gz
        Data from two samples are integrated into a single dataset.

    Data Integration:
    Raw data from the two samples are combined into an AnnData object for further analysis.

    Pre-processing:
    Using the Scanpy library, the script applies the following pre-processing steps:
        Quality control (e.g., filtering cells and genes based on user-defined thresholds).
        Normalization and scaling of gene expression data.
        Dimensionality reduction techniques (e.g., PCA).

    Output:
    The resulting preprocessed AnnData object is aligned with the structure and features of the targeted dataset, making it suitable for downstream analyses.

Requirements

To run this script, you will need the following:

    Python version: >=3.8
    Required Python packages:
        scanpy
        anndata
        numpy
        pandas
        matplotlib
        mygene
        pybiomart
        gzip
        scipy.io

## Task 2 : Improve the RNAseq data integration pipeline
You will find in PDF format a report with the different comments on the pipeline.
