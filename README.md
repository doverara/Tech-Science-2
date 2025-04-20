# Tech-Science-2: Classifying Galaxies by Subclass Using Machine Learning

## Project Description  
We investigate whether photometric magnitudes, color indices, and redshift from the Sloan Digital Sky Survey (SDSS DR18) can be used to classify galaxies into physical subclasses (STARBURST, STARFORMING, AGN, BROADLINE, OTHER) using machine learning models such as SVM and Random Forest.

## Research Question  
Can observable galaxy properties be leveraged to accurately predict galaxy subclasses?

## Methods Overview  
- **Data Preprocessing:** Skipped commented lines, dropped missing values, grouped rare subclasses into `OTHER`, and scaled features for SVM.  
- **Modeling:**  
  - **SVM:** Linear and RBF kernels, `class_weight='balanced'`, hyperparameter tuning via GridSearchCV.  
  - **Random Forest:** 100 trees, `class_weight='balanced'`, feature importance analysis.  
- **Evaluation:** 70/30 train–test split, confusion matrices, classification reports, and test accuracy comparison.

## Key Findings  
- **SVM Test Accuracy:** 0.62  
- **Random Forest Test Accuracy:** 0.80  
- SVM performs well on common classes (STARBURST, STARFORMING) but struggles with rare ones.  
- Random Forest captures nonlinear interactions and handles imbalance more robustly.

## Team Contributions  
- **Araynah D.:** Data ingestion, SVM modeling and evaluation, preprocessing and visualization code.  
- **Palmer W.:** Confusion matrix and classification report analysis, slide preparation.  
- **Katrina S.:** Feature importance extraction, code documentation, heatmap.  
- **Yihan W.:** Data visualization (distribution and sky maps), README and slides formatting.

## Future Work  
- Apply oversampling techniques (e.g., SMOTE) for minority classes.  
- Explore dimensionality reduction (PCA) or feature selection to reduce feature overlap.  
- Further hyperparameter tuning and testing of additional models.

## References  
- Sloan Digital Sky Survey (SDSS DR18) — https://skyserver.sdss.org/dr18  
- scikit-learn documentation — https://scikit-learn.org  
- OpenAI, ChatGPT (code snippets), April 2025
