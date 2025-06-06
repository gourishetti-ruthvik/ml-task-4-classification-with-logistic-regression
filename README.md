# Logistic Regression - Breast Cancer Classification

- **AIM** : This project demonstrates how to build a **binary classification model using Logistic Regression** to classify tumors as malignant or benign using the **Breast Cancer Wisconsin dataset**.

---

## Dataset

The dataset contains features extracted from digitized images of breast mass cell nuclei. Each row represents one tumor case and includes various measurements like radius, texture, perimeter, area, smoothness, etc.

- **Target Variable**: `diagnosis`  
  - `M` = Malignant (1)  
  - `B` = Benign (0)

---

## Steps Performed

### 1. Data Preprocessing
- Loaded dataset using **Pandas**
- Dropped unnecessary columns like `id` and `Unnamed: 32`
- Converted `diagnosis` into a binary target column: `target`

### 2. Feature & Target Separation
- `X` = features  
- `y` = target labels

### 3. Train-Test Split & Feature Scaling
- Used `train_test_split` (80/20)
- Scaled features using `StandardScaler` from `sklearn.preprocessing`

### 4. Logistic Regression Model
- Used `LogisticRegression` from `sklearn.linear_model`
- Trained the model on scaled training data

### 5. Evaluation Metrics
- **Confusion Matrix**
- **Precision, Recall, F1-Score**
- **ROC Curve + AUC Score**

### 6. Threshold Tuning
- Evaluated model performance using custom thresholds (e.g. 0.6)
- Discussed trade-offs between precision and recall

### 7. Sigmoid Function
- Visualized the **Sigmoid function**, which converts log-odds to probability
- Logistic regression decision-making relies on this function

---

## Output Examples:

- **Confusion Matrix**  
  Shows True Positives, False Positives, True Negatives, False Negatives

- **ROC-AUC Curve**  
  Displays model’s ability to distinguish classes across different thresholds

---

## 🧰 Libraries Used

```bash
pandas
numpy
matplotlib
scikit-learn
