# VariGen - AI-Based Genetic Variant Analysis 🧬

This repository contains the machine learning model and research materials developed for the **TEKNOFEST 2026 Health in AI Competition**. 

As part of the **University and Above Level** , this project aims to predict whether genetic variants are "Pathogenic" (disease-causing) or "Benign" (harmless) using their biological and computational properties. This model serves as a digital decision-support mechanism to assist in the early diagnosis of genetic diseases and personalized medicine.

## 🎯 Problem Statement
Classifying genetic variants is critical for clinical diagnosis to prevent data leakage and ensure the model learns true biological patterns rather than memorizing locations, the exact genomic addresses (chromosome and position) of the variants are completely hidden in our dataset. The model must rely solely on the provided bioinformatics features.

## 📊 Dataset & Features
Our model is trained on a balanced dataset containing variants strictly categorized into Pathogenic and Benign classes. The ground truth labels are derived from highly reliable databases like ClinVar, ClinGen, and gnomAD

The multi-dimensional feature set includes:
* **Sequence & Change Data:** Reference/alternative nucleotides and resulting amino acid changes.
* **Local Sequence Context:** Genomic and proteomic neighborhoods (5 elements before and after the variant point).
* **Biochemical & Structural Effects:** Changes in hydrophobicity, polarity, and potential 3D structure impacts.
* **Evolutionary Conservation:** Phylogenetic diversity and conservation scores across different species.
* **Population Data:** Variant frequencies across different human populations (e.g., Minor Allele Frequency).
* **In Silico Risk Scores:** Computational risk scores calculated by various algorithms.

## ⚙️ Evaluation Metric
The ultimate success of the model is evaluated during the external validation phase using a completely hidden test set. The primary metric for determining the ranking is the **F1-Score**, calculated based on True Positives (TP), False Positives (FP), and False Negatives (FN).

## 👨‍💻 Developer
* **Efekan Erkafalı** - Software Engineering Student | Data Structures, Algorithms, OOP with Java & Python.
