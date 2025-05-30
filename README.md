# AIMLTask4
# Binary Classification using Logistic Regression

## Project Description
The project illustrates the development of a binary classifier via Logistic Regression using the Scikit-learn library in Python. The model is used to predict if a tumor is malignant or benign from a dataset based on its features.

## Dataset
- The dataset is presumed to be a CSV file called `data.csv`.
- The target column is `diagnosis` with two classes:
- `M` for malignant (mapped to 1)
- `B` for benign (mapped to 0)
- Missing values are present in the dataset, which are processed in preprocessing.

## Tools & Libraries
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Steps Performed
1. **Data Loading:** Import the dataset from `data.csv`.
2. **Preprocessing:**
   - Remove columns with all missing values.
- Map target labels to binary values.  
   - Impute missing values with column means.  
   - Drop irrelevant columns (e.g., `id`).  
   - Split data into train and test sets (80/20 split).  
   - Standardize features using `StandardScaler`.
3. **Model Training:** Train a Logistic Regression model on the training data.
4. **Evaluation:**
- Create confusion matrix.
- Compute precision, recall, F1-score, and ROC-AUC.
- Plot the ROC curve.
5. **Threshold Tuning:** Illustrate how the classification threshold influences precision and recall.
6. **Sigmoid Function:** Illustrate and describe the sigmoid activation function of Logistic Regression.

## How to Run
1. Place your `data.csv` file inside the working directory (e.g., `/content/` on Google Colab).
2. Execute the Python code or notebook.
3. Inspect printed metrics and plots for model assessment.

## Notes
- Logistic Regression doesn't support missing values inherently, so imputation is required.
- Tuning the threshold can be used to balance recall and precision based on application requirements.
- The sigmoid function transforms model outputs into probabilities ranging from 0 to 1.

## References
- [Scikit-learn Logistic Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
- [ROC Curve and AUC](https://en.wikipedia.org/wiki/Receiver_operating_characteristic)
- [Handling Missing Data in Scikit-learn](https://scikit-learn.org/stable/modules/impute.html)

---

