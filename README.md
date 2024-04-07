# Leaf_Classification

This project was developed as part of an Artificial Neural Networks and Deep Learning course at Politecnico di Milano (2021/2022). It was organized as an Codalab competition among students groups.

## Authors

- [Kinga](https://github.com/Astenna)
- [Marco](https://github.com/zenimarc)
- Andreas

## Problem description

The goal was to perform a classifiction of leaves based on their images. The dataset was composed of 17728 leaf images of 13 different species of plants. In other words, given an image, the goal was to predict the correct species of the plant (class label).

## Dataset

The zipped dataset can be found [here](https://drive.google.com/drive/folders/19nmCsp_6j06UF-GyT1V9NEv6BB4X-lNN?usp=sharing) in file `dataset.zip`. Additionally, also the subset of data used in the TTA tests (`TTA_tests.ipyinb`) is made available in the `TTA-dataset.zip`.

## How to run

To run the `final_model.ipynb` and `TTA_tests.ipynb` notebooks, download the datasets from the link in the *Dataset* section and unzip them to the directory of your choice. Then, adjust the paths to the datasets specified in the code notebooks.

## Solution

The final model submitted by the team can be found in `final_model.ipynb` file. The model uses transfer learning with pre-trained VGG16 extended with one fully connected layer. Since we did not expect the VGG16 to match our classification problem, we fine-tuned the VGG16’s convolutional layers starting from the 14th layer.

The details of the model are described in the `report.pdf` available in this repository. To see how we addressed problems such as overfitting, class imbalance, and how we tuned the hyperparameters, please refer to the report.