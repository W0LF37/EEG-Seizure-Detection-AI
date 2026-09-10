# EEG Seizure Detection using Deep Learning

![STFT Representation](results/stft_samples.png)

## Overview

This project presents a deep learning approach for epileptic seizure classification using EEG (Electroencephalography) signals.

The proposed pipeline transforms raw EEG signals into time-frequency representations using Short-Time Fourier Transform (STFT), then applies a convolutional neural network based on EfficientNetB0 to classify different EEG signal categories.

The project explores the application of deep learning techniques in biomedical signal processing and healthcare AI.

---

## Problem Statement

Epileptic seizure detection from EEG signals is a challenging task due to the complexity and variability of brain activity patterns.

Traditional EEG analysis requires expert interpretation, which motivates the use of automated deep learning approaches capable of extracting meaningful patterns from signal data.

This project investigates how signal transformation and deep learning models can support automated EEG classification.

---

## Methodology

The complete workflow consists of the following stages:

```
Raw EEG Signal
       ↓
Signal Preprocessing
       ↓
STFT Transformation
       ↓
Spectrogram Generation
       ↓
EfficientNetB0 Feature Extraction
       ↓
Multi-Class Classification
```

### Signal Processing

- Raw EEG signals are converted into time-frequency representations using Short-Time Fourier Transform (STFT).
- Generated spectrograms are resized and prepared as image inputs for the deep learning model.

### Deep Learning Model

The classification model is based on EfficientNetB0:

- EfficientNetB0 feature extraction backbone
- Global Average Pooling layer
- Fully connected classification layers
- Softmax output layer for multi-class prediction

---

## Dataset

**Dataset:** Epileptic Seizure Recognition Dataset

The dataset contains EEG signal samples categorized into five different classes.

The signals are transformed into spectrogram representations before being used for model training.

---

## Model Architecture

The proposed architecture:

```
EEG Signal
    ↓
STFT Spectrogram
    ↓
EfficientNetB0
    ↓
Global Average Pooling
    ↓
Dense Layer
    ↓
Softmax Classification
```

---

## Technologies

- Python
- TensorFlow / Keras
- EfficientNet
- Librosa
- OpenCV
- Scikit-learn
- NumPy
- Pandas

---

## Results

The model performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

### Confusion Matrix

![Confusion Matrix](results/confusion_matrix.png)

### Training Performance

![Learning Curves](results/learning_curves.png)

---

## Project Structure

```
EEG-Seizure-Detection-AI/

├── EEG_Seizure_Detection.ipynb
├── README.md
├── requirements.txt
│
└── results/
    ├── stft_samples.png
    ├── confusion_matrix.png
    └── learning_curves.png
```

---

## Key Highlights

- EEG signal processing using STFT transformation
- Spectrogram-based deep learning classification
- EfficientNetB0 implementation for biomedical signal analysis
- Multi-class EEG pattern recognition
- Visualization of model performance and predictions

---

## Future Improvements

Possible improvements include:

- Using pretrained EfficientNet weights through transfer learning
- Testing additional deep learning architectures
- Applying data augmentation techniques
- Evaluating on larger EEG datasets
- Developing a real-time EEG monitoring pipeline

---

## Project Context

This project was developed as part of university coursework to explore deep learning applications in biomedical signal processing.

---

## Author

**Mhd Adnan Lahham**  
**Ahmad Altabaa**
