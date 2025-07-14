# 🐾 AREPS: A Robust Explainable Pawpularity System
## Predicting and Explaining Pet Photo Attractiveness

This project was done as part of a Data Mining and Warehousing course at the University of South Carolina.

## Overview
This project tackles a real-world problem: helping shelter animals get adopted by improving how attractive their photos appear online. Using the PetFinder.my Pawpularity dataset from Kaggle, this system predicts how likely a pet photo is to be deemed "cute" and provides transparent explanations for each prediction using LIME.

The goal is not just high performance, but also explainability and trustworthiness, enabling users and stakeholders to understand why a model made a prediction.

## Motivation
- Pet photos with higher appeal lead to faster adoptions.
- Neural networks can predict visual appeal, but are black-boxes.
- This project builds both a robust model and a trustworthy explanation system to help animal welfare platforms like PetFinder.my improve their decision-making tools.

$ ./tree-md .
# Project tree
.
 * [tree-md](./tree-md)
 * [dir2](./dir2)
   * [file21.ext](./dir2/file21.ext)
   * [file22.ext](./dir2/file22.ext)
   * [file23.ext](./dir2/file23.ext)
 * [dir1](./dir1)
   * [file11.ext](./dir1/file11.ext)
   * [file12.ext](./dir1/file12.ext)
 * [file_in_root.ext](./file_in_root.ext)
 * [README.md](./README.md)
 * [dir3](./dir3)


## Repository Structure
├── AREPS_Report.pdf               # Full project report (Data Mining course)
├── pawpularity.csv                # Metadata and target scores
├── images/                        # Folder of pet images from the dataset
├── AREPS_CNN_Model.ipynb          # Notebook training & evaluating CNN
├── AREPS_InceptionV3_Model.ipynb  # Notebook for InceptionV3 + LIME
├── README.md                      # You're here
