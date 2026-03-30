# Quark vs Gluon Jet Classification (ML4SCI GSoC 2026)

## Summary

In this project, we perform quark vs gluon jet classification  
using three datasets combined into a unified dataset.

We extract physics-based features including jet mass, width,  
pT dispersion (pTD), and multiplicity, and analyze both  
lab frame and rest frame representations.

We train Logistic Regression and Random Forest models.  
The best performance is achieved by Logistic Regression  
in the lab frame with an AUC of 0.852.

The results show that the rest frame does not provide  
a significant advantage for this feature set.

---

## Methodology

- Multi-dataset loading and validation  
- Physics-based feature engineering  
- Lorentz boost to rest frame  
- Machine learning (Logistic + Random Forest)  
- Evaluation (ROC, AUC, Confusion Matrix)  

---

## Results

- Lab Logistic AUC: 0.852  
- Lab RF AUC: 0.849  
- Rest Logistic AUC: 0.848  
- Rest RF AUC: 0.840  

---

## How to Run

### 1. Clone the Repository

git clone https://github.com/7hepratapyadav/ML4SCI-GSoC-2026.git  
cd ML4SCI-GSoC-2026  

---

### 2. Open the Notebook

You can open the notebook using:

- Jupyter Notebook  
- VS Code  
- Google Colab  

---

### 3. Dataset Setup

Upload the required dataset files:

- QG_jets.npz  
- QG_jets_1.npz  
- QG_jets_2.npz  

Place them in the same directory as the notebook:

ML4SCI-GSoC-2026/
│
├── HepsimGSoC.ipynb
├── QG_jets.npz
├── QG_jets_1.npz
├── QG_jets_2.npz

---

### 4. Run the Notebook

Run all cells sequentially:

Runtime → Run All

---

### 5. Requirements

- Python 3.13  
- numpy  
- matplotlib  
- scikit-learn  
- seaborn  

---

## Project Structure

ML4SCI-GSoC-2026/
│
├── HepsimGSoC.ipynb        (Complete pipeline)
├── README.md               (Project documentation)

---

## Notes

- Ensure dataset files are available before running  
- The notebook runs end-to-end without errors
