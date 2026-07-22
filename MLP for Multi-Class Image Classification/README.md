# MLP for Multi-Class Image Classification

A complete implementation of a **Multi-Layer Perceptron (MLP)** for multi-class image classification using the **Fashion-MNIST** dataset. This project demonstrates the end-to-end workflow of building, training, evaluating, and optimizing a neural network using TensorFlow/Keras and Scikit-learn.

The objective of this experiment is not only to classify fashion images but also to understand how different hyperparameters influence the learning behaviour and generalization capability of deep neural networks.

---

## Project Overview

This experiment covers the complete deep learning pipeline:

- Dataset exploration
- Data preprocessing
- MLP model construction
- Model training
- Performance evaluation
- Hyperparameter optimization
- Visualization of learning behaviour
- Result analysis and interpretation

The implementation follows a systematic experimental approach where a baseline model is first developed and later improved through hyperparameter tuning using **Randomized Search Cross Validation**.

---

## Dataset

**Dataset:** Fashion-MNIST

Fashion-MNIST is a benchmark image classification dataset consisting of grayscale images of fashion products belonging to ten different categories.

### Dataset Characteristics

- 70,000 images
- Image Size: **28 × 28**
- Grayscale Images
- 10 Clothing Categories
- Training Images: **60,000**
- Testing Images: **10,000**

### Classes

| Label | Category |
|--------|----------|
| 0 | T-shirt / Top |
| 1 | Trouser |
| 2 | Pullover |
| 3 | Dress |
| 4 | Coat |
| 5 | Sandal |
| 6 | Shirt |
| 7 | Sneaker |
| 8 | Bag |
| 9 | Ankle Boot |

---

## Workflow

### 1. Dataset Exploration

- Loaded Fashion-MNIST dataset
- Displayed sample images
- Visualized class distribution
- Verified dataset dimensions

---

### 2. Data Preprocessing

The following preprocessing steps were performed:

- Flattened 28×28 images into 784-dimensional vectors
- Normalized pixel values to the range [0,1]
- One-hot encoded target labels
- Prepared data for neural network training

---

### 3. Model Architecture

The baseline model consists of fully connected dense layers implemented using TensorFlow/Keras.

Example architecture:

```
Input Layer (784)

↓

Dense Layer

↓

Activation Function

↓

Dropout

↓

Dense Layer

↓

Softmax Output Layer (10 Classes)
```

---

### 4. Model Training

The network was trained using:

- TensorFlow/Keras
- Backpropagation
- Categorical Crossentropy Loss
- Mini-batch Gradient Descent

Training and validation metrics were monitored throughout the learning process.

---

### 5. Model Evaluation

The trained model was evaluated using multiple classification metrics instead of relying solely on accuracy.

Evaluation metrics include:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Classification Report

---

### 6. Hyperparameter Optimization

To improve the model configuration, **RandomizedSearchCV** with **SciKeras** was used.

The following hyperparameters were explored:

- Number of Hidden Layers
- Hidden Neurons
- Learning Rate
- Optimizer
- Activation Function
- Batch Size
- Number of Epochs
- Dropout Rate

The best configuration was selected using **5-Fold Cross Validation**.

---

## Best Hyperparameters

| Hyperparameter | Value |
|---------------|------|
| Hidden Layers | 3 |
| Hidden Neurons | 128 |
| Optimizer | RMSprop |
| Learning Rate | 0.001 |
| Activation Function | Tanh |
| Batch Size | 32 |
| Epochs | 30 |
| Dropout Rate | 0.2 |

---

## Model Performance

### Optimized Model

| Metric | Score |
|---------|------|
| Cross Validation Accuracy | 88.63% |
| Testing Accuracy | 87.99% |
| Precision | 88.09% |
| Recall | 87.99% |
| F1-score | 87.99% |

---

## Visualizations

The project includes the following visualizations:

- Sample Images
- Class Distribution
- Training Accuracy vs Epoch
- Validation Accuracy vs Epoch
- Training Loss vs Epoch
- Validation Loss vs Epoch
- Confusion Matrix
- Hyperparameter Search Results
- Baseline vs Optimized Model Comparison

These visualizations help understand model convergence, learning behaviour, and prediction performance.

---

## Repository Structure

```
MLP for Multi-Class Image Classification
│
├── Figures/
│   ├── sample_images
│   ├── class_distribution
│   ├── training_accuracy
│   ├── validation_accuracy
│   ├── training_loss
│   ├── validation_loss
│   ├── confusion_matrix
│   ├── hyperparameter_search
│   └── accuracy_comparison
│
├── DL_Lab_2.ipynb
├── Experiment_2.pdf
└── README.md
```

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn
- SciKeras
- RandomizedSearchCV

---

## Key Learning Outcomes

Through this implementation, the following concepts were explored:

- Neural network architecture design
- Multi-class image classification
- Data preprocessing for deep learning
- Model evaluation using multiple metrics
- Hyperparameter optimization
- Cross-validation for model selection
- Analysis of learning curves
- Interpretation of confusion matrices
- Understanding the trade-off between model complexity and generalization

---

## Author

**Hemanth Kumar R**

B.Tech Artificial Intelligence & Data Science

Shiv Nadar University Chennai


