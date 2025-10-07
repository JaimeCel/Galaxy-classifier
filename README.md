# Galaxy Classification

Classify galaxies as **central** or **satellite** within dark matter halos using a **Random Forest** model.  
This project use data from a mock catalogue build from Euclid data. 

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
