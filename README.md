# Leveraging Python for Spatial Data Science

## [Spatial Data Science Bootcamp Paris](https://spatial-data-science-conference.com/bootcamps/2023/) October 26th, 2023

[Florian Bayer](https://www.linkedin.com/in/florian-bayer-a4117b30/), PhD in Public Health, MSc in Geography

Health geographer at Agence de la biomédecine, University lecturer at Paris Panthéon Sorbonne and ENSG

## Objective
The aim of this workshop is to deliver an **overview** of spatial analysis tools that enable leveraging spatial dimension in your analyses.

Our primary focus will revolve around examining the spatial distribution of self-employed general practitioners (GPs), distinct from those employed by healthcare institutions, within the Paris metropolitan area and its surrounding regions.

The primary objective is to ascertain the presence of **spatial disparities** in the distribution of general practitioners throughout the Parisian region.

The data comes from the [french health ministry.](https://annuaire.sante.fr/web/site-pro/extractions-publiques)

## Workshop Outline:

- Spatial data management and geocoding
- Introduction to the Modifiable Areal Unit Problem (MAUP)
- Spatial autocorrelation and Hot Spot Detection
- Appendix : travel time computing

## Instructions

This workshop requires Python 3.x (specifically tested with version 3.9). The primary packages utilized in this workshop include:
- [geopandas](https://github.com/geopandas/geopandas) for efficient geographic data handling
- [h3pandas](https://github.com/DahnJ/H3-Pandas) for spatial aggregation
- [matplotlib](https://github.com/matplotlib/matplotlib) for creating maps and visualizations
- [scipy](https://github.com/scipy/scipy) and [splot](https://github.com/pysal/splot) and [esda](https://github.com/pysal/esda) for performing statistical calculations
- [libpysal](https://github.com/pysal/libpysal) for constructing spatial weight matrices
- [geopy](https://github.com/geopy/geopy) for distance calculations based on geographic coordinates
- Additionally, [Jupyter lab](https://github.com/jupyterlab/jupyterlab) is recommended for an interactive environment

Feel free to clone the repository : 
[https://github.com/fbxyz/SDS_Bootcamp](https://github.com/fbxyz/SDS_Bootcamp)

You can install them in your preferred Python virtual environment or use conda :

1. First clone this git repo
```
git clone https://github.com/fbxyz/SDS_Bootcamp
cd SDS_Bootcamp
```
2. Create and activate the conda environment
```
conda create -n bootcamp_level python=3.9 mamba -c conda-forge
conda activate bootcamp_level
```
3.Install packages with mamba
```
mamba install -c conda-forge geopandas h3pandas matplotlib scipy libpysal esda splot geopy notebook jupyterlab
```

4. Optionally, add the environment as a Jupyter kernel
```
python -m ipykernel install --sys-prefix --name bootcamp_level
```
5. Launch Jupyter Notebook or Jupyter Lab
```
jupyter lab
```
