# A Decision Tree Model for Mushroom Edibility Prediction

## 1. Introduction
Data mining involves extracting information and identifying patterns from large datasets to draw insights using statistical and machine learning methods. This project focuses on analyzing the "Mushrooms" dataset and building a decision tree model to predict whether a mushroom is edible or poisonous based on its specifications. The dataset contains 8,124 records with 23 attributes describing different mushroom characteristics.

## 2. Methods & Analysis
### 2.1. Libraries Used
- Rpart: For implementing recursive partitioning for classification.
- Caret: For streamlining model training processes.
- Rpart.plot: For plotting decision trees.
- Rattle: For data exploration, model building, and evaluation.

### 2.2. Loading the Dataset
The "Mushrooms" dataset is loaded into R from the "mushrooms.xlsx" file.

### 3. Exploratory Data Analysis
#### 3.1. Structure of the Dataset
The dataset consists of 23 variables, all of which are character data types.

#### 3.2. Feature Analysis
Frequency distribution of each predictor feature value among edible and poisonous mushrooms is analyzed.

#### 3.3. Finding Missing Values
No missing values are found in the dataset.

#### 3.4. Steps to Measure Variable Importance
A contingency table is created for each predictor variable against the target variable (class), and the number of perfect splits is calculated.

### 4. Data Splicing
The dataset is split into a training set (80%) and a testing set (20%).

### 5. Classification Tree
A decision tree model is built using the training dataset. Pruning is performed to reduce the size of the tree if necessary.

### 5.1. Pruning the Tree
Pruning is conducted based on the complexity parameter (cp) values.

### 5.2. Predictions on Test Set
The model is tested on the test dataset, and predictions are evaluated using a confusion matrix.

## RECOMMENDATION OF ACTION
Recommendations are provided based on the decision tree's findings, suggesting which mushroom characteristics are associated with edibility or toxicity.

## CONCLUSION
The decision tree model accurately predicts mushroom edibility or toxicity based on specified characteristics, achieving 100% accuracy on the test set.

## REFERENCES
1. [Mushroom classification with decision tree](https://www.kaggle.com/code/geland/mushroom-classification-with-decision-tree/report)
2. [11.9 - R Scripts](https://online.stat.psu.edu/stat508/book/export/html/728)
