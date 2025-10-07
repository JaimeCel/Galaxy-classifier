# 🌌 Galaxy Classification

Classify galaxies as **central** or **satellite** within dark matter halos using a **Random Forest** model.  
This project applies key astrophysical features to study galaxy structure and evolution.

---

## 🔭 Overview
- Supervised classification using `scikit-learn`.  
- Core features used:
  - `z_cgal` – redshift  
  - `metallicity` – 12 + log(O/H)  
  - `lmhalo` – log of halo mass  
  - `lml_r` – mass-to-light ratio  
  - `lsfr` – log of star formation rate  
  - `gr_gal` – color index (g−r)  
- Removed redundant or low-importance variables such as magnitudes and velocities.

---

## ⚙️ Workflow
1. Data cleaning and exploration  
2. Feature selection and engineering  
3. Balanced train/test split considering halo sizes  
4. Model training with a Random Forest Classifier  
5. Evaluation through accuracy and feature importance  

---

## 📊 Results
- Achieved strong accuracy distinguishing **central** vs **satellite** galaxies.  
- Most influential factors: `lmhalo`, `lsfr`, and `gr_gal`.

---

## 💻 Tools
Python • pandas • numpy • matplotlib • scikit-learn • Jupyter  

---

## 🌠 Notes
You can open the notebook directly in Jupyter or any notebook interface to explore the data, run the model, and view the visualizations interactively.
