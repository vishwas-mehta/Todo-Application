# Week 2 – DVC Integration in IRIS Machine Learning Pipeline

## Objective
This assignment demonstrates the integration of **Data Version Control (DVC)** into the **IRIS machine learning pipeline**.  
The goal is to enable efficient tracking, storage, and versioning of both datasets and model files using Git and Google Cloud Storage.

---

## Overview
The exercise involved setting up a Git repository, initializing DVC, and configuring a Google Cloud Storage bucket as the remote.  
The **Iris dataset** was added and tracked using DVC, followed by training a base model (`train.py`).  
The dataset was then augmented (`augment.py`) to simulate new data, and the model was retrained to observe versioned changes.  
DVC and Git tags (`v1.0`, `v1.1`) were used to manage and restore different stages of the pipeline.

---

## Files Included

| File | Description |
|------|--------------|
| `train.py` | Trains the base Iris model and generates the model and metrics. |
| `augment.py` | Augments the Iris dataset and retrains the model on the new data. |
| `README.md` | Documentation outlining objectives, workflow, and file descriptions. |

---

## Workflow Summary
1. Initialize Git and DVC in the project directory.  
2. Add and track the Iris dataset using `dvc add`.  
3. Configure Google Cloud Storage as the DVC remote and push data.  
4. Train the base model and track outputs using DVC.  
5. Augment the dataset, retrain the model, and commit new versions.  
6. Use `git checkout` and `dvc checkout` to switch between model and data versions.

---

## Key Takeaways
This task highlights how DVC complements Git for **data and model version control**, ensuring reproducibility and efficient storage.  
It demonstrates the ability to manage dataset changes, retrain models, and seamlessly navigate between different pipeline versions.

---
