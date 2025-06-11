# 🔬 Gamma vs Hadron Classification using Random Forest

This project applies a machine learning pipeline using a Random Forest Classifier to distinguish between **gamma** and **hadron** signals from the MAGIC gamma telescope dataset.

## 📚 Project Overview

The notebook includes the following steps:

1. **Data Loading & Understanding**  
   - Load and inspect the MAGIC dataset.
   - Convert class labels from `g`/`h` to `1`/`0`.

2. **Data Preprocessing**  
   - Handle missing values (if any).
   - Encode labels and clean data.

3. **Exploratory Data Analysis (EDA)**  
   - Visualizations to understand feature distributions and relationships.

4. **Modeling**  
   - Apply a `RandomForestClassifier`.
   - Tune parameters using `GridSearchCV`.

5. **Evaluation**  
   - Accuracy, Precision, Recall, F1-Score.
   - Confusion Matrix and classification report.

## ⚙️ Tools & Libraries

- Python 🐍
- Pandas, NumPy
- Seaborn & Matplotlib
- scikit-learn (sklearn)
- Jupyter Notebook

## 🧠 Model Performance Summary
## 🔍 Precision

- **Class 0 (Hadron)**: **0.88**  
  → When the model predicted class 0, it was correct **88%** of the time.

- **Class 1 (Gamma)**: **0.84**  
  → When the model predicted class 1, it was correct **84%** of the time.

## 🔁 Recall

- **Class 0 (Hadron)**: **0.84**  
  → The model correctly identified **84%** of actual class 0 instances.

- **Class 1 (Gamma)**: **0.89**  
  → The model correctly identified **89%** of actual class 1 instances.

## ⚖️ F1-Score

- **Class 0 (Hadron)**: **0.86**  
  → Shows a good balance between precision and recall.

- **Class 1 (Gamma)**: **0.87**  
  → Slightly higher, indicating slightly better detection of gamma events.

## 📌 Support

- **Class 0 (Hadron)**: 2007 instances  
- **Class 1 (Gamma)**: 2006 instances  

## ✅ Accuracy

- **Overall Accuracy**: **0.86**  
  → The model correctly predicted the class for **86%** of all instances.

---

## 🔢 Averages

- **Macro Average** (equal weight to each class):
  - Precision: 0.86
  - Recall: 0.86
  - F1-Score: 0.86

- **Weighted Average** (accounts for support/class size):
  - Precision: 0.86
  - Recall: 0.86
  - F1-Score: 0.86

---

## 📝 Summary

The **Random Forest classifier** achieved an overall accuracy of **86.2%**, with the number of estimators tuned to **200**. The model shows:

- A **strong balance** between precision and recall across both classes.
- Slightly **better recall** in detecting **gamma events (class 1)** at **88.8%**, which could be valuable depending on the scientific goal (e.g., detecting more gamma rays).
- **Balanced F1-scores**, indicating stable performance across both classes.

---

## 📌 Final Note

✅ *This experiment shows that using physical properties of telescope signals, machine learning—especially Random Forest—can effectively distinguish between gamma and hadron particles with high accuracy.*

🔧 *With proper preprocessing, data balancing, and hyperparameter tuning, we can enhance model reliability and achieve insightful scientific classification.*

## 📁 Files

- `magic04.data` – Dataset file (external(kaggel), not included here)
- `Gamma_Classifier_RF.ipynb` – Main notebook with full analysis
- `README.md` – Project documentation


👩‍💻 Author
Shaimaa Alazazy
GitHub: My GitHub Profile

