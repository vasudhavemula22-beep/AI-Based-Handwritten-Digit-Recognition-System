 AI-Based Handwritten Digit Recognition System
 
A deep learning project that uses Convolutional Neural Networks (CNNs) to classify handwritten digits (0–9) from image data. This project demonstrates the power of CNNs in computer vision and optical character recognition (OCR) applications.

 Overview:
This project builds a CNN model to identify handwritten digits using the MNIST dataset. It includes:

Data preprocessing and normalization
CNN model architecture and training
Model evaluation with accuracy, loss curves, and confusion matrix
Optional comparison with a Multilayer Perceptron (MLP)
Custom image prediction interface

Features:
 Data Preprocessing: Load and normalize MNIST dataset (60,000 training + 10,000 test images)
 CNN Model: Build and train a Convolutional Neural Network for digit classification
 Model Evaluation: Accuracy, loss curves, confusion matrix, and classification report
 MLP Comparison: Optional comparison with a simple Multilayer Perceptron model
 Prediction Interface: Upload and classify custom handwritten digit images
 Visualization: Display sample images, training curves, and prediction results

 Technologies Used:

Python 3.7+

Programming Language: TensorFlow/Keras 2.11+

Deep Learning Framework:
NumPy
Numerical Computing
Matplotlib
Data Visualization
Scikit-learn
Model Evaluation Metrics
Seaborn
Confusion Matrix Visualization
Pillow (PIL)
Image Processing

 Installation:
Prerequisites
Python 3.7 or higher
Jupyter Notebook or Google Colab
pip (Python package manager)

Install Dependencies:
pip install tensorflow numpy matplotlib scikit-learn seaborn pillow

 How to Run:
 Google Colab
Upload the .ipynb file to Google Drive
Open in Google Colab
Run all cells

 Results:
CNN Performance
Metric
Value
Test Accuracy
~98.5%

Test Loss
~0.028

Training Epochs
10

Batch Size
128

MLP Performance
Metric
Value
Test Accuracy
~97.0%
Test Loss
~0.052

 Sample Outputs:
Training Curves

Confusion Matrix

Prediction Interface

 Usage Example
Predict a Custom Image

# Load the model
from tensorflow.keras.models import load_model
model = load_model('mnist_cnn_model.keras')

# Predict a digit
predict_digit(r'C:\Users\sriha\Downloads\sample_digit.png', invert=False)
Output

Copy code
Predicted Digit: 2
Confidence: 95.67%
Top 3 Predictions:
  1. Digit 2: 95.67%
  2. Digit 3: 3.21%
  3. Digit 5: 1.12%

 Report:
A detailed project report is included in the repository:

Dataset Overview: MNIST dataset details and preprocessing
Model Architecture: CNN and MLP layer descriptions
Accuracy Results: Test accuracy, loss curves, confusion matrix
Conclusion: Key findings and future improvements

# Important:
Change the path of the sample_digit.png which is used for testing the model:
'predict_digit(r'C:\Users\sriha\Downloads\sample_digit.png')- to your own path in your system'

 Quick Start Commands:

# Install dependencies
pip install tensorflow numpy matplotlib scikit-learn seaborn pillow

# Run the notebook
jupyter notebook Handwritten_Digit_Recognition.ipynb

# Run prediction
python predict_digit.py
