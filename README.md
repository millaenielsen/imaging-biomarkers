# imaging-biomarkers
Pioneer Centre for AI at the University of Copenhagen internship project to assess the efficacy of classical and deep neuroimaging biomarkers in early Alzheimer’s Disease diagnosis. 

## The Data

The dataset for this study was sourced from the ADNI. Specifically, we used the ADNI1 Screening 1.5T subset, which includes high-quality T1-weighted brain MRIs from 503 subjects at baseline, with an average voxel resolution of 1×1×1.2 mm3. These images underwent preprocessing with FreeSurfer’s cross-sectional pipeline. The preprocessing steps included motion correction, bias field correction, affine registration to the MNI305 space, resampling to an isotropic resolution of 1 mm, and intensity normalization to a range of [0, 255].

## Repository 

This repo contains three .ipynb files. 
The file entiled classifcation.ipynb contains multiple parts the first of which is specifically for use in converting the matlab data files into a useable format, in this case numpy arrays using the h5py package. The latter part of this file works to fit XGBoost for classfication between three stages in Alzheimer's development to various models based on different subsets of the imaging data. 

The other two files are for using ResNet18-3d for feature extraction on the dataset and 
