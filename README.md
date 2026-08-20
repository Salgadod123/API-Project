# Hertzsprung–Russell Diagram from VizieR Catalog Data

This project uses the `astroquery` VizieR client to retrieve Hipparcos stellar data, clean the returned catalog fields, calculate distance and absolute magnitude, and visualize a Hertzsprung–Russell (HR) diagram.

## Objective

Build a compact astronomy data workflow that moves from a remote catalog query to calculated stellar properties, an analysis-ready CSV, and a scientifically conventional visualization.

## Tools and Technologies

- Python
- `astroquery.vizier`
- pandas and NumPy
- Matplotlib
- Jupyter Notebook
- Tableau Public

## Workflow

1. Query the Hipparcos main catalog (`I/239/hip_main`) for HIP identifier, apparent magnitude, parallax, and B−V color index.
2. Remove records with missing values or nonpositive parallax.
3. Convert parallax to distance in parsecs.
4. Calculate absolute magnitude from apparent magnitude and distance.
5. Plot absolute magnitude against B−V color index and invert the magnitude axis by astronomical convention.
6. Export the cleaned B−V and absolute-magnitude values for reuse.

## Key Results and What This Demonstrates

- Produces a cleaned 48-row catalog snapshot and an HR-diagram visualization.
- Demonstrates remote scientific-catalog access, null and validity filtering, derived-variable calculation, CSV export, and domain-aware plotting.
- Connects an API-oriented data-acquisition step with both Python and Tableau visualization workflows.

## Visualization

[View the related Tableau story](https://public.tableau.com/app/profile/david.salgado4874/viz/StarDataVisualizationAbsoluteMagnitudevsBVIndex/Story1)

## Repository Contents

| Path | Description |
| --- | --- |
| [`APIproject.ipynb`](APIproject.ipynb) | Catalog query, cleaning, calculations, export, and HR diagram |
| [`hr_diagram_data.csv`](hr_diagram_data.csv) | Cleaned B−V color-index and absolute-magnitude values |

## Viewing Notes

[View the notebook in nbviewer](https://nbviewer.org/github/Salgadod123/API-Project/blob/main/APIproject.ipynb) if GitHub does not render the plot.
