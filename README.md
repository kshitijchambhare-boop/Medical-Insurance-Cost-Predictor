# 💰 Medical Insurance Cost Predictor

Beginner-level healthcare ML **regression** project jo predict karta hai kisi person ka medical insurance cost, uske age, BMI, smoking status, aur baaki attributes ke basis par.

## Project Structure
```
├── Medical_Insurance_Cost_Predictor.ipynb   # Main notebook (run this)
├── requirements.txt                          # Dependencies
└── README.md
```

## Setup & Run (Local Jupyter Notebook)

1. Virtual environment banao (optional but recommended):
   ```
   python -m venv venv
   venv\Scripts\activate      # Windows
   source venv/bin/activate   # Mac/Linux
   ```

2. Dependencies install karo:
   ```
   pip install -r requirements.txt
   ```

3. Jupyter Notebook start karo:
   ```
   jupyter notebook
   ```

4. Browser mein `Medical_Insurance_Cost_Predictor.ipynb` open karo aur cells ko top se bottom run karo (Run All / Shift+Enter).

## What's Inside
- Synthetic-but-realistic insurance dataset (1000 records) — koi external CSV download nahi chahiye, fully offline chalta hai
- Exploratory Data Analysis (distribution plots, smoker vs non-smoker comparison, scatter plots)
- Linear Regression + Random Forest Regressor models
- Model evaluation (MAE, RMSE, R²)
- New person prediction example

## Using a Real Dataset (Optional Upgrade)
Agar aap real-world data use karna chahte ho, Kaggle se **"Medical Cost Personal Datasets"** (`insurance.csv`) download karo aur notebook ke Section 2 mein:
```python
df = pd.read_csv("insurance.csv")
```
se replace kar do — baaki poora code same rahega kyunki column names match karte hain.

## Next Steps
- Hyperparameter tuning (GridSearchCV)
- Cross-validation
- Try Gradient Boosting / XGBoost Regressor
- Deploy as a "Insurance Cost Calculator" web app using Streamlit
