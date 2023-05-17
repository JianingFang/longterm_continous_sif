# LCSIF Generation
This repository contains the code associated with the manuscript "Reconstruction of a Long-term Solar-induced Fluorescence over 1982-2021". Specifically, the repository contains code (in Python and Jupyter notebooks) for
- Preprocessing MCD43C4 and OCO-2 SIF files to generate train and test datasets for calibrating the neurnal network for SIF reconstruction [MODIS_SIF.ipynb](https://github.com/JianingFang/longterm_continous_sif/blob/main/FLUXNET.ipynb).
- Train the machine learning model to map from MCD43C4 to OCO-2 SIF [MODIS_SIF.ipynb](https://github.com/JianingFang/longterm_continous_sif/blob/main/FLUXNET.ipynb)
- Generating the clear-sky LCSIF dataset using the trained model and calibrated reflectance parameters(LCREF) [Predict_LCSIF_Clear-Sky_MODIS_Period.ipynb](https://github.com/JianingFang/longterm_continous_sif/blob/main/Predict_LCSIF_Clear-Sky_MODIS_Period.ipynb) and [Predict_LCSIF_Clear-Sky_AVHRR_Period.ipynb](https://github.com/JianingFang/longterm_continous_sif/blob/main/Predict_LCSIF_Clear-Sky_AVHRR_Period.ipynb).
- Generating all-sky LCSIF dataset [Process_ERA5_and_Generate_LCSIF_v2.ipynb](https://github.com/JianingFang/longterm_continous_sif/blob/main/Process_ERA5_and_Generate_LCSIF_v2.ipynb)
- Evaluating the spatial and temporal patterns of LCSIF [Create_Trend_Figure-linear_regression.ipynb](https://github.com/JianingFang/longterm_continous_sif/blob/main/Create_Trend_Figure-linear_regression.ipynb) and [Create_Trend_Figure-Kenn-Mandall_test.ipynb](https://github.com/JianingFang/longterm_continous_sif/blob/main/Create_Trend_Figure-Kenn-Mandall_test.ipynb)
- Evaluating the residual orbital effects in LCREF and downstream LCSIF products, globally [GlobalSZAAnomaly.ipynb](https://github.com/JianingFang/longterm_continous_sif/blob/main/GlobalSZAAnomaly.ipynb) or at PICS sites [PICS_analysis_MODIS_AVHRR_comparison.ipynb](https://github.com/JianingFang/longterm_continous_sif/blob/main/PICS_analysis_MODIS_AVHRR_comparison.ipynb)
- Evaluating LCSIF, CSIF, GOSIF, and VIs against FLUXNET GPP [FLUXNET.ipynb](https://github.com/JianingFang/longterm_continous_sif/blob/main/FLUXNET.ipynb)

Note that the source code was written and tested on the Ginsburg HPC cluster at Columbia University. The user will need to download the resulting datasets, configure the directories, and install all required packages prior to running the code. We have removed directory path and private access codes before uploading the scripts to GitHub. Questions regarding the code should be directed to Jianing Fang (jf3423@columbia.edu).

Also please note that this repository does not include the code for calibrating the AVHRR reflectance datasets against MODIS to generate the LCREF dataset. Questions regarding the LCREF dataset can be directed to Dr. Xu Lian (xl3179@columbia.edu).

The LCREF dataset is available at DOI [doi:10.5281/zenodo.7920380](https://doi.org/10.5281/zenodo.7920380).
The LCSIF dataset is available at DOI [doi:10.5281/zenodo.7916851](https://doi.org/10.5281/zenodo.7916851) for the AVHRR period, and [doi:10.5281/zenodo.7916879](https://doi.org/10.5281/zenodo.7916879) for the MODIS period.


