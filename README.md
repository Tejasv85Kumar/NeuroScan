# NeuroScan: Brain Tumor Classification using CNN #
## 1. Project Overview ##
The primary objective of this project is to develop a deep learning model capable of identifying the presence of a brain tumor from Magnetic Resonance Imaging (MRI) scans. By leveraging Convolutional Neural Networks (CNN), the model automates the classification process into two categories: Tumor (Yes) and No Tumor (No).

## 2. Dataset Description ##
The model is trained on the Brain MRI Images for Brain Tumor Detection dataset.

Class 0 (No): MRI scans showing no signs of a brain tumor.

Class 1 (Yes): MRI scans indicating the presence of a tumor.

## 3. Technical Stack ##
Language: Python 3

Framework: Keras / TensorFlow

Libraries:  NumPy, Pandas for data manipulation.

Matplotlib, PIL (Pillow) for image processing and visualization.

Scikit-learn for data splitting and preprocessing.

## 4. Model Architecture ##
The project utilizes a Sequential CNN model designed for binary classification. Key layers include:

Convolutional Layers (Conv2D): Extracts spatial features from the MRI images.

Pooling Layers (MaxPooling2D): Reduces dimensionality while preserving important features.

Batch Normalization: Accelerates training and stabilizes the learning process.

Dropout: Prevents overfitting by randomly deactivating neurons during training.

Dense Layers: Fully connected layers leading to the final output classification.

## 5. Implementation Workflow ##
Data Preprocessing: Images are resized to a uniform dimension (128x128) and normalized. One-hot encoding is applied to the labels.

Data Splitting: The dataset is divided into training and testing sets (80/20 split) to evaluate the model's performance on unseen data.

Training: The model is trained using the training partition, with validation monitoring to track accuracy and loss.

Evaluation: Performance is visualized through loss and accuracy plots.

Prediction: A dedicated function processes new MRI images to provide a classification result with a confidence score.

## 6. How to Use ##
Environment Setup: Ensure you have Python installed along with the required libraries:

Bash
pip install tensorflow pandas matplotlib pillow scikit-learn
Dataset: Download the dataset from Kaggle and ensure the file paths in the notebook match your local directory structure.

Run the Notebook: Execute NeuroScan.ipynb to train the model and generate predictions.

## 7. Results ##
The model generates a classification output indicating whether a tumor is detected or not, alongside a confidence percentage. Visualization of the training history is provided to demonstrate the model's convergence over time.
