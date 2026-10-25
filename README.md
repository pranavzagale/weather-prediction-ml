# Smart Weather Forecasting and Rain Prediction System

Mini Project, Machine Learning Laboratory (CS3201L)
JSPM's Rajarshi Shahu College of Engineering, Pune | TY Div A | 2026-27

## About the Project
This project studies daily weather data (temperature, humidity, pressure and wind speed), finds the hidden weather type behind it, detects unusual weather weeks, and predicts whether it will rain tomorrow.

## What it does
1. **Data cleaning:** fills missing values with the median and converts rain Yes/No to 1/0.
2. **K-Means clustering:** groups days into 3 weather types: Sunny, Cloudy, Rainy.
3. **Hidden Markov Model (HMM):** builds the starting (pi), transition (A) and emission (B) probabilities.
4. **Forward algorithm:** finds how likely each week is and flags unusual weeks.
5. **Viterbi algorithm:** finds the most likely weather sequence for each week and measures accuracy.
6. **Rain prediction:** compares Logistic Regression, Decision Tree and AdaBoost using accuracy, precision, recall and F1-score.
7. **Graphs:** cluster plot, HMM matrices, actual vs decoded weather, week likelihood, model comparison.

## Technologies Used
- Python 3
- NumPy, Pandas, Matplotlib
- scikit-learn

## Dataset
The code reads a file named `weather.csv` with these columns:

| Column | Meaning |
|--------|---------|
| temperature | Average temperature (°C) |
| humidity | Humidity (%) |
| pressure | Air pressure (hPa) |
| wind | Wind speed (km/h) |
| rain | Did it rain? (yes/no or 1/0) |

If `weather.csv` is not found, the code automatically generates sample weather data, so it runs without any dataset.

## How to Run
**Option 1: Google Colab (easiest)**
1. Open `ML_PROJECT.ipynb` in Google Colab.
2. Click **Runtime > Run all**.

**Option 2: On your computer**
```
pip install numpy pandas matplotlib scikit-learn
python weather_project.py
```

## Files in this Repository
- `ML_PROJECT.ipynb`: full project code
- `ML_PROJECT.ipynb - Colab.pdf`: code with outputs
- `README.md`: project description

## Author
Name: PRANAV ZAGALE
Roll No: CS3127
Class: TY Div A
