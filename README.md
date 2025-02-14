# cymirCNV
## A cytoscape plugin for miRNA-gene correlation network visualization

cymirCNV is a Cytoscape plug-in designed for constructing and visualizing miRNA-gene correlation networks from expression data. It supports Pearson and Spearman correlation analysis, allowing users to explore regulatory interactions with customizable thresholds. Ideal for researchers studying miRNA-mediated gene regulation, cymirCNV streamlines data preprocessing, correlation computation, and network visualization within Cytoscape.

# cymiRCNV: A Step-by-Step Tutorial
## A Cytoscape plug-in for miRNA-Gene Correlation Network Analysis

## 1. Introduction
cymiRCNV is a Cytoscape plug-in designed for constructing and visualizing miRNA-gene correlation networks from expression data. It supports Pearson and Spearman correlation analysis and allows users to explore regulatory interactions interactively.

## 2. Installation
### Method 1: Install from Cytoscape App Store
Open Cytoscape.
Go to Apps → App Manager.
Search for cymiRCNV.
Click Install and wait for the installation to complete.
Restart Cytoscape to enable the plug-in.
### Method 2: Manual Installation (Alternative)
Download the cymiRCNV JAR file from the Cytoscape App Store or GitHub.
In Cytoscape, go to Apps → App Manager → Install from File.
Select the downloaded cymiRCNV JAR file and click Open.
Restart Cytoscape to apply changes.

## 3. Preparing Input Data
### Required Data Format
To use cymiRCNV, you need paired gene and miRNA expression data with the same samples.

File Format: CSV
The first column should contain miRNA/gene IDs.
The remaining columns should contain expression values for samples.
Each sample column in miRNA data should exactly match the sample columns in mRNA data.
Example: miRNA Expression Data
miRNA/gene	Sample1	Sample2	Sample3	Sample4
miR-21	5.2	4.8	6.1	5.7
miR-155	2.1	3.0	1.8	2.5
Example: Gene Expression Data
miRNA/gene	Sample1	Sample2	Sample3	Sample4
TP53	1.5	2.4	3.2	2.8
BCL2	2.8	3.1	4.0	3.7
🚨 Important Notes:
✔ File format: Ensure the data is correctly formatted (no missing values).
✔ Matching columns: The sample IDs must be identical in both miRNA and gene expression datasets.
