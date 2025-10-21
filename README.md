# 🎓 Linear Regression — From Scratch (Python + NumPy)

A simple, educational implementation of **Linear Regression** built entirely from scratch using **Python** and **NumPy** — without relying on any pre-built machine learning libraries like scikit-learn.

The goal is to **understand how Linear Regression actually works** under the hood 💡

---

## 🧩 Project Idea

Linear Regression tries to find the **best-fitting straight line** that represents the relationship between input `X` and output `y`.

In simple terms, it learns this equation:



y = w * X + b


Where:
- `w` → Weight (slope)
- `b` → Bias (intercept)

The main objective is to minimize the error between the predicted and true values.

---

## ⚙️ Implementation Steps

### 1️⃣ Create the Class
A custom class `LinearRegression` was created with three main methods:
- `__init__()` → sets the learning rate and number of iterations  
- `fit()` → trains the model using gradient descent  
- `predict()` → makes predictions after training  

### 2️⃣ How Learning Happens (Gradient Descent)
The model starts with random values for `w` and `b`, then:
1. Predicts `y` values.
2. Calculates the difference between predictions and real values (error).
3. Adjusts `w` and `b` in the direction that reduces the error.
4. Repeats the process thousands of times until the loss becomes minimal.

This repetitive adjustment process is called **Gradient Descent**, which is the heart of how most ML models “learn”.

---

## 🧠 Why Build It From Scratch?

When you code a model manually, you understand that it’s not magic — it’s just:
- simple math operations,
- repeated optimizations,
- and small improvements every iteration.

That’s what turns numbers into a “learning” model.

This understanding separates someone who *uses* ML tools from someone who truly *knows* what’s happening behind the scenes.

---

## 🧪 Example Used

A simple dataset was used for demonstration:

```python
X = np.array([[1], [2], [3], [4], [5]])
y = np.array([2, 4, 6, 8, 10])  # True relation: y = 2x
