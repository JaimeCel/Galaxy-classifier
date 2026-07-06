# Galaxy Classification

Galaxies don't exist in isolation — they live inside invisible clouds of dark matter called halos. Some galaxies sit at the centre of their halo (central), others orbit around them (satellite). This project builds a machine learning model that classifies which type a galaxy is, based on observable properties like its mass, color, and star formation rate.

---

## Overview
- Supervised classification using `scikit-learn`.  
- Features used:
  - `z_cgal` – redshift  
  - `metallicity` – 12 + log(O/H)  
  - `lmhalo` – log of halo mass  
  - `lml_r` – mass-to-light ratio  
  - `lsfr` – log of star formation rate  
  - `gr_gal` – color index (g−r)
  - `Imstellar`: mass of the galaxy
- Removed redundant or low-importance variables.

---

##  Workflow 
- Feature selection
- Balanced train/test split considering galaxies from same halos.  
- Model training with a Random Forest Classifier  
- Evaluation through metrics and feature importance 

---

##  Results
- The model achieves good accuracy distinguishing **central** vs **satellite** galaxies.  
- Most influential features: `lmhalo`, `Imstellar`.

---

##  Notes
The dataset is stored in a Google Drive folder for size issues. You can download it from this link [Dataset](https://drive.google.com/file/d/1Z9YyuZSNVbWEV0S2HT1GRVama11JNr8R/view?usp=drive_link)
