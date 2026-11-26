# Chihuahua vs. Muffin Classification Using CNN

## Course Information
- Student: Ali Abed
- Course: ITAI 1378 - Computer Vision
- Lab: L05
- Institution: Houston Community College

## Problem Statement

The objective of this project is to develop a Convolutional
Neural Network (CNN) that classifies images as either
Chihuahuas or muffins.

## Approach

The project uses PyTorch to build, train, and evaluate
a CNN for binary image classification.

The main steps include:

- Image resizing to 224 x 224 pixels
- Image normalization and data augmentation
- Training and validation dataset preparation
- CNN model development
- Cross-entropy loss function
- Adam optimizer with a learning rate of 0.001
- Model training over 10 epochs
- Performance evaluation and visualization

## Results

| Metric | Result |
|---|---|
| Training epochs | 10 |
| Training samples | 10 |
| Validation samples | 10 |
| Final training accuracy | 40% |
| Validation accuracy | 50% |
| Final validation loss | 0.6933 |

The model achieved 50% validation accuracy because a
dataset-loading issue caused the notebook to use
placeholder gray images instead of real images.

These results do not represent the model's actual
classification ability on real Chihuahua and muffin images.

## Key Findings

- CNNs preserve spatial relationships within images.
- Convolutional layers extract important visual features.
- Data quality directly affects model performance.
- Training data must be verified before model training.
- Successful code execution does not guarantee reliable results.

## Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Pillow
- tqdm
- Google Colab

## Dataset

The intended dataset is available at:

https://github.com/mlatsjsu/workshop-chihuahua-vs-muffin

The original experiment used placeholder images due to
a dataset-loading issue.

## How to Run

1. Open the Jupyter notebook in Google Colab.
2. Install the required libraries.
3. Download the original dataset from the source above.
4. Configure the training and validation dataset paths.
5. Remove the placeholder image generation cell.
6. Run all notebook cells.
7. Review the training results and predictions.

## Future Improvements

- Restore the original image dataset.
- Verify images before training.
- Retrain the CNN using real images.
- Compare performance with a traditional neural network.
- Evaluate accuracy and confusion matrix.

## References and Credits

- [Original Workshop](https://github.com/mlatsjsu/workshop-chihuahua-vs-muffin)
- [DeepSense.ai Tutorial](https://deepsense.ai/keras-vs-pytorch-avp-transfer-learning/)
- [PyTorch Documentation](https://pytorch.org/docs/stable/)

