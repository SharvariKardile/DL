# Assignment 2 – Multilayer Perceptron for Wine Classification

## Aim

To design and implement a Multilayer Perceptron (MLP) for classification of the Wine dataset and evaluate its performance using accuracy and a confusion matrix.

## Objective

The objective of this assignment is to:

- Load and explore the Wine dataset.
- Preprocess the input features.
- Normalize the features using StandardScaler.
- Split the dataset into training and testing sets.
- Design a Multilayer Perceptron using TensorFlow/Keras.
- Train the MLP model.
- Evaluate the model using test accuracy.
- Generate and visualize a confusion matrix.

## Dataset

The Wine dataset from `sklearn.datasets` is used in this assignment.

### Dataset Details

- Number of samples: 178
- Number of input features: 13
- Number of classes: 3
- Classes: 0, 1, 2
- Classification type: Multiclass classification

## Libraries Used

- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Tasks Performed

### 1. Dataset Loading

The Wine dataset was loaded using `load_wine()` from Scikit-learn.

### 2. Data Preprocessing

The input features were separated from the target variable and standardized using `StandardScaler`.

### 3. Train-Test Splitting

The dataset was divided into training and testing sets using an 80:20 split.

### 4. MLP Model Design

A Multilayer Perceptron was designed using TensorFlow/Keras with the following architecture:

- Input layer: 13 features
- Hidden layer 1: 16 neurons with ReLU activation
- Hidden layer 2: 8 neurons with ReLU activation
- Output layer: 3 neurons with Softmax activation

### 5. Model Training

The MLP model was compiled using the Adam optimizer and sparse categorical cross-entropy loss and trained for 50 epochs.

### 6. Model Evaluation

The trained model was evaluated on the test dataset using classification accuracy.

The model achieved a test accuracy of approximately 97.22%.

### 7. Confusion Matrix

A confusion matrix was generated using the model's predictions on the test dataset and visualized using a heatmap.

## Result

The Multilayer Perceptron successfully classified the Wine dataset into three classes and achieved approximately 97.22% test accuracy.

The confusion matrix was also generated to analyze the classification performance of the model.

## Conclusion

A Multilayer Perceptron was successfully designed and implemented using TensorFlow/Keras for multiclass classification of the Wine dataset. The model was evaluated using test accuracy and a confusion matrix.
