# Leveraging Python for Spatial Data Science

## [Spatial Data Science Bootcamp Paris](https://spatial-data-science-conference.com/bootcamps/2023/) October 26th, 2023

[Florian Bayer](https://www.linkedin.com/in/florian-bayer-a4117b30/), PhD in Public Health, MSc in Geography

Health geographer at Agence de la biomédecine, University lecturer at Paris Panthéon Sorbonne and ENSG

## Objective
The objective of this workshop is to provide an overview of spatial analysis tools that enable leveraging spatial dimension in your analyses.

We will focus on the issue of the spatial distribution of self-employed general practitioners (not employed by a healthcare institution) in Paris and its outskirts. 

The goal is to determine whether there are spatial disparities in the distribution of general practitioners related to the population.

The data comes from the [french health ministry.](https://annuaire.sante.fr/web/site-pro/extractions-publiques)

## Workshop Outline:

- Spatial data management and geocoding
- Introduction to the Modifiable Areal Unit Problem (MAUP)
- Frontier effect
- Spatial autocorrelation and Hot Spot Detection

## Instructions

This workshop requires Python 3.x (tested with 3.9). The main packages used are :
- [geopandas](https://github.com/geopandas/geopandas) for handling geographic data
- [h3pandas](https://github.com/DahnJ/H3-Pandas) for spatial aggregation
- [matplotlib](https://github.com/matplotlib/matplotlib) for mapping
- [scipy](https://github.com/scipy/scipy) and [splot](https://github.com/pysal/splot) and [esda](https://github.com/pysal/esda) for statistical calculations 
- [libpysal](https://github.com/pysal/libpysal) for creating spatial weight matrices
- [geopy](https://github.com/geopy/geopy) for calculating distances from geographic coordinates
- and [Jupyter lab](https://github.com/jupyterlab/jupyterlab).

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
