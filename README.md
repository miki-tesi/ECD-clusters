# ECD-clusters
Cluster analysis on Erdheim-Chester Disease patients data

**Author**: Michelangelo Tesi  
**Date**: April 2025

## Overview

This repository contains code for generating synthetic Erdheim-Chester Disease (ECD) patient data and analyzing it using **Multiple Correspondence Analysis (MCA)** followed by **Hierarchical Clustering on Principal Components (HCPC)**. The analysis replicates and explores clinical cluster structures and patient outcomes. This is the code (except for the simulation part) that was used to generate the results presented in the paper by Tesi M et al 2025 "Cluster Analysis Reveals the Clinical Spectrum of Erdheim-Chester Disease".

## Features

- **Synthetic Data Generation**: Realistic simulation of ECD organ involvement, demographics, mutation status, therapies, and survival outcomes.
- **Preprocessing**: Computation of cardiovascular risk scores, number of involved organs, and therapy response indicators.
- **MCA + HCPC**: Dimensionality reduction and clustering on categorical clinical features.
- **Cluster Validation**: Bootstrap-based cluster stability assessment using Jaccard similarity index.
- **Visualizations**:
  - Clustered heatmaps of V-test scores
  - Radar plots of feature prevalence
  - Dot plots of cluster-wise variable means
  - Kaplan-Meier survival curves stratified by cluster
- **Cluster Summary Tables**: Publication-ready descriptive statistics stratified by cluster using `gtsummary`.

## File Structure

- `simulate_ECD_cluster_analysis.Rmd` – Full analysis pipeline (simulation → clustering → characterization of the clusters)
