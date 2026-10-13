# Lab Task 2 - Linear Regression

## Student Info
- **Name:** [Your Name]
- **Roll No:** [Your Roll No]
- **Subject:** Machine Learning / Data Science
- **Lab Task:** 2

---

## About This Project

In this lab task, I implemented **Linear Regression** on two different datasets.
I also created user interfaces using **Gradio** and **Flask**.

---

## Datasets Used

### Dataset 1 - `temperature_electricity.csv`
- **Feature (X):** Temperature in Celsius
- **Target (Y):** Electricity Consumption in kWh
- **Rows:** 50
- **Description:** This dataset shows how electricity consumption changes with daily temperature.

### Dataset 2 - `car_age_price.csv`
- **Feature (X):** Car Age in Years
- **Target (Y):** Car Market Price in PKR (Thousands)
- **Rows:** 50
- **Description:** This dataset shows how car price decreases as the car gets older.

---

## Files in This Project

| File | Description |
|------|-------------|
| `linear_regression_lab2.ipynb` | Main Jupyter Notebook with all code |
| `temperature_electricity.csv` | Dataset 1 |
| `car_age_price.csv` | Dataset 2 |
| `README.md` | This file |

---

## Libraries Used

```
pandas
numpy
matplotlib
scikit-learn
gradio
flask
```

Install all libraries using:
```
pip install pandas numpy matplotlib scikit-learn gradio flask
```

---

## How to Run

1. Open **Jupyter Notebook**
2. Open the file `linear_regression_lab2.ipynb`
3. Run all cells one by one from top to bottom

### For Gradio UI:
- Run the Gradio cell
- A link will appear below the cell automatically
- Click the link to open the app

### For Flask UI:
- Run the Flask cell
- A **clickable blue link** will appear
- Click it to open `http://127.0.0.1:5000` in your browser

---

## What I Did (Steps)

1. Imported all libraries
2. Loaded Dataset 1 and Dataset 2
3. Did basic EDA (head, describe, isnull)
4. Plotted scatter graphs
5. Split data into train and test (80/20)
6. Trained Linear Regression model on both datasets
7. Evaluated using MSE and R2 Score
8. Plotted Regression Line
9. Built Gradio Interface with 2 tabs
10. Built Flask Web Interface with clickable link

---

## Results

| | Dataset 1 | Dataset 2 |
|---|---|---|
| Feature | Temperature (C) | Car Age (Years) |
| Target | Electricity (kWh) | Price (PKR Thousands) |
| Algorithm | Linear Regression | Linear Regression |
| Train/Test Split | 80% / 20% | 80% / 20% |
