# Machine Learning Assignment 2

**Name:** Amrit Kumar Giri  
**Roll Number:** M26ECC001  
**Dataset:** Olivetti Faces  
**Random Seed:** 26001

## Project Overview

This project studies the performance of decision trees, bagging, and multiclass SAMME boosting on the Olivetti Faces dataset.

The assignment is divided into three experiments:

- **Q1: Decision Tree and Bagging** : Training individual decision trees, implementing bootstrap bagging, analysing out-of-bag predictions, and evaluating model performance when part of a face image is missing.
- **Q2: Multiclass Boosting** : Implementing the SAMME algorithm from scratch and comparing boosting with bagging.
- **Q3: Bias and Variance** : Measuring bias squared and variance across 30 resampled training sets and studying the effect of decision-tree depth.

## Dataset

The Olivetti Faces dataset contains 400 grayscale face images representing 40 individuals. Each image has 64 × 64 pixels.

For each individual, the dataset is divided into:

- 6 training images
- 2 validation images
- 2 testing images

The same saved split is used throughout the project.

## Main Results

| Model | Clean Test Accuracy | Masked Test Accuracy |
|---|---:|---:|
| Single Decision Tree | 53.75% | 35.00% |
| Bagging | 80.00% | 61.25% |
| SAMME Boosting | 50.00% | 46.25% |

The experiments show that bagging provides the highest accuracy on both clean and masked images.

## Running the Project

1. Install Python and create a virtual environment.
2. Install the required packages using `pip install -r requirements.txt`.
3. Open the project folder in VS Code or Jupyter.
4. Run the Q1, Q2, and Q3 notebooks in order.
5. Keep the original saved dataset split to reproduce the experiments.

The `data` folder contains saved dataset indices and the `results` folder contains figures, tables, and experimental outputs.

## Reproducibility

The experiments use random seed 26001. Hyperparameters are selected using validation accuracy, and the clean test set is kept separate from model selection.

## Author

Amrit Kumar Giri  
M26ECC001