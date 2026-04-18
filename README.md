# Repo 5: Task-fMRI GLM Cognitive Activation Analysis

## Overview

This repository demonstrates an end-to-end task-based fMRI statistical analysis workflow using the Haxby dataset and Python neuroimaging tools.

The project was designed to expand methodological breadth beyond previous resting-state connectivity and machine learning repositories by implementing classical task-fMRI inference using the General Linear Model (GLM).

Core components include:

- dataset auditing
- experimental condition inspection
- event construction from stimulus labels
- first-level voxelwise GLM
- linear contrast testing
- statistical activation maps
- multi-contrast analysis
- reporting and interpretation

---

## Scientific Objective

To identify category-selective neural activation patterns during visual stimulus processing using task-fMRI data.

Example hypotheses tested:

- Face > House
- Face > Scrambled
- House > Scrambled
- Cat > Bottle

---

## Dataset

**Haxby Dataset** (available through Nilearn)

A canonical public task-fMRI dataset widely used in neuroimaging education and research.

---

## Repository Structure

```repo5-task-fmri-glm-cognitive-activation/
│── notebooks/
│   ├── 01_dataset_audit.ipynb
│   ├── 02_first_level_glm.ipynb
│   ├── 03_advanced_contrast_analysis.ipynb
│   └── 04_reporting_and_interpretation.ipynb
│
│── figures/
│   ├── design_matrix_first_level.png
│   ├── face_vs_house_stat_map.png
│   ├── face_vs_house.png
│   ├── face_vs_scrambled.png
│   ├── house_vs_scrambled.png
│   └── cat_vs_bottle.png
│
└── README.md
```
---

## Notebooks

### 01_dataset_audit.ipynb
Fetches the dataset, inspects files, and verifies task labels.

### 02_first_level_glm.ipynb
Builds events, fits a first-level GLM, creates design matrix and Face > House contrast.

### 03_advanced_contrast_analysis.ipynb
Runs multiple contrasts across stimulus categories and saves activation maps.

### 04_reporting_and_interpretation.ipynb
Summarizes methods, outputs, and scientific interpretation.

---

## Methods

Implemented with:

- Python
- Nilearn
- Pandas
- Matplotlib
- Nibabel

GLM settings:

- SPM hemodynamic response function
- cosine drift regressors
- high-pass filtering
- spatial smoothing
- voxelwise linear modelling

---

## Why This Repository Matters

This project demonstrates competency in:

- task-fMRI workflows
- event-based modelling
- neuroimaging statistics
- contrast specification
- scientific visualization
- reproducible computational pipelines

---

## Future Directions

Potential extensions include:

- ROI-based summaries
- MVPA / decoding analysis
- representational similarity analysis
- larger multi-subject inference
- permutation-based statistics
