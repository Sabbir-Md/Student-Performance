# 🎓 Student Performance Prediction (Pass/Fail using ML)

This project uses **Machine Learning (Random Forest Classifier)** to predict whether a student will **pass or fail** the final exam based on their background, study habits, past grades, and other factors.

The dataset is based on the well-known **Student Performance** dataset (UCI / Kaggle) and includes information such as:

- Demographics  
- Family and social background  
- Study time, support, absences  
- First and second period grades (`G1`, `G2`)  
- Final grade (`G3`)

---

## 📌 Project Goals

- Build a **binary classifier** to predict if a student will **pass (1)** or **fail (0)**.
- Analyze which **features are most important** for prediction.
- Provide a simple **interface** to:
  - Predict performance for a new student (CLI and Streamlit web app).
  - Visualize feature importance.

---

## 📂 Dataset

- File used: `student_data.csv`
- Each row = one student.
- Original final grade: **`G3`** (0–20)
- Target label created:

```python
passed = 1 if G3 >= 10 else 0
passed = 0 if G3 < 10
