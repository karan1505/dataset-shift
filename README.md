
# CS594 Final Project – Dataset Shift Demonstration

This repository presents a comprehensive demonstration of three distinct types of **dataset shift** in machine learning:

1. **Covariate Shift**
2. **Prior Probability Shift**
3. **Rejection Pattern (MCARS: Missing Completely At Random Shift)**

Each shift type is covered in its **own directory** with:
- An explanatory Jupyter notebook
- Visualizations and metrics
- Code cells for data simulation, modeling, and evaluation
- Dataset-specific requirements

---

## 📂 Repository Structure

```
.
├── CovariateShift/
│   ├── CovariateShift_Explained.ipynb
│   ├── requirements.txt
│   └── weatherAUS.csv
│
├── PriorProbabilityShift/
│   ├── PriorShift_Explained.ipynb
│   ├── requirements.txt
│   └── data.csv (Breast Cancer Wisconsin Dataset)
│
├── MCARS/
│   ├── MCARS_Explained.ipynb
│   ├── requirements.txt
│   └── train.csv (Loan Prediction Dataset)
│
├── DatasetShift_FinalPresentation.pptx
├── README.md
```

---

## 🧪 Shift Types Explained

### 1️⃣ Covariate Shift
- **What Changes?** Feature distribution `P(X)`
- **What Stays?** Conditional distribution `P(Y|X)`
- **Example:** Model trained on sunny weather fails on rainy conditions.

### 2️⃣ Prior Probability Shift
- **What Changes?** Label distribution `P(Y)`
- **What Stays?** Feature distribution given label `P(X|Y)`
- **Example:** Model trained on mostly benign tumors is tested on balanced classes.

### 3️⃣ Rejection Pattern – MCARS
- **What Changes?** Sample inclusion, randomly dropped (MCAR)
- **Effect:** Joint distribution `P(X, Y)` is shifted
- **Example:** Training set randomly loses 50% of samples.

---

## 💻 Running the Notebooks

Each folder contains:
- Its own notebook (with embedded explanations)
- A specific dataset file
- A `requirements.txt` file for dependencies

To run a notebook:
1. `cd` into the desired shift directory
2. Create a virtual environment (optional but recommended)
3. Install dependencies: `pip install -r requirements.txt`
4. Launch Jupyter Notebook and open the `.ipynb` file

---

## 📊 Deliverables

- ✅ Fully explained notebooks with markdown + visuals
- ✅ ROC curves, confusion matrices, and accuracy charts
- ✅ A slide deck: `DatasetShift_FinalPresentation.pptx`
- ✅ This README for repository documentation

---

## 👨‍💻 Authors

- **Karan Sreedhar**
- **Ravi Teja Ravella**
- **Srinath Ganesh**

> CS594 – Responsible AI Engineering  
> University of Illinois at Chicago

---

## 📄 License

This project is for educational purposes only under the UIC CS594 course requirements.
