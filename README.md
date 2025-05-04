# Drug Property Analysis Using PubChem Data

## Overview
This project involves retrieving molecular data for selected compounds from the PubChem database and analyzing their physicochemical properties, particularly **Molecular Weight** and **LogP** (XLogP). These properties play a crucial role in drug development, especially in solvent selection, formulation, and bioavailability prediction.

## Objectives
- Load and explore compound data using Pandas.
- Visualize trends in molecular weight and lipophilicity (XLogP).
- Understand how these trends influence drug formulation and solvent selection.

## Dataset
The data was fetched directly from PubChem using the REST API:


Fields included:
- CID: Compound ID
- MolecularWeight
- XLogP: An estimation of LogP
- InChIKey
- CanonicalSMILES

## Steps Performed

### 1. Data Loading
Used `pandas` to read the dataset from the provided URL.

### 2. Data Inspection
  Verified column names, data types, and checked for missing values.
  Displayed descriptive statistics and data preview.

### 3. Data Cleaning
  Removed duplicate rows.
  Checked for any null or malformed entries in key columns.

### 4. Visualization
  Used `matplotlib` and `seaborn` to:
  Plot the relationship between Molecular Weight and XLogP using a scatterplot.
  Display **XLogP** values across different compounds using a barplot.

### 5. Property Trends Interpretation

#### Key Insight:
  low Molecular Weight & Low XLogP (Hydrophilic): Better suited for aqueous (water-based) solvents.
  High Molecular Weight & High XLogP (Hydrophobic): Require **lipophilic or organic solvents.

#### Examples:
  Paracetamol (lower LogP): Easily dissolves in water-based solvents.
  Aspirin (higher LogP): More suited for organic solvents.

These insights are critical in optimizing drug **solubility**, **absorption**, and **bioavailability**.

## Technologies Used
- Python 3.x
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Conclusion
This analysis highlights the importance of molecular properties in pharmaceutical formulation. LogP and molecular weight trends provide a strong basis for selecting appropriate solvents, impacting the overall effectiveness and stability of drug compounds.


Author: Abotula sai sandeep 
Date: 04/05/2025
