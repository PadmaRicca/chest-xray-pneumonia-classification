# Chest X-Ray Pneumonia Classification

**Project Level:** Postgraduate

**Author:** Padma Michela Ricca  
**Institution:** University College London (UCL)  
**Degree:** MSc Artificial Intelligence for Biomedicine and Healthcare
**Module:** COMP0188 (Deep Representations and Learning)  
**Assessment Outcome:** 79% (Distinction-level)  
**Overall Module Mark:** 75.10% (Distinction-level)  
**Project Type:** Deep learning, medical image classification and model evaluation project

## Project Overview

Developed convolutional neural networks (CNNs) from scratch using PyTorch to distinguish Normal and Pneumonia chest X-ray images from the publicly available [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia) dataset.

The project progressed from a baseline architecture to a regularised network, using comparative experiments to investigate overfitting, generalisation and the effects of different design choices.

The final network achieved 94.7% accuracy on a held-out test set of 587 images, with recall of 97.2% for Pneumonia and 88.1% for Normal. It missed 12 Pneumonia cases and incorrectly identified 19 Normal images, highlighting class-specific error trade-offs. These results do not establish clinical validity.

## Contributions

- Analysed class distributions, image dimensions and channel formats, identifying a 73% Pneumonia majority and informing preprocessing requirements.
- Implemented a custom PyTorch data pipeline incorporating greyscale conversion, resizing, normalisation and controlled rotation augmentation, while excluding horizontal flipping to preserve anatomical plausibility.
- Designed and trained a baseline three-block CNN, subsequently introducing batch normalisation, dropout, weight decay and learning-rate scheduling to address observed overfitting.
- Developed reusable training and validation routines to track losses, overall and class-wise accuracies, visualise learning curves and manage saved checkpoints.
- Compared the original and refined networks, observing a reduction in final-epoch validation loss from 0.1444 to 0.0671 despite identical peak validation accuracies of 97.4%.
- Conducted three ablation experiments removing batch normalisation, dropout and the combined optimisation modifications, identifying differences in convergence and demonstrating that individual changes did not consistently improve results.
- Assessed the final predictions using precision, recall, F1 scores and confusion matrix analysis to examine false positives and false negatives.

## Skills Demonstrated

- **Deep Learning:** Understanding of convolutional architectures, optimisation strategies and regularisation techniques.
- **Medical Image Processing:** Preparing radiographic datasets and selecting anatomically appropriate transformations.
- **Experimental Design:** Constructing controlled comparisons, investigating individual design choices and interpreting inconclusive findings.
- **Performance Analysis:** Evaluating learning behaviour, class imbalance and diagnostic error patterns.
- **Scientific Programming and Technical Documentation:** Structuring reusable computational workflows, managing experimental outputs and communicating technical findings.

## Report Availability

The original academic notebook and associated source code are currently withheld from public access to uphold academic integrity.

This repository provides an overview of the project's objectives, deep learning approach, experimental evaluation and skills demonstrated.

Further technical documentation and implementation details may be made available upon request, in accordance with the University's policies.
