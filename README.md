📈 Exchange Rate Prediction with ANN

A lightweight ML + finance project exploring how macroeconomic variables shape currency movements.

⭐ Project Summary

This project uses an Artificial Neural Network (ANN) to predict monthly exchange rate movements using both historical prices and key macroeconomic indicators (GDP, inflation, unemployment, interest rates).
It evaluates not only how well the model forecasts the next period, but also where and when it fails — revealing structural breaks and blind spots.

🧠 Method

Clean + align macroeconomic data into daily format

Apply feature scaling, temporal interpolation, and engineered lags

Train an LSTM for:

Regression: next-month exchange rate

Classification: up/down movement

Evaluate with MAE, RMSE, accuracy, AUC

Plot divergence zones where rolling prediction error exceeds a dynamic threshold

📊 Key Feature
Divergence Time-Series Visualization

A custom plot highlights periods where the ANN consistently diverges from actual outcomes — shading these regions directly on the time axis.
This creates an interpretable, finance-friendly diagnostic for understanding model bias and instability.

▶️ Running the Notebook

Install dependencies:

pip install numpy pandas matplotlib scikit-learn tensorflow


Then open:

ANN_Money,_Money,_Money.ipynb


Run cells in order to train the model and generate plots.
