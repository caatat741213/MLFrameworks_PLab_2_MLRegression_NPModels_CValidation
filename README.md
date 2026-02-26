# # Practical Lab 2: Multivariate Linear Regression, Non-Parametric Models and Cross-Validation (Diabetes Progression Prediction)

I use Python to predict how diabetes grows in patients using the Scikit-Learn Diabetes dataset.

## 📝 Project Objective
The goal is to build a "Screening Tool" for doctors. We want to find which model can best predict diabetes progression after one year. We check BMI and other health data.

## 🛠️ Models I Tested
I tried many different math ways to find the answer:
1. **Univariate Polynomial Regression:** Only use BMI feature (Degree 0 to 5).
2. **Multivariate Polynomial Regression:** Use all features (Degree 2 and 3).
3. **Decision Trees:** Use different depths (3 and 5).
4. **k-Nearest Neighbors (kNN):** Use different k values (5 and 15).
5. **Logistic Regression:** Change the problem to "High Risk" or "Low Risk" (Classification).

## 📊 Key Findings
* **BMI is very important:** In Part 2, BMI alone explained about 40% of the risk.
* **The "Best" Model:** For predicting the exact number, the **Simple Degree 1 (Linear)** and **Decision Tree (depth 5)** are the strongest.
* **Overfitting Warning:** I learned that complex models (like Poly Degree 3 or 5) look good in practice but fail on the real Test Set. Simple is often better!
* **Metrics:** I used **R-Squared**, **MAE**, and **MAPE** to check the "score" of each model.

## 📂 Files
* `PLab_2_MLRegression_NPModels_CValidation.ipynb`: My full code, graphs, and notes.
* `README.md`: This file.

## 💡 What I Learned
I learned that using "All Features" makes the model see the big picture, but we must be careful not to make the model too "crazy" (Overfitting). Also, "Accuracy" in Logistic Regression is different from "R-Squared" in Linear Regression!

## 🚀 How to Run this Project (Clone and Setup)

To use this project on your computer, please follow these steps in your terminal:

1. **Clone the project:**
   ```bash
   git clone [https://github.com/caatat741213/MLFrameworks_PLab_2_MLRegression_NPModels_CValidation.git]
    ```

2. **Create a Virtual Environment**
   ```bash
    python -m venv venv
    # On Windows:
    .\venv\Scripts\activate
    # On Mac/Linux:
    source venv/bin/activate
    ```

3. **Install Dependencies:**
   ```bash
    pip install -r requirements.txt
    ```   
    
---
*Created by: Chao-Chung, Liu*