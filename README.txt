Readme:

Content:

The following trained VNN models are included.
1. FTDC_100x7_models: This folder includes the 100 VNNs that were trained on FTDC100 dataset.
2. FTDC_300x7_models: This folder includes the 100 VNNs that were trained on FTDC300 dataset.
3. FTDC_500x7_models: This folder includes the 100 VNNs that were trained on FTDC500 dataset.
4. OASIS3_VNN: This folder includes the 100 VNNs that were trained on HC group in OASIS-3 dataset.

5. Data: This folder contains the following:
     a) CT_100_CN.pt: z-score normalized cortical thickness organized according to 100 parcellation version of Schaefer's atlas for HC group in FTDC100 dataset.
     b) CT_300_CN.pt: z-score normalized cortical thickness organized according to 300 parcellation version of Schaefer's atlas for HC group in FTDC300 dataset.
     c) CT_500_CN.pt: z-score normalized cortical thickness organized according t0 500 parcellation version of Schaefer's atlas for HC group in FTDC500 dataset.
     d) C_100_CN.pt: normalized anatomical covariance matrix (max eigenvalue = 1) derived from cortical thickness organized according to 100 parcellation version of Schaefer's atlas for HC          group in FTDC100 dataset.
     e) C_300_CN.pt: normalized anatomical covariance matrix (max eigenvalue = 1) derived from cortical thickness organized according to 300 parcellation version of Schaefer's atlas for HC          group in FTDC300 dataset.
     f) C_500_CN.pt: normalized anatomical covariance matrix (max eigenvalue = 1) derived from cortical thickness organized according to 500 parcellation version of Schaefer's atlas for HC          group in FTDC500 dataset.

Contact sihags@pennmedicine.upenn.edu for the following.

     g) C_OASIS_HC.pt: normalized anatomical covariance matrix (max eigenvalue = 1) derived from cortical thickness organized according to DKT atlas for HC group in OASIS-3 dataset.
     h) C_OASIS.pt: normalized anatomical covariance matrix (max eigenvalue = 1) derived from cortical thickness organized according to DKT atlas for HC and AD+ groups in OASIS-3 dataset.
     i) CT_OASIS.xlsx: this file contains the IDs for all individuals in OASIS-3, cortical thickness data and diagnosis information. 
     
     
6. Demonstrations:
     a) transfer_demo_FTDC.ipynb: This jupyter notebook demonstrates the transference of VNN models trained on FTDC datasets across different resolutions of cortical thickness data. 
     b) regional_profile_demo.ipynb: This jupyter notebook demonstrates (i) the evaluation of regional profiles associated with the robustness of observing significantly elevated regional               residuals in AD+ group relative to HC group in OASIS-3, where the robustness is evaluated across 100 VNN models trained on the HC group of any of the four datasets: FTDC100, FTDC300, FTDC500, OASIS-3, and (ii) the association between regional residuals and eigenvectors/principal components of the anatomical covariance matrix from OASIS-3. 
     Packages used in the demonstrations:
     pandas==1.1.3
     numpy==1.19.2
     torch==1.11.0+cu113
     utils==3.6.3
     base==3.6.3
     fsbrain==0.5.3 (R package)
     matplotlib==3.3.2
     re==2.2.1
     seaborn==0.11.0
     statsmodels.api==0.13.3
     nibabel==3.2.1
     
7.delta_age_code.py: This file contains the code for brain age evaluation from VNN outputs after age-bias correction. 
