# CodeAlpha_Emotion_Recognition_From_Speech
Emotion Recognition from Speech using MFCC features and CNN deep learning.

# Emotion Recognition from Speech using CNN

## Project Overview

This project is part of **CodeAlpha Machine Learning Task 2**.
The objective is to recognize human emotions from speech audio using **Machine Learning and Deep Learning techniques**.

The project processes `.wav` speech files, extracts **MFCC (Mel-Frequency Cepstral Coefficients)** features from the audio, and uses a **Convolutional Neural Network (CNN)** to classify the speech into different emotion categories.

## Objectives

* Process speech audio files.
* Extract useful speech features using MFCC.
* Build a CNN-based deep learning model.
* Classify speech into different emotion categories.
* Evaluate the model using accuracy, precision, recall, F1-score, and a confusion matrix.
* Predict the emotion of a new speech audio file.

## Dataset

The project uses the **RAVDESS-style Audio Speech Actors dataset** containing speech recordings from multiple actors.

### Dataset Details

* Number of actors: 24
* Number of audio files: 1,440
* Audio format: WAV
* Sampling rate: 16 kHz
* Number of emotion classes: 8

### Emotion Classes

| Code | Emotion   |
| ---- | --------- |
| 01   | Neutral   |
| 02   | Calm      |
| 03   | Happy     |
| 04   | Sad       |
| 05   | Angry     |
| 06   | Fearful   |
| 07   | Disgust   |
| 08   | Surprised |

## Technologies Used

* Python
* Google Colab
* NumPy
* Pandas
* Librosa
* Scikit-learn
* TensorFlow
* Keras
* Matplotlib
* Seaborn

## Methodology

The project follows these steps:

```text
Speech Audio
     ↓
Audio Loading
     ↓
Preprocessing
     ↓
MFCC Feature Extraction
     ↓
Feature Preparation
     ↓
Train/Test Split
     ↓
CNN Model
     ↓
Model Training
     ↓
Model Evaluation
     ↓
Emotion Prediction
```

## Feature Extraction

**MFCC (Mel-Frequency Cepstral Coefficients)** are extracted from each speech recording.

The extracted MFCC features are converted into a fixed-size representation so that they can be used as input to the CNN model.

## CNN Model

The CNN model contains:

* Convolutional layers
* Max Pooling layers
* Flatten layer
* Dense layer
* Dropout layer
* Softmax output layer

The final layer contains 8 output classes corresponding to the eight emotions.

## Model Evaluation

The model is evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

The actual performance values are reported based on the final training and testing results obtained in Google Colab.

## Results

After training, the model is evaluated on speech recordings from actors that were not included in the training data.

### Test Accuracy

**Add your actual Colab test accuracy here.**

Example:

```text
Test Accuracy: XX.XX%
```

### Evaluation Graphs

The project includes:

* Training vs Validation Accuracy
* Training vs Validation Loss
* Emotion Distribution
* MFCC Visualization
* Confusion Matrix

## Emotion Prediction

The trained CNN model can take a new `.wav` speech file and predict its most likely emotion.

Example:

```text
Input:
speech.wav

Output:
Predicted Emotion: Happy
Confidence: XX.XX%
```

## Project Files

```text
Task_2_Emotion_Recognition/
│
├── Task_2_Emotion_Recognition_CNN.ipynb
├── emotion_recognition_cnn.keras
├── emotion_label_encoder.pkl
├── README.md
└── results/
    ├── emotion_distribution.png
    ├── waveform.png
    ├── mfcc.png
    ├── accuracy.png
    ├── loss.png
    └── confusion_matrix.png
```

### Run the Notebook

Run the cells in order:

1. Install libraries
2. Import libraries
3. Upload and extract dataset
4. Prepare the dataset
5. Extract MFCC features
6. Train the CNN model
7. Evaluate the model
8. Test emotion prediction

## Conclusion

This project demonstrates how speech audio can be processed and classified using deep learning. MFCC features are extracted from speech recordings and used as input to a CNN model for emotion classification.

The project provides a complete workflow from **audio preprocessing and feature extraction to model training, evaluation, and emotion prediction**.

## Author

**Rahi Prajapati**

### Project

**CodeAlpha Machine Learning Internship – Task 2**

**Emotion Recognition from Speech using CNN**
