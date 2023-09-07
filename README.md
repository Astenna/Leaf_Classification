# Leaf_Classification

This project was developed as part of an Artificial Neural Networks and Deep Learning course at Politecnico di Milano (2021/2022). It was organized as an Codalab competition among students groups.

## Authours

TODO: add names

## Problem description

The goal was to perform a classifiction of leaves based on their images. The dataset was composed of 17728 leaf images of 13 different species of plants. In other words, given an image, the goal was to predict the correct species of the plant (class label).

## Dataset

The dataset is available [here](https://drive.google.com/file/d/1axOBW2e9Q8M4ICLLsaqKF3URzlAWliQh/view?usp=drive_link).

## Solution

The final model submitted by the team can be found in `final_model.ipynb` file. The model uses transfer learning with pre-trained VGG16 extended with one fully connected layer. Since we did not expect the VGG16 to match our classification problem, we fine-tuned the VGG16’s convolutional layers starting from the 14th layer.

The details of the model are described in the `report.pdf` available in this repository. To see how we addressed problems such as overfitting, class imbalance, and how we tuned the hyperparameters, please refer to the report.