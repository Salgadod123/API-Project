# API Project
Used star data to plot an HR diagram
 HR Diagram from Vizier API Data

This project demonstrates how to retrieve stellar catalog data from the Vizier API, process it, and visualize a classic Hertzsprung–Russell (HR) diagram, a cornerstone of stellar astrophysics.

The resulting plot compares absolute magnitude to color index (B−V) — revealing the structure and life stages of stars, from the main sequence to red giants and white dwarfs.
 Project Overview

     Accessed star data using astroquery and the Vizier catalog service

     Cleaned and filtered raw data to remove outliers and missing values

     Calculated or extracted absolute magnitude and B−V color index

     Plotted the HR diagram using Matplotlib

     Inverted the y-axis (lower magnitudes = brighter stars) for proper visual convention

 Technologies & Tools Used

    astroquery.vizier for API access to star catalogs (e.g., Hipparcos, Tycho-2)

    pandas for data manipulation

    matplotlib for plotting

    numpy for numerical filtering and transformations
    
    tableu public for further plotting

Check out the tableu public vizz fir this project: https://public.tableau.com/app/profile/david.salgado4874/viz/StarDataVisualizationAbsoluteMagnitudevsBVIndex/Story1
Use https://nbviewer.org/ to view the notebook