# Assignment 6: Tomato Leaf Disease Classification Using CNN

## 1. Aim
To design and implement a Convolutional Neural Network (CNN) for image classification using a tomato leaf disease dataset.

## 2. Dataset
The Tomato Leaf Disease Dataset was downloaded from Kaggle.

- **Dataset:** Tomato Leaf Diseases Dataset
- **Number of classes:** 10
- **Total images used:** 3,000
- **Training images:** 2,400
- **Validation images:** 600
- **Image size:** 128 × 128 pixels

### Disease Classes
1. Bacterial Spot
2. Early Blight
3. Healthy
4. Late Blight
5. Leaf Mold
6. Mosaic Virus
7. Septoria Leaf Spot
8. Spider Mites
9. Target Spot
10. Yellow Leaf Curl Virus

To balance the dataset, 300 images were selected from each class.

## 3. Technologies Used
- Python
- Google Colab
- TensorFlow and Keras
- NumPy
- Matplotlib
- Scikit-learn
- Seaborn

## 4. Implementation Steps
1. Imported the required Python libraries.
2. Downloaded the tomato leaf disease dataset from Kaggle.
3. Explored the dataset and identified the 10 disease classes.
4. Selected 300 images from each class to create a balanced dataset.
5. Resized images to 128 × 128 pixels.
6. Split the dataset into training and validation sets.
7. Built a CNN model using TensorFlow and Keras.
8. Trained the CNN model for 10 epochs.
9. Evaluated the model using accuracy and loss.
10. Generated accuracy and loss graphs, a classification report, and a confusion matrix.

## 5. CNN Model Architecture
The CNN model uses the following layers:

- Rescaling Layer
- Convolutional Layer (32 filters, ReLU activation)
- Max Pooling Layer
- Convolutional Layer (64 filters, ReLU activation)
- Max Pooling Layer
- Convolutional Layer (128 filters, ReLU activation)
- Max Pooling Layer
- Flatten Layer
- Dense Layer (128 neurons, ReLU activation)
- Dropout Layer
- Output Dense Layer (10 neurons, Softmax activation)

## 6. Results
The model was trained for 10 epochs.

**Observed evaluation results:**
- Training Accuracy: approximately 88.75%
- Validation Accuracy: approximately 78.33%
- Test Accuracy: 78.33%
- Test Loss: 0.6616

The notebook also generates accuracy and loss graphs, a classification report, and a confusion matrix to evaluate the model's performance.

## 7. Conclusion
A Convolutional Neural Network was successfully designed and implemented for classifying tomato leaf diseases into 10 different categories. The model learned visual patterns from tomato leaf images and achieved an observed test accuracy of 78.33%.

This experiment demonstrates how deep learning and CNNs can be used for automated plant disease classification.

## 8. Tools and Platform
- Google Colab for implementation and model training.
- Kaggle for dataset acquisition.
- GitHub for assignment documentation and code storage.
