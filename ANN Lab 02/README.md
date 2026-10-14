# Logistic Regression on 2 Datasets (Gradio + Flask)

## What is in this folder
| File | What it is |
|---|---|
| logistic_regression.ipynb | Main notebook (code, graphs, Gradio UI, Flask UI) |
| diabetes.csv | Dataset 1: predicts diabetes (1 = Yes, 0 = No) |
| cancer.csv | Dataset 2: predicts tumor type (1 = Benign, 0 = Malignant) |
| README.md | This file |

## Datasets
1. Diabetes (Pima Indians): 768 rows, 8 features, target = Outcome
2. Breast Cancer (Wisconsin): 569 rows, 5 features, target = target

## How to run
1. Put all 4 files in one folder.
2. Install the libraries:
   pip install pandas scikit-learn matplotlib gradio flask jupyter
3. Open Jupyter Notebook and open logistic_regression.ipynb
4. Click Kernel > Restart & Run All (or run the cells one by one from top to bottom).

## Using your own file path
In Step 2 of the notebook, change the path. In Windows, right-click the file,
choose "Copy as path" and paste it like this:
    path1 = r"C:\Users\YourName\Downloads\diabetes.csv"
(Keep the letter r before the quotes and remove the extra quotes Windows adds.)

## UIs
- Gradio: opens inside the notebook, or at http://127.0.0.1:7860
- Flask: open http://127.0.0.1:5000 in your browser
  (Pages: /diabetes and /cancer)

## What the notebook does
1. Loads the CSV with pandas
2. Draws a bar graph of the classes (matplotlib)
3. Splits data 80% train / 20% test
4. Scales the data and trains LogisticRegression
5. Prints accuracy and classification report
6. Draws a confusion matrix and a feature coefficient graph
7. Builds the Gradio and Flask apps for prediction

## Results (approximate)
- Diabetes accuracy: about 75%
- Breast Cancer accuracy: about 94%

## Test values
- Diabetes: 6, 148, 72, 35, 0, 33.6, 0.627, 50 -> Diabetic
- Cancer: 20, 20, 130, 1200, 0.1 -> Malignant

## Problems?
- "Address already in use" in Flask: restart the kernel or change port=5000 to port=5001.
- "File not found": check that the CSV files are in the same folder as the notebook, or fix the path.
