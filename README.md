# yorkregion_crime_analysis
Exploratory analysis of contributing socioeconomic factors to crime within the York region.
# README

## Overview
This repository contains a project that investigates the relationship between neighborhood safety and a range of socio‑economic factors in York Region. The work is comprised of two main files:

1. [`analysis.md`](c:\Users\Patri\OneDrive\Desktop\Alek's Assignments\cpt\analysis.md)  
   • Implements data loading, cleaning, plotting, and logistic‑regression modeling in Python.  
   • Displays visualizations such as maps showing disseminations areas, crime incidence, and safety scores.  
   • Uses both [`crime_data_york_2024.csv`](data/crime_data_york_2024.csv) and [`dissemination.shp`](dissemination.shp) to spatially join crime data with Census boundaries.

2. [`latex_code.tex`](c:\Users\Patri\OneDrive\Desktop\Alek's Assignments\cpt\latex_code.tex)  
   • Provides the final compiled report in LaTeX format.  
   • Imports references from the relevant file ([`references.bib`](c:\Users\Patri\OneDrive\Desktop\Alek's Assignments\cpt\references.bib)) and shows how the final paper is structured.  
   • Contains tables, figures, and commentary about data, methodology, and findings.

## Data Sources and Citations
All external datasets are cited throughout the repository and in the LaTeX sources. Key references include:
- [`yrp2024`](c:\Users\Patri\OneDrive\Desktop\Alek's Assignments\cpt\references.bib) for York Regional Police crime data.  
- [`statcanCiteGuide`](c:\Users\Patri\OneDrive\Desktop\Alek's Assignments\cpt\references.bib) for general census guidelines and DA definitions.

Other statistical files (e.g., socio‑economic data) are obtained from the York Region Open Data Portal (2016 and 2021 Census data). Detailed references are collected in the [`references.bib`](c:\Users\Patri\OneDrive\Desktop\Alek's Assignments\cpt\references.bib).

## Major Findings
1. **Crime Hotspots**: The spatial join (shown in the figures within [`analysis.md`](c:\Users\Patri\OneDrive\Desktop\Alek's Assignments\cpt\analysis.md)) highlights certain Dissemination Areas with higher weighted “SAFETY_SCORE.”  
2. **Socio‑Economic Correlations**: Higher median incomes correlated with some types of offenses—possibly due to reporting patterns or property‑related crimes.  
3. **Logistic Regression Accuracy**: Achieved ~71.5% test‑set accuracy in predicting whether an area is “Safer” or “Less Safe.”  
4. **Key Drivers**: Variables like unemployment rate and migration rate had moderate associations with local safety levels.

Below is an example map from the analysis, illustrating crime counts per Dissemination Area. Refer to the notebook for details:

![Crime count per Dissemination Area](analysis_files/analysis_10_5.png)

To see further plots (e.g., demographic comparisons and regression outputs), open the rendered sections of the Jupyter Notebook portion in [`analysis.md`](c:\Users\Patri\OneDrive\Desktop\Alek's Assignments\cpt\analysis.md).

## How to Use
1. **Data Analysis**:  
   • Place the shapefile ([`dissemination.shp`](dissemination.shp) and related files) and CSV datasets (`data/*.csv`) in the correct folders.  
   • Run the Python code in [`analysis.md`](c:\Users\Patri\OneDrive\Desktop\Alek's Assignments\cpt\analysis.md) (best viewed in a Jupyter environment) to generate figures and model outputs.

2. **LaTeX Report**:  
   • Compile [`latex_code.tex`](c:\Users\Patri\OneDrive\Desktop\Alek's Assignments\cpt\latex_code.tex) with a LaTeX distribution supporting `biber` for references.  
   • The compiled PDF will contain an academic‑style write‑up and data references.

## License & Disclaimer
• This work uses public data from the York Region Open Data Portal, which may have its own license or usage terms.  
• The logistic‑regression model is for academic demonstration only and should not be used for critical decision‑making without further validation.

Feel free to clone or download this repository for educational purposes. For any issues or questions, open an issue on GitHub or contact the author.
