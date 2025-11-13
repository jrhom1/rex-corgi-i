## CoronaGraph Instrument Reference stars for Exoplanets I: Github repo for reproducing figures

This repository has a Jupyter notebook for creating each of the figures (1-8) in CoronaGraph Instrument Reference stars for Exoplanets I: Preliminary Vetting and Implications for the Roman Coronagraph and Habitable Worlds Observatory (Hom, J., Wolff, S. G., Clark, C. A. et al. 2025)

## Contents
- Jupyter Notebook for making Figures (Jupyter notebook) (CorGI_REx_I.ipynb). Using this notebook relies on all csv, txt, and npy files in this repository.
- Reference Star Properties csv (RefStar_S10_amendGrade.csv), necessary for creating Figures 2-8 in CorGI_REx_I.ipynb.
- Reference Star Properties schema csv (RefStar_S10_Schema.csv) Schema for Reference Star Properties csv, describes column names and units of columns.
- Numpy data arrays (.npy) for generating Figure 8 (FullSky_A_Step_1.npy, FullSky_AB_Step_1.npy, FullSky_ABC_Step_1.npy, FullSky_SolarDays_Step_1.npy)
- Unocculted HLC PSF profile (HLC_prof.csv), sourced from https://roman.ipac.caltech.edu/page/additional-coronagraph-instrument-parameters-model-and-data-html. Necessary for creating Figure 1.
- Table from Pecaut and Mamajek (2013) of main sequence spectral types, colors, and magnitudes (txt file, MamajekTable.txt). This is necessary for generating Figures 3 and 4 in the text.
- Observing log info for speckle observations csv (speckle_log_info.csv). Necessary for creating Figure 4.

## Data Access
All images and contrast curves can be accessed through ExoFOP (https://exofop.ipac.caltech.edu/tess/). The Jupyter notebook CorGI_REx_I.ipynb expects this data to be in a certain format (not the native format as posted on ExoFOP). This data and the v1.0.0 release of this repository are available here: https://doi.org/10.5281/zenodo.17548112

## Requirements
- python >=3.10
- astropy >= 7
- astroquery >=0.4
- matplotlib >=3.10
- numpy >= 2.2
- pandas >= 2.2
- roman-pointing >=1.0 (https://github.com/roman-corgi/roman_pointing/tree/main)
- scipy >=1.15

## References
Pecaut & Mamajek (2013); Intrinsic Colors, Temperatures, and Bolometric Corrections of Pre-main-sequence Stars, ApJS, 208, 9

The construction of RefStar_S10_amendGrade.csv involved programmatic querying of Simbad (https://simbad.cds.unistra.fr/simbad/), VizieR catalogs (https://vizier.cds.unistra.fr/viz-bin/VizieR), and the Gaia Archive (https://gea.esac.esa.int/archive/)

The specific catalogs queried were:

- Bourgés et al. (2014); The JMMC Stellar Diameters Catalog v2 (JSDC): A New Release Based on SearchCal Improvements, ASPC, 485, 223
- Duvert (2016); JMDC : JMMC Measured Stellar Diameters Catalogue, VizieR On-line Data Catalog: II/345
- Kervella et al. (2019); Stellar and substellar companions of nearby stars from Gaia DR2. Binarity from proper motion anomaly, A&A, 623, A72
- Kervella et al. (2022); Stellar and substellar companions from Gaia EDR3. Proper-motion anomaly and resolved common proper-motion pairs, A&A, 657, A7

References (in the form of ADS bibcodes) for other properties in RefStar_S10_amendGrade.csv are included within the csv file as column entries.
