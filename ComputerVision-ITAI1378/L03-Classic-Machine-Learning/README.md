# L03 - Computer Vision with Classical Machine Learning

## Course Information

- Student: Ali Abed
- Course: ITAI 1378 - Computer Vision
- Institution: Houston Community College

## Problem Statement

This project explores how classical machine learning
algorithms can be used for image classification and
facial recognition without relying on deep learning.

## Approach

The project implements a classical machine learning
pipeline using image feature extraction, model
training, validation, and performance evaluation.

The main steps include:

- Dataset loading and exploration
- Training, validation, and test data splitting
- HOG and LBP feature extraction
- Support Vector Machine (SVM) classification
- Random Forest classification
- Overfitting analysis
- Five-fold cross-validation
- Model selection and evaluation

## Dataset

This project uses the Olivetti Faces dataset.

| Dataset Information | Value |
|---|---|
| Total images | 400 |
| Number of individuals | 40 |
| Images per individual | 10 |
| Image dimensions | 64 x 64 |
| Training images | 240 |
| Validation images | 80 |
| Test images | 80 |

The dataset is available through Scikit-learn:

https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_olivetti_faces.html

It can be loaded using:

```python
from sklearn.datasets import fetch_olivetti_faces

faces = fetch_olivetti_faces(
    shuffle=True,
    random_state=42
)
```

## Results

The notebook is designed to compare different feature
extraction techniques and machine learning models.

The evaluation focuses on:

- Training accuracy
- Validation accuracy
- Test accuracy
- Overfitting gaps
- Cross-validation performance

Final numerical results will be added after executing
the notebook.

## Key Findings

- Feature extraction helps transform images into
  meaningful numerical representations.
- High training accuracy does not necessarily indicate
  strong performance on unseen data.
- Complex models can memorize training examples.
- Cross-validation helps estimate model generalization.
- Proper dataset splitting is essential for reliable
  machine learning evaluation.

## Technologies Used

- Python
- OpenCV
- Scikit-learn
- Scikit-image
- NumPy
- Matplotlib
- Seaborn
- Google Colab
- Jupyter Notebook

## How to Run

1. Open the notebook in Google Colab.
2. Install the required libraries if necessary.
3. Run all notebook cells in order.
4. Allow the Olivetti Faces dataset to download.
5. Review the feature extraction visualizations.
6. Compare model performance and evaluation results.

## Real-World Applications

- Image classification
- Computer vision research
- Pattern recognition
- Machine learning model evaluation

## Acknowledgments

This project was completed as part of the ITAI 1378
Computer Vision coursework at Houston Community College.
