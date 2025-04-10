# Retinal_image_preprocessing
Preprocessing of retinal images for AI based artery vein segmentation of retinal image.

This repository is created as part of an "AI-based aretery vein segmentation in fundus images for vascular analysis" project. It focuses on "preprocessing retinal images" from benchmark datasets to prepare them for deep learning models, such as U-Net.

# repository structure
Retinal_image_preprocessing/
 ├── DRIVE/ # Folder containing the DRIVE dataset 
 │ ├── training/ # Training images, masks, ROI masks 
 │ ├── test/ # Testing images, ROI masks 
 ├── preprocessing_DRIVE.ipynb # Master notebook for DRIVE dataset preprocessing 
 ├── STARE/ # (Downloaded dataset - code not yet integrated) 
 ├── CHASE_DB1/ # (Downloaded dataset - code not yet integrated) 
 └── README.md # Project documentation

##  Current Status

Currently, the repository contains:
-preprocessing_DRIVE.ipynb -a notebook containing fully functional code for preprocessing the DRIVE dataset(training and test sets).

## What the Code Does

The preprocessing code performs the following tasks:

1. **Reads original retinal fundus images**from the DRIVE dataset.
2. **Applies ROI masking** (to focus only on the region of interest).
3. **Converts the image to grayscale**.
4. **Enhances contrast using CLAHE** (Contrast Limited Adaptive Histogram Equalization).
5. **Resizes all images** to a uniform shape (`512x512`).
6. **Loads and binarizes ground truth masks** (for training images).
7. Provides a **visualization utility** to compare original vs preprocessed images and masks.


## Technologies Used

- Python
- OpenCV
- NumPy
- Matplotlib
- PIL
- Jupyter Notebook
- Datasets sourced from Kaggle


## Coming Up

- Add preprocessing support for **STARE** and **CHASE_DB1** datasets.
- Implement advanced preprocessing techniques (e.g., vessel enhancement filters).
- Prepare preprocessed data for training segmentation models.


