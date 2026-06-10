# 🏠 Boston Housing Price Prediction using Linear Regression

A Machine Learning project that predicts housing prices using **Linear Regression**. This project demonstrates the complete ML workflow including data preprocessing, exploratory data analysis, model training, prediction, and evaluation using Python and Scikit-Learn.

---

## 📌 Project Overview

Predicting house prices is one of the most common real-world applications of Machine Learning. In this project, we use the **Boston Housing Dataset** and apply **Linear Regression** to understand the relationship between housing features and property prices.

The project is designed for beginners who want to learn how a Machine Learning model is built from scratch and deployed on real-world data.

---

## 🎯 Objectives

* Understand the fundamentals of Linear Regression
* Explore and analyze housing data
* Perform data preprocessing
* Train a Machine Learning model
* Evaluate model performance
* Predict housing prices using unseen data

---

## 🛠️ Technologies Used

| Technology       | Purpose                 |
| ---------------- | ----------------------- |
| Python           | Programming Language    |
| NumPy            | Numerical Computations  |
| Pandas           | Data Manipulation       |
| Matplotlib       | Data Visualization      |
| Scikit-Learn     | Machine Learning Model  |
| Jupyter Notebook | Development Environment |

---
## 📊 Dataset Features

The model uses housing-related attributes such as:

* CRIM – Crime Rate
* RM – Average Number of Rooms
* AGE – Age of Property
* DIS – Distance to Employment Centers
* TAX – Property Tax Rate
* PTRATIO – Pupil-Teacher Ratio
* LSTAT – Lower Status Population Percentage

### Target Variable

**MEDV** – Median Value of Owner-Occupied Homes

---

## 🔍 Exploratory Data Analysis (EDA)

The following analyses were performed:

✅ Data Inspection

✅ Missing Value Check

✅ Correlation Analysis

✅ Feature Distribution Visualization

✅ Scatter Plot Analysis

✅ Relationship Between Features and Housing Prices

---

## 🤖 Machine Learning Model

### Algorithm Used

**Linear Regression**

Linear Regression attempts to find the best-fit line that minimizes prediction error and models the relationship between input features and the target variable.

### Formula

y=\beta_0+\beta_1x_1+\beta_2x_2+\cdots+\beta_nx_n

Where:

* y = Predicted House Price
* β₀ = Intercept
* β₁...βₙ = Feature Coefficients
* x₁...xₙ = Input Features

---

## ⚙️ Model Training Process

### Step 1: Import Libraries

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt

from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
```

### Step 2: Load Dataset

```python
df = pd.read_csv("housing_dataset.csv")
```

### Step 3: Split Dataset

```python
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)
```

### Step 4: Train Model

```python
model = LinearRegression()
model.fit(X_train, y_train)
```

### Step 5: Make Predictions

```python
y_pred = model.predict(X_test)
```

---

## 📈 Model Evaluation

The model was evaluated using:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

Example:

```python
from sklearn.metrics import r2_score

score = r2_score(y_test, y_pred)
print(score)
```

---

## 📷 Sample Output

### Regression Visualization

* Scatter Plot of Actual Data
* Best Fit Regression Line
* Predicted vs Actual Values

---

## 🚀 How to Run the Project

### Clone Repository

```bash
git clone https://github.com/yourusername/Boston-Housing-Prediction.git
```

### Navigate to Project Folder

```bash
cd Boston-Housing-Prediction
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Notebook

```bash
jupyter notebook
```

---

## 📹 Project Video

A complete explanation of this project with theory and code walkthrough is available on YouTube:

🔗 **YouTube Tutorial:** *(Add Your Video Link Here)*

---

## 📚 Complete Documentation

Detailed project explanation, code walkthrough, and implementation details:

🔗 **Project Documentation:** *(Add Documentation Link Here)*

---

## 🎓 Learning Outcomes

After completing this project, you will understand:

* Fundamentals of Machine Learning
* Linear Regression Theory
* Data Preprocessing Techniques
* Feature Engineering Basics
* Model Training and Testing
* Model Evaluation Metrics
* Real-World ML Workflow

---

## 🔮 Future Improvements

* Polynomial Regression
* Ridge Regression
* Lasso Regression
* Feature Selection Techniques
* Hyperparameter Optimization
* Model Deployment using Flask/Streamlit

---

## 🤝 Contributing

Contributions are welcome!

If you'd like to improve this project:

1. Fork the repository
2. Create a new branch
3. Commit changes
4. Submit a Pull Request

---

## ⭐ Support

If you found this project helpful:

⭐ Star the repository

👍 Like the YouTube video

🔔 Follow for more Machine Learning and Data Science projects

---

## 👨‍💻 Author

**Nikita Mishra**

Computer Science Student | Data Science Enthusiast | Machine Learning Learner

📺 YouTube: https://youtu.be/yaiJFd1N8MA?si=hBsfXXn_Y07bBeYN
💼 LinkedIn: https://www.linkedin.com/in/nikita-mishra-63a829204?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app
🐙 GitHub: https://github.com/NikitaMishra04-COMMITS/Machine-learning-projects-/new/main?filename=README.md

---

### 🌟 "The best way to learn Machine Learning is by building projects and sharing your journey." 🚀
