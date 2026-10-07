# MNIST Handwritten Digit Recognition

## Project Overview

This project focuses on recognizing handwritten digits from 0 to 9 using the MNIST dataset.

The project compares multiple traditional Machine Learning algorithms with a Convolutional Neural Network (CNN) to determine the most suitable model for handwritten digit classification.

The complete implementation, preprocessing, visualization, model training, evaluation, and comparison are available in `MNIST.ipynb`.

---

## Dataset

The MNIST dataset contains grayscale images of handwritten digits.

- Training images: 60,000
- Testing images: 10,000
- Image size: 28 × 28 pixels
- Number of classes: 10
- Classes: Digits 0–9

The dataset is loaded using TensorFlow/Keras.

---

## Project Workflow

MNIST Dataset
↓
Data Loading
↓
Dataset Inspection
↓
Exploratory Data Analysis
↓
Image Visualization
↓
Data Preprocessing
↓
Pixel Normalization
↓
Traditional Machine Learning Models
↓
Model Comparison
↓
CNN Development
↓
Model Evaluation
↓
Best Model Selection

---

## Exploratory Data Analysis

The project includes:

- Dataset shape analysis
- Sample handwritten digit visualization
- Digit class distribution
- Pixel intensity distribution
- Individual image and pixel-value analysis

These steps help understand the structure and characteristics of the MNIST dataset before model training.

---

## Data Preprocessing

The MNIST images are prepared differently for traditional Machine Learning models and CNN.

### Traditional Machine Learning

The 28 × 28 images are flattened into 784 features.

Pixel values are normalized from the range:

0 – 255

to:

0 – 1

### CNN

The original spatial structure of the image is preserved using the shape:

28 × 28 × 1

This allows the CNN to learn spatial patterns such as edges, curves, and shapes.

---

## Machine Learning Models

The following traditional Machine Learning algorithms were implemented:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Support Vector Machine (SVM)
4. Decision Tree
5. Random Forest

A Convolutional Neural Network was then developed using TensorFlow/Keras.

---

## Model Performance

The traditional Machine Learning models were evaluated using accuracy, precision, recall, and F1-score.

| Model | Accuracy |
|---|---:|
| Logistic Regression | 92.61% |
| KNN | 96.88% |
| SVM | 97.92% |
| Decision Tree | 87.54% |
| Random Forest | 97.04% |
| CNN | 99.05% |

The CNN achieved the highest test accuracy among the implemented models.

---

## Best Model: Convolutional Neural Network

The Convolutional Neural Network achieved a test accuracy of approximately **99.05%**.

### CNN Architecture

Input: 28 × 28 × 1
↓
Convolutional Layer
↓
Max Pooling
↓
Convolutional Layer
↓
Max Pooling
↓
Flatten
↓
Dense Layer
↓
Dropout
↓
Output Layer

### Why CNN Performed Best

CNN is particularly suitable for image classification because it preserves the spatial structure of images and automatically learns important visual features.

The CNN can learn patterns such as:

- Edges
- Corners
- Curves
- Shapes
- Digit patterns

---

## Why CNN Instead of Traditional Machine Learning?

Traditional Machine Learning models treat each image as a list of 784 pixel values.

When the image is flattened, the spatial relationship between neighboring pixels is lost.

CNN processes the image in its original 28 × 28 form, preserving spatial information and automatically learning meaningful visual features.

Therefore, CNN is well suited for handwritten digit image classification.

---

## Technologies Used

### Programming Language

- Python

### Data Processing

- NumPy
- Pandas

### Data Visualization

- Matplotlib
- Seaborn

### Machine Learning

- Scikit-learn

### Deep Learning

- TensorFlow
- Keras

### Development Environment

- Jupyter Notebook

---

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Classification Report
- Confusion Matrix

---

## Model Comparison

The traditional Machine Learning models produced the following results:

- Logistic Regression provides a fast baseline.
- KNN performs well but can be computationally expensive during prediction.
- SVM provides excellent classification performance.
- Decision Tree is simple and interpretable but produces lower accuracy.
- Random Forest improves upon a single Decision Tree through ensemble learning.

The traditional models require the images to be flattened into 784 features.

The CNN preserves the original image structure and automatically learns relevant image features.

---

## Key Learning Outcomes

Through this project, I gained practical experience in:

- Image classification
- Exploratory Data Analysis
- Data preprocessing
- Feature transformation
- Machine Learning classification
- Deep Learning
- CNN architecture
- Model evaluation
- Model comparison
- Python-based data science workflow

---

## Challenges Faced

During the development of this project, several challenges were addressed:

- Understanding image data instead of traditional tabular data.
- Converting images into the correct format for different Machine Learning algorithms.
- Preparing separate preprocessing approaches for traditional Machine Learning models and CNN.
- Managing computational resources while training deep learning models.
- Selecting appropriate evaluation metrics.
- Comparing multiple algorithms using the same testing dataset.
- Understanding the architecture and working principles of Convolutional Neural Networks.

These challenges were addressed through appropriate preprocessing, model selection, and systematic evaluation.

---

## Project Structure

```text
MNIST-Handwritten-Digit-Recognition/
│
├── MNIST.ipynb
├── README.md
└── requirements.txt
