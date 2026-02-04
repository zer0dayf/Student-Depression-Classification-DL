# Student Depression Prediction via Deep Learning

This repository features a Deep Learning project designed to predict depression status among students by analyzing demographic data, academic performance, and lifestyle habits.

## 📊 Project Overview
Mental health in academic environments is a critical concern. This project utilizes the **Student Depression Dataset** to build an Artificial Neural Network (ANN) that identifies potential depression markers with high accuracy.

The core objective was to explore how metrics like Academic Pressure, Study Satisfaction, and Sleep Duration correlate with mental well-being.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Frameworks:** TensorFlow / Keras
* **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib
* **Environment:** Google Colab / Jupyter Notebook

## 🧬 Dataset & Preprocessing
The dataset consists of 27,001 entries with 18 features (e.g., CGPA, Financial Stress, Family History).
* **Data Cleaning:** Removed duplicates and handled missing values.
* **Feature Engineering:** Categorical variables were encoded, and irrelevant columns (like IDs) were dropped.
* **Normalization:** Features were scaled using `MinMaxScaler` for optimal neural network convergence.

## 🧠 Model Architecture (Experiment 5 - Best Fit)
After iterative testing, the final model was built using a **Sequential API**:
* **Input Layer:** Matches the feature dimensions of the preprocessed dataset.
* **Hidden Layers:** Multiple Dense layers with `ReLU` activation.
* **Regularization:** Integrated **Dropout** layers to prevent overfitting and improve generalization.
* **Output Layer:** Single neuron with `Sigmoid` activation for binary classification.
* **Optimizer:** `Adam` (with tuned learning rates).

## 📈 Performance & Results
The model successfully captured the complex patterns of student psychology, achieving the following metrics:
* **Validation Accuracy:** ~84.00%
* **Test Accuracy:** **85.29%**
* **Test Loss:** 0.34

> **Note:** The results suggest that even with simple metrics like sleep duration and study hours, the model provides a robust baseline for mental health screening.

## 🚀 Installation & Usage
1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/student-depression-dl.git](https://github.com/yourusername/student-depression-dl.git)
2. Install dependencies:
 ```bash
    pip install -r requirements.txt

3. Run the notebook located in the notebooks/ directory.

Developed by: [Öner Efe Güngör]
