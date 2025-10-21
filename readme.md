## CoronaGraph Instrument Reference stars for Exoplanets I: Github repo for reproducing figures

This repository has a Jupyter notebook for creating each of the figures (1-8) in CoronaGraph Instrument Reference stars for Exoplanets I: Preliminary Vetting and Implications for the Roman Coronagraph and Habitable Worlds Observatory (Hom, J., Wolff, S. G., Clark, C. A. et al. 2025)

## Contents
- Jupyter Notebook for making Figures (CorGI_REx_I.ipynb)
- Reference Star Properties csv (RefStar_S10_amendGrade.csv)
- Reference Star Properties schema (RefStar_S10_Schema.csv) Schema for Reference Star Properties csv
- Numpy data arrays for generating Figure 8 (FullSky_A_Step_1.npy, FullSky_AB_Step_1.npy, FullSky_ABC_Step_1.npy, FullSky_SolarDays_Step_1.npy)
- Unocculted HLC PSF profile (HLC_prof.csv)
- Table from Pecaut and Mamajek (2013) of main sequence spectral types, colors, and magnitudes (MamajekTable.txt)
- Observing log info for speckle observations (speckle_log_info.csv)

## Requirements
- astropy >= 7
- astroquery >=0.4
- matplotlib >=3.10
- numpy >= 2.2
- pandas >= 2.2
- roman-pointing >=1.0 (https://github.com/roman-corgi/roman_pointing/tree/main)
- scipy >=1.15
