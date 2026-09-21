# Assignment 3 – Forward Propagation, Backpropagation and Hyperparameter Analysis

## Aim

To implement forward propagation and backpropagation using TensorFlow/Keras and analyze the effect of different learning rates and numbers of epochs on model performance.

## Objective

The objective of this assignment is to:

- Understand forward propagation in a neural network.
- Implement backpropagation using TensorFlow.
- Train a neural network using different learning rates.
- Analyze the effect of different numbers of epochs.
- Compare model performance using test accuracy.

## Dataset

The Iris dataset from `sklearn.datasets` is used in this assignment.

### Dataset Details

- Number of samples: 150
- Number of input features: 4
- Number of classes: 3
- Classes: Setosa, Versicolor, Virginica
- Classification type: Multiclass classification

## Libraries Used

- TensorFlow
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Tasks Performed

### 1. Dataset Loading

The Iris dataset was loaded using `load_iris()` from Scikit-learn.

### 2. Data Preprocessing

The input features were standardized using `StandardScaler`.

### 3. Train-Test Splitting

The dataset was divided into training and testing sets using an 80:20 split.

### 4. Neural Network Model

A neural network was created using TensorFlow/Keras with:

- Input layer: 4 features
- Hidden layer 1: 16 neurons with ReLU activation
- Hidden layer 2: 8 neurons with ReLU activation
- Output layer: 3 neurons with Softmax activation

### 5. Forward Propagation

During forward propagation, the input data was passed through the neural network to generate predictions.

### 6. Backpropagation

Backpropagation was implemented using TensorFlow's `GradientTape`. The gradients of the loss with respect to the trainable model parameters were calculated and used to update the weights.

### 7. Test Accuracy

The model was evaluated on the test dataset.

The initial model achieved a test accuracy of approximately 83.33%.

### 8. Learning Rate Analysis

The model was trained for 50 epochs using different learning rates.

| Learning Rate | Test Accuracy |
|---:|---:|
| 0.001 | 63.33% |
| 0.01 | 76.67% |
| 0.1 | 86.67% |

### 9. Epoch Analysis

The learning rate was fixed at 0.01 and the model was trained using different numbers of epochs.

| Epochs | Test Accuracy |
|---:|---:|
| 10 | 70.00% |
| 30 | 33.33% |
| 50 | 36.67% |
| 100 | 63.33% |

### 10. Visualization

Graphs were created to analyze:

- Effect of learning rate on test accuracy
- Effect of number of epochs on test accuracy

## Analysis

The experiments showed that changing the learning rate affected the test accuracy of the model. Among the tested learning rates, 0.1 produced the highest test accuracy of 86.67%.

The experiment with different numbers of epochs showed that increasing the number of epochs did not consistently improve test accuracy. The performance varied across the tested epoch values.

## Conclusion

Forward propagation and backpropagation were successfully implemented using TensorFlow/Keras. Experiments were performed using different learning rates and numbers of epochs, and their effects on model performance were analyzed using test accuracy.
