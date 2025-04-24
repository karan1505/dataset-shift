# MCARS (Missing Completely At Random Shift) Summary

This notebook demonstrates **MCARS**, a rejection pattern where data is randomly excluded from the training set, regardless of its feature or label values.

### Dataset
- Loan Prediction dataset
- Target: `Loan_Status` (Y/N)

### Simulation
- Drop 50% of training set samples randomly

### Models
- Random Forest on full data
- Random Forest on MCARS-reduced data

### Visuals
- Label distribution before and after MCARS
- Accuracy comparison bar chart
- Evaluation with classification report

### Key Takeaway
Random loss of training data impacts performance and emphasizes the need for robust modeling and data redundancy.
