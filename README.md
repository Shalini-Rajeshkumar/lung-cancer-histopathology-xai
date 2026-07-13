# Lung Cancer Histopathology Classification with Explainable AI

## Project Overview

This project presents an explainable ensemble deep learning pipeline for lung cancer histopathology classification. The aim is to classify lung tissue images into three categories:

- Adenocarcinoma
- Squamous Cell Carcinoma
- Benign Lung Tissue

The project uses transfer learning with multiple convolutional neural network architectures and integrates explainable AI using Grad-CAM to improve transparency and interpretability.

## Academic Context

This project was developed as part of an MSc Data Science and Computational Intelligence academic research project at Coventry University.

Only a portfolio-safe summary is included in this repository. The full university dissertation report is not uploaded publicly due to academic and copyright considerations.

## Dataset

The project is based on the LC25000 Lung and Colon Histopathology Dataset.

For this work, a balanced lung subset was used:

- Total images: 3,000
- Classes: 3
- Images per class: 1,000
- Split: 70% training, 15% validation, 15% testing

The dataset is not included directly in this repository. Users should download it from the original source and follow the setup instructions in `data/README.md`.

## Models Used

The project compares three transfer learning models:

- ResNet-50
- DenseNet-121
- EfficientNet-B0

A soft-voting ensemble was then created by combining the predictions of the individual CNN models.

## Explainable AI

Grad-CAM was used to visualise the image regions influencing model predictions. This helps make the deep learning pipeline more interpretable by highlighting tissue regions that contributed to classification decisions.

## Key Workflow

1. Load and prepare lung histopathology images
2. Balance the dataset across three classes
3. Resize and augment images
4. Train transfer learning CNN models
5. Compare individual model performance
6. Build a soft-voting ensemble
7. Evaluate using accuracy, precision, recall, F1-score, and confusion matrix
8. Apply Grad-CAM for explainability
9. Analyse model errors and interpretability outputs

## Tools and Technologies

- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- OpenCV
- Grad-CAM
- Google Colab / Jupyter Notebook

## Repository Structure

```text
lung-cancer-histopathology-xai/
├── README.md
├── PROJECT_SUMMARY.md
├── REPORT_SUMMARY.md
├── requirements.txt
├── data/
│   └── README.md
├── notebooks/
│   └── README.md
├── visuals/
│   └── README.md
├── outputs/
│   └── README.md
└── src/
    └── README.md
```

## Results Summary

The ensemble model was designed to improve classification robustness compared with individual CNN models. Grad-CAM visualisations were used to support interpretability by showing class-discriminative image regions.

## Important Note

This repository is a portfolio-safe version of the academic project. It does not contain:

- Full university dissertation report
- Student ID
- Ethics application number
- Declaration pages
- Copyright pages
- Private academic submission material

## Future Improvements

- Extend the pipeline to whole-slide images
- Add transformer-based architectures
- Improve external validation using multi-source pathology datasets
- Deploy the model as an interactive demo
- Add a Streamlit dashboard for prediction and Grad-CAM visualisation

## Author

**Shalini Rajeshkumar**  
MSc Data Science and Computational Intelligence  
Coventry University  
GitHub: [Shalini-Rajeshkumar](https://github.com/Shalini-Rajeshkumar)
