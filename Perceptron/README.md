# Perceptron from Scratch | Deep Learning Lab 1

Implementation of a **Single Layer Perceptron** from scratch using Python as part of the Deep Learning Laboratory. This experiment focuses on understanding the fundamentals of linear binary classification without relying on high-level deep learning frameworks.

---

## Objective

The primary objectives of this experiment are to:

- Understand the architecture of a Single Layer Perceptron.
- Implement the Perceptron Learning Algorithm from scratch.
- Study the effect of feature normalization on convergence.
- Compare the custom implementation with Scikit-learn's Perceptron.
- Analyze the limitations of a Single Layer Perceptron on non-linearly separable data.

---

## Dataset

**Banknote Authentication Dataset**

The dataset contains features extracted from images of genuine and forged banknotes.

### Features

| Feature | Description |
|----------|-------------|
| Variance | Wavelet transformed image variance |
| Skewness | Wavelet transformed image skewness |
| Curtosis | Wavelet transformed image kurtosis |
| Entropy | Image entropy |
| Class | Genuine (0) / Forged (1) |

---

## Experiment Workflow

```
Dataset
      │
      ▼
Data Exploration
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Feature Normalization
      │
      ▼
Train-Test Split
      │
      ▼
Perceptron Implementation
      │
      ▼
Model Training
      │
      ▼
Performance Evaluation
      │
      ▼
Visualization & Analysis
```

---

## Implementation Details

The Perceptron was implemented completely from scratch using **NumPy**.

Implemented components include:

- Weight Initialization
- Bias Initialization
- Forward Propagation
- Step Activation Function
- Perceptron Learning Rule
- Weight Updates
- Bias Updates
- Epoch-wise Training
- Prediction
- Model Evaluation

No deep learning libraries such as TensorFlow or PyTorch were used for the core implementation.

---

## Exploratory Data Analysis

The following analyses were performed before training:

- Dataset Inspection
- Missing Value Analysis
- Statistical Summary
- Feature Histograms
- Correlation Heatmap
- Scatter Plot Matrix
- Boxplots

These analyses helped understand feature distributions and relationships before model training.

---

## Performance Evaluation

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

Training convergence was also analyzed using epoch-wise error tracking.

---

## Additional Experiments

This experiment also includes:

- Feature Normalization Analysis
- Step vs Sigmoid Activation Comparison
- Scikit-learn Perceptron Comparison
- XOR Problem Visualization
- Decision Boundary Visualization
- Learning Rate Comparison
- Weight Evolution
- Bias Evolution

---

## Repository Structure

```
Perceptron/
│
├── Figures/
│   ├── correlation_heatmap.pdf
│   ├── confusionmatrix.pdf
│   ├── decision_boundary.pdf
│   ├── scatter_plot_matrix.pdf
│   ├── training_error.eps
│   ├── normalization_effect.eps
│   ├── learning_rate_comparison.eps
│   ├── sklearn_comparison.eps
│   ├── xor_problem.eps
│   └── ...
│
├── DL_Lab_1.ipynb
├── Experiment_1.pdf
├── data_banknote_authentication.txt
└── README.md
```

---

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## Key Learning Outcomes

Through this experiment, I learned:

- How a Perceptron performs binary classification.
- The mathematics behind weight and bias updates.
- Why feature normalization improves convergence.
- The importance of activation functions.
- Why Single Layer Perceptrons fail on non-linearly separable problems such as XOR.
- How classical neural networks compare with Scikit-learn implementations.

---

## Results

The custom Perceptron successfully learned a linear decision boundary for the Banknote Authentication dataset and achieved high classification performance after proper feature normalization. The additional visualizations provided insights into the learning dynamics and convergence behaviour throughout training.

---


## Author

**Hemanth Kumar R**

B.Tech Artificial Intelligence & Data Science

Shiv Nadar University Chennai
