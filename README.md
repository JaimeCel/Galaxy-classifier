# Galaxy Classification

Classify galaxies as **central** or **satellite** within dark matter halos using a **Random Forest** model.  
This project use data from a mock catalogue build from Euclid data. 

---

## Overview
- Supervised classification using `scikit-learn`.  
- Ffeatures used:
  - `z_cgal` – redshift  
  - `metallicity` – 12 + log(O/H)  
  - `lmhalo` – log of halo mass  
  - `lml_r` – mass-to-light ratio  
  - `lsfr` – log of star formation rate  
  - `gr_gal` – color index (g−r)
  - Imstellar: mass of the galaxy
- Removed redundant or low-importance variables such as magnitudes and velocities.

---

## ⚙️ Workflow 
2. Feature selection 
3. Balanced train/test split considering galaxies from same halos.  
4. Model training with a Random Forest Classifier  
5. Evaluation through metrics and feature importance  

---

## 📊 Results
- Achieved strong accuracy distinguishing **central** vs **satellite** galaxies.  
- Most influential features: `lmhalo`, `Imstellar`.

---

## 🌠 Notes
I save the data in a google drive folder. I fu want to download it i link here : https://drive.google.com/file/d/1Z9YyuZSNVbWEV0S2HT1GRVama11JNr8R/view?usp=drive_link
