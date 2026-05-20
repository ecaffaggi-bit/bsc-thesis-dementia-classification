# Dementia Classification with ResNet-18 and MedViT - BSc Thesis - Cognitive Science and Artificial Intelligence

This project investigates Alzheimer’s disease classification using MRI scans from the OASIS-1 dataset. It compares a CNN-based model (ResNet-18) and a hybrid CNN vision transformer-based model (MedViT) under the same experimental setting.

## Project Overview
- Dataset: OASIS-1 MRI scans
- Task: Binary classification (Dementia vs Non-Dementia)
- Models: ResNet-18, MedViT
- Methods: preprocessing, augmentation, training, evaluation, Grad-CAM, confusion matrices

## Dataset
The pipeline uses preprocessed T88 GFC MRI volumes from OASIS-1.  
Subjects are split at the subject level to avoid data leakage.  
Each 3D volume is converted into 2D slices for model training.

## Workflow
1. Load and preprocess MRI volumes.
2. Extract center axial slices.
3. Build subject-level train/validation/test splits.
4. Apply data augmentation.
5. Train ResNet-18 and MedViT.
6. Evaluate performance on the test set.
7. Generate training curves and Grad-CAM visualizations.

## Requirements
- Python 3.x
- PyTorch
- torchvision
- nibabel
- numpy
- pandas
- scikit-learn
- matplotlib
- opencv-python
- imageio

## Outputs
- Preprocessed slice images
- Train/validation/test split CSV files
- Training and validation loss/accuracy curves
- Model checkpoints
- Grad-CAM visualizations
- Comparison figures for the thesis

