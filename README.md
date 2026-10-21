# Handwritten Digit Recognition Using CNN

## Project Overview

This project develops a Convolutional Neural Network (CNN) using TensorFlow and Keras to recognize handwritten digits (0–9) from images.

The model is trained and evaluated using the MNIST handwritten digit dataset.

## Objective

To develop a deep learning classification model capable of accurately recognizing handwritten digits using image processing and convolutional neural networks.

## Dataset

**Dataset:** MNIST Handwritten Digit Dataset

- Training images: 60,000
- Testing images: 10,000
- Image dimensions: 28 × 28 pixels
- Image format: Grayscale
- Number of classes: 10 (digits 0–9)

The images are normalized to the range 0–1 before training.

## CNN Model Architecture

The neural network consists of the following layers:

1. Conv2D — 32 filters, 3 × 3 kernel, ReLU activation
2. MaxPooling2D — 2 × 2
3. Conv2D — 64 filters, 3 × 3 kernel, ReLU activation
4. MaxPooling2D — 2 × 2
5. Flatten
6. Dense — 128 neurons, ReLU activation
7. Dropout — 0.3
8. Dense — 10 neurons, Softmax activation

**Total trainable parameters:** 225,034

## Model Training

| Parameter | Value |
|---|---|
| Optimizer | Adam |
| Loss Function | Sparse Categorical Crossentropy |
| Epochs | 5 |
| Batch Size | 64 |
| Validation Split | 10% |

## Model Performance

| Evaluation Metric | Result |
|---|---|
| Test Accuracy | **98.81%** |
| Test Loss | 0.0450 |
| Macro Average F1-Score | Approximately 0.99 |
| Test Samples | 10,000 |

The model correctly classified approximately 98.81% of the MNIST test images.

## Project Workflow

1. Import necessary Python libraries
2. Load the MNIST dataset
3. Visualize handwritten digit images
4. Normalize and preprocess image data
5. Build the CNN architecture
6. Compile and train the model
7. Evaluate model performance
8. Visualize accuracy and loss
9. Generate the confusion matrix and classification report
10. Predict handwritten digits
11. Save and reload the trained model

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## Installation

Install the required libraries:

`pip install -r requirements.txt`

## How to Run

1. Download or clone this GitHub repository.
2. Open `CodeAlpha_HandwrittenCharacterRecognition.ipynb` in Google Colab or Jupyter Notebook.
3. Install the required dependencies.
4. Run the notebook cells sequentially.
5. Review the training results, predictions, and evaluation metrics.

The MNIST dataset is automatically downloaded through TensorFlow/Keras.

## Project Files

| File | Description |
|---|---|
| CodeAlpha_HandwrittenCharacterRecognition.ipynb | Complete CNN implementation and evaluation |
| handwritten_digit_cnn.keras | Saved trained CNN model |
| requirements.txt | Python dependencies |
| README.md | Project documentation |

## Limitations

This model recognizes handwritten digits (0–9), not letters or complete words. It has been evaluated on MNIST and has not been validated for clinical, security-critical, or other high-stakes applications.

## Conclusion

The CNN model achieved **98.81% test accuracy** on the MNIST dataset, demonstrating the effectiveness of convolutional neural networks for handwritten digit recognition.

## Author

**Sadia Afrin Suchi**

Machine Learning Intern — CodeAlpha
