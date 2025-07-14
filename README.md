# 🐾 AREPS: A Robust Explainable Pawpularity System
## Predicting and Explaining Pet Photo Attractiveness

This project was done as part of a Data Mining and Warehousing course at the University of South Carolina.

<div align="center"> 
  <img width="349" height="298" alt="Screenshot 2025-07-14 at 5 40 18 PM" src="https://github.com/user-attachments/assets/57f82268-c96f-4a75-8226-21e2deca5c4a" />
</div>

## Overview
This project tackles a real-world problem: helping shelter animals get adopted by improving how attractive their photos appear online. Using the PetFinder.my Pawpularity dataset from Kaggle, this system predicts how likely a pet photo is to be deemed "cute" and provides transparent explanations for each prediction using LIME.

The goal is not just high performance, but also explainability and trustworthiness, enabling users and stakeholders to understand why a model made a prediction.

## Motivation
- Pet photos with higher appeal lead to faster adoptions.
- Neural networks can predict visual appeal, but are black-boxes.
- This project builds both a robust model and a trustworthy explanation system to help animal welfare platforms like PetFinder.my improve their decision-making tools.

$ ./tree-md .
## Repository Structure

 * [code](./code)
   * [PetFinder.ipynb](./code/PetFinder.ipynb)
 * [docs](./docs)
   * [report.pdf](./docs/report.pdf)
 * [README.md](./README.md)

## 🐶 Dataset
- Source: Kaggle Pawpularity Competition
- Images: 9912 pet photos
- Metadata: 14 features (e.g., eyes, face, blur, collage, etc.)
- Target: Pawpularity score (0–100), converted into 5 bins for classification.

## Preprocessing Steps
- Extract image + Pawpularity score using ID
- Normalize pixel values
- Convert score into 5 bins (classification instead of regression)
- Apply horizontal flip data augmentation
- Reshape labels into a binary array form

## Models Used
- CNN:	Custom 5-layer CNN with Conv, ReLU, BN, Pool, Dropout
- InceptionV3:	Transfer learning from ImageNet, with custom dense head and softmax

## 🔍 Explainability with LIME
LIME was applied post-training to understand which parts of the pet image contributed most to the prediction.
- Highlights eyes, paws, and background as key visual features
- Helps identify model bias toward certain backgrounds or poses
- Encourages data and model improvement through visual insight

<div align="center"> 
  <img width="477" height="290" alt="Screenshot 2025-07-14 at 5 39 44 PM" src="https://github.com/user-attachments/assets/15c1219e-8827-4c62-b840-b48f43a0857c" />
</div>
