# Covariate Shift Summary

This notebook demonstrates **Covariate Shift**, where the distribution of input features `P(X)` changes between training and test sets, but the relationship `P(Y|X)` remains the same.

### Dataset
- Australian Weather dataset
- Target: `RainTomorrow` (Yes/No)

### Simulation
- Train only on samples with `RainToday == No` (sunny)
- Test on samples with `RainToday == Yes` (rainy)

### Models
- Random Forest
- Logistic Regression (with and without scaling/pipeline)
- Drop vs Impute comparison

### Visuals
- PCA projection of input space
- Confusion matrix (normalized + labeled)
- Accuracy comparison bar chart

### Key Takeaway
Covariate shift can severely impact model performance when unseen feature distributions occur during testing.
