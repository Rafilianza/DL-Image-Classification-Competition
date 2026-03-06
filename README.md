# FIT5215 Deep Learning: Image Classification Competition



## Overview
This repository contains the code, evaluation metrics, and ensembling strategies used for the **FIT5215 Deep Learning** image classification competition at Monash University. The primary approach leverages a fine-tuned **DINOv2** (Vision Transformer) model to achieve highly accurate predictions across a diverse set of image classes.

## Results & Achievement
**Ranked in the Top 10 out of a cohort of 380 students.**

<div align="center">
  <img src="assets/Kaggle Certificate.jpg" width="700" alt="FIT5215 Top 10 Certificate of Achievement">
  <p><i>Official Certificate of Achievement for the FIT5215 Deep Learning Competition.</i></p>
</div>

## Dataset Specification
The model was trained and evaluated on a custom dataset provided for the competition, structured as follows:
* **Total Classes:** 20 distinct categories
* **Training Data:** 10,000 labeled images
* **Test Data:** 16,000 unlabelled images (used for final competition scoring)

## Repository Structure

* **`1_Training_DinoV2.ipynb`** Contains the core training pipeline. This notebook covers data loading, preprocessing, and the fine-tuning of the pre-trained DINOv2 foundational model on the 20-class dataset.
  
* **`2_Classification_Reports.ipynb`** A comprehensive evaluation module. This file generates and stores classification reports (Precision, Recall, F1-Score) and confusion matrices for every model iteration produced during the experimentation phase.
  
* **`3_Ensemble_Results.ipynb`** The final inference pipeline. This script aggregates the predictions from the top-performing models and applies ensembling techniques (such as majority voting or weighted averaging) to maximize final accuracy on the 16,000-image test set.
