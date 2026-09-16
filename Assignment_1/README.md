# Assignment 1 – TensorFlow/Keras Setup, Data Preprocessing and Visualization

## Aim

To install and configure TensorFlow/Keras in Google Colab and perform data preprocessing, normalization, train-test splitting, and data visualization on a sample dataset.

## Objective

The objective of this assignment is to understand the basic workflow of a Deep Learning project, including:

- Installing and configuring TensorFlow/Keras in Google Colab
- Loading and exploring a sample dataset
- Checking for missing values
- Performing data preprocessing
- Normalizing the input features
- Splitting the dataset into training and testing sets
- Visualizing the dataset
- Building and evaluating a basic neural network model

## Dataset

The Heart Cleveland dataset is used in this assignment.

The dataset contains information related to heart disease and includes 297 samples with 14 columns.

### Dataset Details

- Number of samples: 297
- Number of columns: 14
- Number of input features: 13
- Target variable: `condition`
- Target values: 0 and 1
- Missing values: None

## Libraries Used

The following Python libraries are used:

- TensorFlow
- Keras
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Tasks Performed

### 1. TensorFlow/Keras Installation and Configuration

TensorFlow was installed and configured in Google Colab.

The TensorFlow version used was 2.20.0.

### 2. Dataset Loading

The Heart Cleveland dataset was loaded from an Excel file using Pandas.

### 3. Dataset Exploration

The dataset was explored using:

- `head()`
- `shape`
- `columns`
- `info()`
- `describe()`

### 4. Missing Value Checking

The dataset was checked for missing values using `isnull().sum()`.

No missing values were found in the dataset.

### 5. Data Preprocessing

The target variable `condition` was separated from the input features.

```python
X = df.drop("condition", axis=1)
y = df["condition"]
