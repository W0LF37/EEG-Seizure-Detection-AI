# EEG Seizure Detection using Deep Learning

## Overview

This project presents a deep learning approach for detecting epileptic seizures from EEG signals.

The system converts raw EEG signals into time-frequency representations using Short-Time Fourier Transform (STFT), then applies EfficientNetB0 for classification.

## Methodology

Pipeline:

EEG Signal
↓
Signal Preprocessing
↓
STFT Transformation
↓
Spectrogram Image Generation
↓
EfficientNetB0 Feature Extraction
↓
Seizure Classification


## Dataset

Dataset:
Epileptic Seizure Recognition Dataset

The dataset contains EEG signal samples categorized into five classes.

## Model Architecture

- STFT-based signal representation
- EfficientNetB0 backbone
- Global Average Pooling
- Dense classification layers
- Softmax output


## Technologies

- Python
- TensorFlow / Keras
- EfficientNet
- Librosa
- OpenCV
- Scikit-learn


## Results

(Add your final accuracy here)

Evaluation metrics:
- Accuracy
- Classification Report
- Confusion Matrix


## Project Structure
notebooks/
src/
results/
models/


## Author

Mhd Adnan Lahham
Ahmad altabaa
