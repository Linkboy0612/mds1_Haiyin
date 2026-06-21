# Iris Flower Classification with Decision Tree

## Overview

This project demonstrates a complete machine learning workflow using the famous Iris dataset. A Decision Tree Classifier is trained to predict iris flower species based on four flower measurements.

The notebook covers:

* Data loading and preprocessing
* Train-test split
* Decision Tree model training
* Model evaluation
* Decision tree visualization
* Interactive inference for new predictions

## Dataset

The project uses the Iris dataset, which contains measurements of iris flowers from three species:

* Iris-setosa
* Iris-versicolor
* Iris-virginica

### Features

| Feature      | Description              |
| ------------ | ------------------------ |
| Sepal Length | Length of the sepal (cm) |
| Sepal Width  | Width of the sepal (cm)  |
| Petal Length | Length of the petal (cm) |
| Petal Width  | Width of the petal (cm)  |

### Target

* Species

## Requirements

Install the required Python packages:

```bash
pip install pandas scikit-learn matplotlib
```

## Project Structure

```text
project/
│
├── iris_pred.ipynb
├── data/
│   └── iris.csv
└── README.md
```

## Workflow

### 1. Load Dataset

The Iris dataset is loaded using Pandas.

```python
df = pd.read_csv('../data/iris.csv')
```

### 2. Prepare Features and Labels

```python
X = df.drop("species", axis=1)
y = df["species"]
```

### 3. Split Dataset

The dataset is divided into training and testing sets.

```python
train_test_split(
    X,
    y,
    test_size=0.2,
    random_state=42
)
```

### 4. Train Model

A Decision Tree Classifier is trained on the training data.

```python
clf = DecisionTreeClassifier(random_state=42)
clf.fit(X_train, y_train)
```

### 5. Evaluate Performance

Model performance is measured using classification accuracy.

```python
accuracy_score(y_test, y_pred)
```

### 6. Visualize Decision Tree

The trained decision tree is visualized to help understand how predictions are made.

```python
plot_tree(
    clf,
    feature_names=X.columns,
    class_names=clf.classes_,
    filled=True
)
```

### 7. Interactive Prediction

Users can manually enter flower measurements and receive a predicted species.

Example input:

```text
Sepal Length: 5.1
Sepal Width: 3.5
Petal Length: 1.4
Petal Width: 0.2
```

Example output:

```text
Predicted Species: Iris-setosa
```

## Machine Learning Algorithm

### Decision Tree Classifier

A Decision Tree is a supervised learning algorithm that:

* Learns decision rules from training data
* Splits data based on feature values
* Produces interpretable classification logic
* Supports multi-class classification tasks

## Results

The notebook evaluates the model on a held-out test set and reports classification accuracy.

Typical accuracy on the Iris dataset is above 90%, depending on the train-test split and model configuration.

## Learning Objectives

This project is suitable for beginners who want to learn:

* Supervised Machine Learning
* Classification problems
* Data preprocessing
* Model training with Scikit-learn
* Model evaluation
* Decision Tree visualization
* Interactive prediction workflows

## Author

Created as a machine learning practice project using Python and Scikit-learn.
