# Skin Disease Identification System Using Deep Learning

## Overview

The Skin Disease Identification System is a machine learning and deep learning project that classifies skin lesion images into seven diagnostic categories using the HAM10000 dataset.

The project uses EfficientNetB4, a convolutional neural network architecture, for image classification. It also compares traditional machine learning algorithms to evaluate their performance against the deep learning approach.

**Note:** This project is intended for educational and research purposes. It is not a substitute for professional medical diagnosis.

## Objectives

- Develop a deep learning model for skin lesion image classification.
- Explore and analyze the HAM10000 dataset.
- Compare traditional machine learning algorithms with deep learning.
- Evaluate model performance using accuracy, precision, recall, and F1-score.
- Visualize training performance and classification results.

## Technologies Used

- Python
- TensorFlow and Keras
- NumPy
- Pandas
- Scikit-learn
- OpenCV
- Matplotlib
- Seaborn
- XGBoost
- Imbalanced-learn
- KaggleHub

## Dataset

**Dataset:** HAM10000 — Human Against Machine with 10,000 training images.

The dataset contains 10,015 dermatoscopic images organized into seven skin lesion categories.

The categories are:

| Code | Category |
|---|---|
| akiec | Actinic Keratoses and Intraepithelial Carcinoma |
| bcc | Basal Cell Carcinoma |
| bkl | Benign Keratosis-like Lesions |
| df | Dermatofibroma |
| mel | Melanoma |
| nv | Melanocytic Nevi |
| vasc | Vascular Lesions |

Dataset information: https://doi.org/10.1038/sdata.2018.161

## Machine Learning Models

The project compares the following models:

1. Random Forest
2. XGBoost
3. Support Vector Machine (SVM)
4. EfficientNetB4

EfficientNetB4 is used as the primary deep learning architecture.

## Methodology

The project follows these steps:

1. Check the available GPU and install dependencies.
2. Load the HAM10000 dataset.
3. Perform exploratory data analysis.
4. Analyze class imbalance.
5. Evaluate traditional machine learning baselines.
6. Prepare image data and apply augmentation.
7. Build an EfficientNetB4-based classification model.
8. Train the model in multiple phases.
9. Apply test-time augmentation during prediction.
10. Evaluate performance using classification metrics.
11. Generate confusion matrices and performance plots.
12. Test predictions on sample images.
13. Save the trained model.

## Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- Per-class classification performance

Actual results should be taken from the completed notebook execution.

## Project Structure

```text
skin-disease-identification-ham10000/
│
├── Skin_Disease_HAM10000_FINAL.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── LICENSE
```

Additional result files and model weights can be included when available and appropriate.

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/skin-disease-identification-ham10000.git
```

Move into the project directory:

```bash
cd skin-disease-identification-ham10000
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Open the notebook in Jupyter:

```bash
jupyter notebook Skin_Disease_HAM10000_FINAL.ipynb
```

You can also run the notebook in Google Colab with GPU acceleration.

## Results

The notebook generates:

- Dataset distribution visualizations
- Sample skin lesion images
- Machine learning model comparisons
- Training and validation curves
- Confusion matrices
- Classification reports
- Sample image predictions

**Performance:** Add the actual test accuracy, precision, recall, and F1-score after running the complete notebook.

Do not report a target accuracy as an achieved result unless it is supported by experimental results.

## Limitations

- Model performance depends on the dataset, preprocessing, and evaluation methodology.
- Class imbalance may affect predictions for less frequent categories.
- Results on HAM10000 may not generalize to other datasets or real-world clinical images.
- Predictions should not be used independently to diagnose or treat a medical condition.

## Future Improvements

- Develop a web application for image uploads and predictions.
- Evaluate performance on independent external datasets.
- Improve model interpretability using Grad-CAM.
- Investigate methods for handling class imbalance.
- Optimize model inference and deployment.

## Disclaimer

This project is for educational and research purposes only. It is not a clinically validated diagnostic tool and must not replace consultation with a qualified healthcare professional.
