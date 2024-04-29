# Forest Type Classification
## Overview
This project focuses on the classification of forest types based on various environmental and tree features. The dataset used comprises multiple features that describe different aspects of forests, and the goal is to accurately classify each forest type. The Python script leverages machine learning techniques, specifically the K-Nearest Neighbors (KNN) algorithm, to predict forest types.
## Dataset
The dataset, forest_dataset.csv, includes various features about trees and environmental conditions. The last column in the dataset represents the class labels for forest types.
## Features
- The dataset consists of 54 features including soil type, shade, elevation, and other environmental characteristics relevant to forestry.
- The last column is the target variable representing different types of forests encoded as integers.
## Requirements
- Python 3.x
- Libraries: pandas, numpy, sklearn, matplotlib
## Installation
To set up the environment for running this project, you need to install the required libraries. You can install these using pip:
```bash
pip install pandas numpy scikit-learn matplotlib
```
## Usage
1. Load the dataset into a pandas DataFrame.
2. Split the dataset into training and testing sets.
3. Train a K-Nearest Neighbors (KNN) classifier on the training data.
4. Evaluate the model on the test set.
5. Use GridSearchCV to find the optimal parameters for the KNN classifier.
6. Compare the classification accuracy before and after parameter tuning.
7. Visualize the real vs predicted frequency of each class.
Additionally, you can use the predict_tree function to predict the forest type based on a provided feature array.
## Predicting Forest Type
o predict the type of forest using an array of features:
```python
# Replace the list with your actual feature values
features = [0.1, 0.2, ..., 0.54]  # Example feature values
predicted_class = predict_tree(features)
print("Predicted tree class:", predicted_class)
```
## Example Output
The script will output the initial classification accuracy and the accuracy after performing grid search optimization. Additionally, a bar chart showing the real vs predicted frequency of each forest class is displayed.
## Classes Dictionary
The classes are mapped as follows:
- 0: Pine tree
- 1: Fir
- 2: Birch tree
- 3: Poplar
- 4: Oak
- 5: Maple
These mappings are used to decode the predicted classes into understandable labels.
## Visualization
A bar chart is plotted to compare the real frequency of forest types in the test set against the predicted frequency derived from the model probabilities.
## Conclusion
This project demonstrates the application of KNN for classifying forest types and the use of grid search to optimize model parameters for better accuracy. It includes a function for making predictions on new data, making it applicable for real-world forestry management and research scenarios.
