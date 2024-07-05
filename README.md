# Gradient Boosting Classifier for Wine Classification Using Weights & Biases

This repository leverages Weights & Biases to systematically optimize and evaluate the hyperparameters of a Gradient Boosting Classifier. The dataset utilized is the Wine dataset.

![banner](https://enoturismospain.com/imagen/bodega/4/124/bodega-fundador-mezquita.jpg)

## Results

Detailed experimentation results are available on the Weights & Biases dashboard. This includes performance metrics such as accuracy and the specific hyperparameters used for each trial.

🔗 [Dashboard](https://wandb.ai/mar27benitez-Upgrade%20hub/wine_class/reports/Wine-Classification-with-GradientBoosting-Wandb--Vmlldzo4NTYzNTYw?accessToken=34lkqaroi53sgo04qhrvkhlxj2n8z0qtdk3v3z7fs0sju68wtzl2k1gimuhxjlfx)

## Problem Overview

This project addresses a typical multi-class classification problem. The goal is to predict the wine category based on various physicochemical properties. The Wine dataset is a well-known benchmark in the machine learning field.

## Dataset Description

The Wine dataset is publicly accessible and includes 178 wine samples, each with 13 attributes such as Alcohol content, Malic acid, and Ash. The samples are categorized into three classes, representing different wine types. This dataset is ideal for classification tasks.

## Experimentation

For this project, I use the Gradient Boosting Classifier, a robust ensemble machine learning algorithm built upon decision trees. It is particularly noted for its efficacy in classification tasks.

To identify the optimal model, I experiment with various hyperparameter combinations including learning rate, tree depth, and the number of estimators. Systematic experimentation helps in understanding how these hyperparameters influence model performance and identifying the optimal configuration.

Weights & Biases is integrated into the experimentation pipeline, enabling logging of hyperparameters and performance metrics for each experiment. This tool provides an interactive dashboard to visualize and analyze results.

## Hyperparameter Tuning and Optimal Model

During the experimentation, an extensive hyperparameter search was conducted, testing a total of 384 different combinations. The hyperparameters tuned include:

- Learning rate
- Maximum tree depth
- Number of estimators
- Loss function
- Subsample fraction
- Minimum samples required to split an internal node
- Minimum samples required to be at a leaf node

The **best-performing model** achieved an accuracy of 0.9815, demonstrating its effectiveness in accurately classifying the wine samples. The optimal hyperparameters are:

    Learning rate: 0.1
    Loss function: deviance
    Max depth: 3
    Min samples leaf: 2
    Min samples split: 2
    N estimators: 50
    Subsample: 1

This optimal combination allowed the Gradient Boosting Classifier to effectively capture the data patterns and deliver highly accurate predictions.
