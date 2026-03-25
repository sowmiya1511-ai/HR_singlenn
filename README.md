**Single Neuron Model for Employee Attrition Prediction**

**Overview**

This project implements a Single Neuron Model(equivalent to Logistic Regression) to predict whether an employee will leave a company.

In neural network terms, this model represents:

* One neuron
* Linear combination of inputs
* Sigmoid activation function


**Model Intuition**

The model behaves like a **single artificial neuron**:
z = w1x1 + w2x2 + ... + wn xn + b

Then applies an activation function:
ŷ = sigmoid(z)
* Output (ŷ) is a probability between **0 and 1**
* If ŷ > 0.5 → Employee leaves
* Else → Employee stays

 **Dataset**

The dataset (`HR_dataset.csv`) contains employee features such as:

* Satisfaction level
* Last evaluation
* Number of projects
* Average monthly hours
* Time spent at company
* Work accidents
* Promotion in last 5 years
* Department
* Salary
* Target: `left`

---

**Technologies Used**

* Python
* Pandas
* Scikit-learn
* Jupyter Notebook

**Workflow**

### 1. Data Preprocessing

* Loaded dataset using Pandas
* Converted categorical features (`Department`, `salary`) using one-hot encoding

### 2. Feature & Target Split

* Input features → all columns except `left`
* Output → `left`

### 3. Train-Test Split

* 80% training
* 20% testing

### 4. Model Training

* Used Logistic Regression (acts as a **single neuron**)
* Trained using gradient-based optimization

### 5. Evaluation

* Accuracy achieved: **~79%**

**Why "Single Neuron"?**

Logistic Regression is equivalent to:

* A neural network with:

  * **No hidden layers**
  * **One neuron**
  * **Sigmoid activation**

This makes it the **simplest form of a neural network**.

 **Results**

* Accuracy: **0.791 (~79%)**
* Demonstrates how a single neuron can perform binary classification

**How to Run**

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
pip install pandas scikit-learn
jupyter notebook
```
