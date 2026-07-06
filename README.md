# Galaxy Classification

Galaxies don't exist in isolation — they live inside invisible clouds of dark matter called halos. Some galaxies sit at the centre of their halo (central), others orbit around them (satellite). This project builds a machine learning model that classifies which type a galaxy is, based on observable properties like its mass, color, and star formation rate.

---

## Workflow

- **Halo-aware train/test split** — galaxies from the same halo are never split across sets, preventing data leakage
- **Random Forest classifier** with hyperparameter tuning via `RandomizedSearchCV` (20 combinations, 3-fold cross-validation)
- Evaluation through classification metrics, confusion matrix, and ROC curve
- Feature importance analysis

---

## Results

ROC-AUC of $\mathbf{0.98}$, precision and recall above $0.94$ for both classes.  
The most influential features are halo mass $\log_{10}(M_\mathrm{halo})$ and stellar mass $\log_{10}(M_*)$, which aligns with physical expectations — more massive halos host more satellites, and more massive galaxies tend to be centrals.

---

## Requirements

```bash
pip install pandas scikit-learn matplotlib seaborn
```

---

## Data

Mock catalogue built from Euclid data, available via [CosmoHub](https://cosmohub.pic.es/).  
A copy is available [here](https://drive.google.com/uc?id=1Z9YyuZSNVbWEV0S2HT1GRVama11JNr8R) (large file — use `gdown` to download).
