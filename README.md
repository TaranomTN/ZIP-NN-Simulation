# ZIP-NN-Simulation

## Model Comparison on Simulated Count Data

This project evaluates the performance of different statistical and machine learning models in predicting count data using simulated datasets. The goal is to compare classical and neural network-based approaches for handling zero-inflated count variables.

Models compared:
- Poisson Regression
- Classical Zero-Inflated Poisson (ZIP)
- **Poisson Neural Network**
- **ZIP Neural Network (Ours)**

---

### 📊 Evaluation Results

| Model                     | MAE   | RMSE  |
|---------------------------|-------|-------|
| Poisson Regression        | 0.820 | 1.090 |
| Classical ZIP             | 0.840 | 1.110 |
| Poisson Neural Network    | 0.838 | 1.108 |
| **ZIP Neural Network (Ours)** | **0.760** | **1.059** |

> ✅ Our proposed **ZIP Neural Network** achieves the lowest error rates across both MAE and RMSE, outperforming all baseline models.

---

### 🧠 Key Insights

- The dataset exhibits high zero-inflation, making it ideal for ZIP modeling.
- Neural networks can effectively learn complex relationships in count data.
- Combining zero-inflation modeling with deep learning improves accuracy.

---

### 📁 Files

- `zip_nn_simulation.ipynb`: Colab notebook containing simulation setup, model training, and evaluation.

---

### 🔧 Requirements

- Python 3.x
- Jupyter Notebook or Colab
- Required libraries: `pandas`, `numpy`, `scikit-learn`, `torch`, `statsmodels`

Install dependencies:
```bash
pip install pandas numpy scikit-learn torch statsmodels
```
