# NIH Sickle Cell Research Funding Analysis

## Overview
This repository contains a Jupyter notebook that explores **NIH-funded research projects related to sickle cell disease** using publicly available data from the **NIH RePORTER** database. The goal of this project is to better understand how sickle cell research is represented within broader hematology research funding and to practice applied data science and machine learning techniques on real-world biomedical data.

This project was completed as part of my effort to build experience in **data science, machine learning, and research-oriented analysis**, particularly for graduate school preparation.

---

## Motivation
Sickle cell disease is a serious and historically underfunded condition relative to its impact. The NIH Cure Sickle Cell Initiative aims to address this gap, and NIH RePORTER provides detailed data on funded research projects.

This project was motivated by the following questions:
- How frequently do sickle cell–focused projects appear within NIH hematology research funding?
- Can basic natural language processing techniques help distinguish sickle cell research from other hematology topics?
- What challenges arise when working with imbalanced, real-world research data?

---

## Data Source
- **NIH RePORTER Project and Abstract Data**
- CSV files containing project metadata and abstracts (e.g., fiscal year data)

The data includes project titles, abstracts, funding details, and research categories.

---

## What the Notebook Does
The notebook walks through the following steps:

### 1. Data Loading & Cleaning
- Load NIH RePORTER CSV files
- Filter projects related to hematology
- Label projects as *sickle cell* or *other hematology* based on keywords

### 2. Exploratory Analysis
- Examine class imbalance between sickle cell and non–sickle cell projects
- Inspect example abstracts and labels

### 3. Text Processing
- Basic text preprocessing
- Feature extraction using standard NLP techniques

### 4. Machine Learning Model
- Train a simple classification model to distinguish sickle cell research from other hematology research
- Evaluate performance using accuracy, precision, recall, and F1 score

### 5. Results & Reflection
- Analyze model performance
- Discuss limitations caused by class imbalance and overlapping research topics
- Reflect on what worked, what didn’t, and why

---

## Key Findings
- The dataset is **highly imbalanced**, with far fewer sickle cell–specific projects compared to other hematology research.
- While overall accuracy is high, recall for sickle cell projects is relatively low, highlighting the limitations of basic models on imbalanced text data.
- Many abstracts overlap in terminology, making strict classification challenging without more advanced techniques.

These results emphasize the importance of careful evaluation beyond accuracy alone.

---

## Learning Outcomes
Through this project, I gained hands-on experience with:
- Working with real-world biomedical research data
- Text preprocessing and feature extraction
- Training and evaluating classification models
- Interpreting model performance in the presence of class imbalance
- Writing reflective, research-oriented analysis

This notebook is intended as a **learning and exploratory project**, not a production-level system.

---

## Future Work
Possible next steps include:
- Applying class weighting or resampling techniques
- Trying alternative text representations (e.g., TF-IDF vs embeddings)
- Exploring topic modeling to better capture overlapping research themes
- Analyzing funding amounts and trends over time

---

## Notes
This project is part of a broader effort to build a portfolio for graduate study in data science / machine learning and to gain experience with applied research analysis.

