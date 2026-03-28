# Linear Regression Model — Diabetes Dataset

A machine learning project that applies **Linear Regression** to the classic **Diabetes Dataset** from scikit-learn to predict disease progression one year after baseline measurements.

---

## 📋 Dataset Overview

- **Source:** `sklearn.datasets.load_diabetes()`
- **Samples:** 442 patients
- **Features:** 10 baseline variables (all mean-centered and scaled)

| Feature | Description |
|---------|-------------|
| `age` | Age in years |
| `sex` | Sex |
| `bmi` | Body Mass Index |
| `bp` | Average blood pressure |
| `s1` | TC — total serum cholesterol |
| `s2` | LDL — low-density lipoproteins |
| `s3` | HDL — high-density lipoproteins |
| `s4` | TCH — total cholesterol / HDL |
| `s5` | LTG — log of serum triglycerides level |
| `s6` | GLU — blood sugar level |

- **Target:** Quantitative measure of disease progression one year after baseline

---

## 🔧 Techniques Used

### 1. Data Loading & Exploration
- Loaded the dataset using `sklearn.datasets`
- Inspected shape, type, and description of features and target

### 2. Train-Test Split
- Split data into **70% training** and **30% testing** using `train_test_split`
- Used `random_state=42` for reproducibility

### 3. Linear Regression
- Trained a **Linear Regression** model from `sklearn.linear_model`
- Used the Ordinary Least Squares (OLS) method to find the best-fit line

### 4. Model Evaluation
- **Mean Squared Error (MSE):** Measures average squared difference between predicted and actual values
- **R² Score (Coefficient of Determination):** Measures how well the model explains the variance in the target

### 5. Visualization
- **Scatter plots** comparing actual vs. predicted values
- **Correlation heatmaps** using `seaborn` to understand feature relationships

---

## 📊 Sample Outputs

- Training set shape: `(309, 10)`
- Test set shape: `(133, 10)`
- The model predicts a continuous disease progression score for each patient.

---

## 🚀 How to Run

### Prerequisites

Install the required Python libraries:

```bash
pip install -r requirements.txt
```

### Running the Notebook

```bash
jupyter notebook "Linear_Regression_Model _Diabetes_Dataset.ipynb"
```

Or open it directly in **VS Code**, **JupyterLab**, or **Google Colab**.

---

## 📦 Requirements

```
numpy
scikit-learn
matplotlib
seaborn
jupyter
```

Install with:

```bash
pip install numpy scikit-learn matplotlib seaborn jupyter
```

---

## 📁 Project Structure

```
├── Linear_Regression_Model _Diabetes_Dataset.ipynb   # Main notebook
└── README.md                                          # Project documentation
```

---

## 📚 References

- [Scikit-learn Diabetes Dataset](https://scikit-learn.org/stable/datasets/toy_dataset.html#diabetes-dataset)
- Efron, Hastie, Johnstone & Tibshirani (2004) — *Least Angle Regression*, Annals of Statistics
