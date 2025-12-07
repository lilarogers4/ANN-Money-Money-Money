# 💸 MONEY, MONEY, MONEY  
*A multi-model exploration of exchange rate prediction using machine learning, deep learning, and engineered financial indicators.*

---

## 📌 Overview  
This project investigates whether machine-learning models can reliably predict **exchange-rate direction** using both price-based technical indicators and macro-aligned monthly features.  
It compares several modelling strategies — from simple baselines to deep recurrent networks — and evaluates performance across synthetic and real datasets.

The notebook is structured as a sequence of modelling experiments, each building toward a deeper understanding of what drives currency movement and how difficult it is to capture with ML.

---

## 📂 Notebook Structure

### **1. Data Loading and Initial Preparation**  
- Importing and cleaning raw exchange-rate data  
- Aligning timestamps and constructing supervised learning labels  
- Preparing training / validation / test splits  

---

### **2. Feature Engineering — Technical Indicators**  
Creation of price-based features commonly used in quantitative finance, including:  
- Moving averages  
- Momentum indicators  
- Rolling volatility  
- Normalized returns  

These form the input space for initial modelling attempts.

---

### **3. Logistic Regression Model**  
First modelling baseline to determine whether **linear separability** exists in directional movements.  
Evaluated using:  
- Accuracy  
- AUC  
- Confusion matrix  

This serves as a sanity check before more complex models.

---

### **4. LSTM Model for Directional Prediction**  
A recurrent neural network is trained on sequential windows of price features to test whether temporal dependencies improve forecasting.  
Covers:  
- Data windowing  
- Model architecture  
- Training vs. validation performance  
- Direction-prediction accuracy  

---

### **5. Random Guesser (Baseline)**  
A benchmark model that predicts direction randomly.  
Its purpose is to quantify whether ML models are **actually adding signal** or merely noise.

---

### **6. Old Model Iterations**  
Archived experiments using:  
- Pure price-based features  
- Monthly macro-aligned features  
- Mixed feature sets  

Useful for comparing how design choices influence predictability.

---

### **7. Advanced Feature Engineering & Multi-Approach LSTM Testing (Synthetic Data)**  
Synthetic datasets are used to:  
- Stress-test models  
- Validate pipeline logic  
- Control complexity and noise  

Multiple LSTM configurations are explored to understand sensitivity to feature design.

---

### **8. Real Data Testing and Evaluation**  
Final evaluation using real-world exchange-rate data.  
Includes:  
- Accuracy analysis  
- Prediction vs. actual plots  
- Model stability checks  
- Observations about forecasting difficulty in FX markets  

---

## 🚀 How to Run the Notebook  
Install dependencies:

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow
