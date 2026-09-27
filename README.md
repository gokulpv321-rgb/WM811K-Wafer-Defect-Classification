# Deep Learning Based Semiconductor Wafer Defect Inspection

## Project Overview

This project develops a deep learning-based system for automatic semiconductor wafer defect classification using the WM-811K wafer map dataset.

The objective is to classify wafer maps into different defect categories using Convolutional Neural Networks (CNNs), reducing the dependence on manual wafer inspection.

## Dataset

The project uses the WM-811K dataset, containing wafer maps with different failure patterns.

The nine classes considered in this project are:

- Center
- Donut
- Edge-Loc
- Edge-Ring
- Loc
- Near-full
- Random
- Scratch
- None

The original dataset is not uploaded to this repository because of its large file size.

## Methodology

The project workflow consists of:

1. Loading and exploring the WM-811K dataset
2. Cleaning and preprocessing wafer maps
3. Visualizing wafer-map failure patterns
4. Preparing training, validation, and test datasets
5. Building a baseline Convolutional Neural Network
6. Training and validating the CNN
7. Evaluating model performance using test accuracy
8. Generating a confusion matrix
9. Calculating precision, recall, and F1-score
10. Performing misclassification analysis
11. Developing and evaluating an improved CNN architecture

## Model Performance

### Baseline CNN

- Test Accuracy: **80.63%**
- Test Loss: **0.7068**

The confusion matrix and class-wise precision, recall, and F1-score were used to evaluate the model beyond overall accuracy.

### Improved CNN

- Test Accuracy: **78.08%**

The improved architecture did not outperform the baseline CNN on the test set, demonstrating the importance of validating architectural changes experimentally rather than assuming that a more complex model will necessarily perform better.

## Key Results

The baseline CNN achieved:

- **80.63% overall test accuracy**
- Strong classification performance for classes such as Center, Donut, Edge-Ring, and Near-full
- Greater confusion among visually similar defect patterns such as Loc, Edge-Loc, Scratch, and None

Misclassification analysis was also performed to identify the most frequent class-to-class prediction errors.

## Technologies Used

- Python
- Google Colab
- NumPy
- Pandas
- Matplotlib
- TensorFlow / Keras
- Scikit-learn
- Convolutional Neural Networks (CNN)

## Repository Contents

```text
WM811K-Wafer-Defect-Classification/
│
├── Deep_Learning_Semiconductor_Wafer_Defect_Inspection.ipynb
└── README.md
