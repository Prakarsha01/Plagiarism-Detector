# Plagiarism Project, Machine Learning Deployment

This repository contains code and associated files for deploying a plagiarism detector using AWS SageMaker.

## Project Overview

In this project, I build a plagiarism detector that examines a text file and performs binary classification, labeling that file as either *plagiarized* or *not*, based on how similar it is to a provided source text. Detecting plagiarism is a challenging task as the differences between paraphrased answers and original work are often subtle and not easily discernible.
This project will be broken down into three main notebooks:

**Notebook 1: Data Exploration**

* Load in the corpus of plagiarism text data.
* Explore the existing data features and the data distribution.

**Notebook 2: Feature Engineering**

* Clean and pre-process the text data.
* Define features for comparing the similarity of an answer text and a source text, and extract similarity features.
* Select "good" features, by analyzing the correlations between different features.
* Create train/test `.csv` files that hold the relevant features and class labels for train/test data points.

**Notebook 3: Train and Deploy Your Model in SageMaker**

* Upload train/test feature data to S3.
* Define a binary classification model and a training script.
* Train model and deploy it using SageMaker.
* Evaluate deployed classifier.

---

## Acknowledgments

This project is part of the **Udacity Machine Learning Engineer Nanodegree** course on Udacity. Special thanks to the course instructor for the guidance and inspiration.
