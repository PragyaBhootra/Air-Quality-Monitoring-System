# **Digit Recognizer Using MNIST Dataset**

## **Overview**
This project implements a Convolutional Neural Network (CNN) to recognize handwritten digits using the MNIST dataset. The model is trained to classify grayscale images of digits (0-9) and achieves high accuracy on the test set. The system also visualizes predictions and the performance of the model.

---

## **Features**
- Preprocesses the MNIST dataset by reshaping and normalizing image data.
- Implements a CNN for high accuracy digit recognition.
- Provides a visual interface to display test images and their predicted labels.
- Achieves high accuracy on the MNIST test dataset.

---

## **Requirements**
| Library        | Version (Recommended) |
|----------------|------------------------|
| TensorFlow     | 2.x                    |
| NumPy          | Latest                 |
| Matplotlib     | Latest                 |
| Python         | 3.x                    |

---

## **Project Structure**
1. **Data Loading**:
   - Loads the MNIST dataset directly from TensorFlow's dataset library.
2. **Preprocessing**:
   - Reshapes images into `(28, 28, 1)` for CNN compatibility.
   - Normalizes pixel values to the range `[0, 1]`.
3. **Model Definition**:
   - A Sequential CNN model with two convolutional layers, max pooling, dropout, and dense layers.
4. **Training**:
   - Trains the model using the Adam optimizer and sparse categorical cross-entropy loss.
5. **Evaluation**:
   - Evaluates the model on the test dataset for accuracy.
6. **Prediction**:
   - Predicts labels for test images and visualizes results.

---



