# 🧠 Mental Health and Stress Prevention System

A machine learning–based system to predict mental health risk (e.g., depression) using lifestyle, behavioral, and emotional patterns. It uses supervised learning, class balancing techniques, and interpretable logic for early intervention recommendations.

---

## 📈 Problem Statement

Design a system that:
- Analyzes behavioral and lifestyle patterns
- Predicts risk of mental health concerns like depression
- Provides preventive recommendations before the condition worsens

---

## 🛠️ Technologies Used

| Area              | Tools & Libraries                      |
|------------------|----------------------------------------|
| Language          | Python                                 |
| ML Libraries      | Scikit-learn, XGBoost, Imbalanced-learn|
| Data Handling     | Pandas, NumPy                          |
| Visualization     | Seaborn, Matplotlib                    |
| Interface (Optional) | Streamlit                          |
| Dataset Source    | Kaggle (Student Mental Health Dataset) |

---

## 📆 Features

- Predicts mental health risk using behavioral data
- Handles class imbalance with SMOTE
- Uses XGBoost for high-accuracy predictions
- Offers risk-level assessment messages
- Visualizes user stress patterns over time

---

## 🚀 Installation & Setup

1. Clone the repository or download the files.
2. Install dependencies:

```bash
pip install pandas numpy scikit-learn xgboost imbalanced-learn matplotlib seaborn
```

3. Open `mental_health_model.ipynb` or `mental_health_model.py` and run all cells.

4. (Optional) If using Streamlit UI:

```bash
pip install streamlit
streamlit run app.py
```

---

## 📊 Dataset

- **Name:** Student Mental Health Dataset
- **Link:** https://www.kaggle.com/datasets/rkiattisak/student-mental-health
- **Fields:** Gender, Age, Course, Year, Depression, Anxiety, Panic Attack, Seek Help

---

## 📊 Model Performance

- **Algorithm:** XGBoost Classifier
- **Accuracy:** ~95% after tuning with RandomizedSearchCV
- **Metrics:** Accuracy, Precision, Recall, Confusion Matrix

---

## 🧰 Project Structure

```
mental-health-stress-system/
├── README.md
├── mental_health_model.ipynb      # Google Colab notebook
├── mental_health_model.py         # Script version
├── app.py                         # (Optional) Streamlit interface
├── requirements.txt
├── data/
│   └── student-mental-health.csv
```

---

## 🧠 How It Works

1. Load and clean dataset
2. Encode categorical values
3. Balance dataset using SMOTE
4. Train model using XGBoost
5. Predict mental health risk level
6. Provide recommendation based on predicted class

---

## ⚠️ Risk Assessment Logic

```python
def assess_risk(prediction):
    if prediction == 1:
        return "⚠️ High risk of depression. Please seek support or professional help."
    else:
        return "✅ You're currently at low risk. Maintain healthy routines."
```

---

## 💡 Future Improvements

- Add journaling NLP sentiment analysis
- Integrate with Google Fit or wearables
- Real-time alerts and weekly reports
- Deploy as a mobile app

---

