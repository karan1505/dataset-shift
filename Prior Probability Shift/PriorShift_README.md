# Prior Probability Shift Summary

This notebook demonstrates **Prior Probability Shift**, where the label distribution `P(Y)` changes between training and test sets, but the feature distributions given the label `P(X|Y)` stay the same.

### Dataset
- Breast Cancer Wisconsin dataset
- Target: `diagnosis` (Benign/Malignant)

### Simulation
- Training set: 80% Benign, 20% Malignant
- Test set: Remaining balanced data

### Models
- Random Forest
- Logistic Regression (with pipeline and scaling)
- SMOTE resampling for class balance

### Visuals
- ROC curves + AUC comparison
- Class balance before/after SMOTE
- Accuracy comparison bar chart

### Key Takeaway
Class imbalance due to shift in `P(Y)` reduces model generalization and highlights the value of class balancing techniques.
