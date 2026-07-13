# Report Summary

## Project Aim
The aim of this project was to develop an explainable ensemble deep learning pipeline for classifying lung cancer histopathology images.

## Problem
Lung cancer diagnosis often relies on histopathological examination. Manual microscopy can be time-consuming and may vary between observers. Deep learning models can support automated classification, but their black-box nature makes interpretability a challenge in healthcare settings.

## Dataset
The project used a lung-only subset of the LC25000 histopathology dataset. The selected dataset contained 3,000 balanced images across three classes:

- Adenocarcinoma
- Squamous Cell Carcinoma
- Benign Lung Tissue

## Methodology
The workflow included dataset preparation, image resizing, augmentation, CNN transfer learning, ensemble modelling, evaluation, Grad-CAM explainability, and error analysis.

## Models
- ResNet-50
- DenseNet-121
- EfficientNet-B0
- Soft-voting ensemble model

## Explainability
Grad-CAM was used to highlight the regions of histopathology images that influenced classification decisions. This supports transparency and helps understand whether the model is focusing on meaningful tissue structures.

## Key Outcomes
- Built an end-to-end deep learning pipeline for medical image classification
- Compared multiple CNN architectures
- Developed an ensemble model for robust prediction
- Integrated Grad-CAM visualisation for explainable AI
- Strengthened skills in healthcare AI, PyTorch, transfer learning, and model evaluation

## Safe Portfolio Note
This is a summarised portfolio version of the academic project. The full university dissertation report is not included publicly.
