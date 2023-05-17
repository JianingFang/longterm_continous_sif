# LCSIF Generation
This repository contains the code associated with the manuscript "Reconstruction of a Long-term Solar-induced Fluorescence over 1982-2021". Specifically, the repository contains code (in Python and Jupyter notebooks) for
- Preprocessing MCD43C4 and OCO-2 SIF files to generate train and test datasets for calibrating the neurnal network for SIF reconstruction.
- Train the machine learning model to map from MCD43C4 to OCO-2 SIF
- Generating the LCSIF dataset using the trained model and calibrated reflectance parameters (LCREF).
- Evaluating the spatial and temporal patterns of LCSIF
- Evaluating the residual orbital effects in LCREF and downstream LCSIF products
- Evaluating LCSIF, CSIF, GOSIF, and VIs against FLUXNET GPP

Note that the source code was written and tested on the Ginsburg HPC cluster at Columbia University. The user will need to download the resulting datasets, configure the directories, and install all required packages prior to running the code. We have removed directory path and private access codes before uploading the scripts to GitHub. Questions regarding the code should be directed to Jianing Fang (jf3423@columbia.edu).

Also please note that this repository does not include the code for calibrating the AVHRR reflectance datasets against MODIS to generate the LCREF dataset. Questions regarding the LCREF dataset can be directed to Dr. Xu Lian (xl3179@columbia.edu).

The LCREF dataset is available at DOI 10.5281/zenodo.7920380.
The LCSIF dataset is available at DOI 10.5281/zenodo.7916851 for the AVHRR period, and DOI 10.5281/zenodo.7916879 for the MODIS period.


