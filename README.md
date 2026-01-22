# Multi-Class-Arrhythmia-Diagnosis-and-classification-with-Deep-Learning
ECG Arrhythmia Classification Using CNN-BiLSTM with Attention

Introduction

This project focuses on automatic detection of cardiac arrhythmias using deep learning. ECG signals are analyzed using a hybrid CNN-BiLSTM model with an Attention mechanism to classify different heart rhythm conditions accurately.

Objectives

Automate ECG arrhythmia detection

Extract spatial and temporal ECG features

Improve classification accuracy using Attention

Support multi-class prediction

Dataset

Source: PhysioNet 12-Lead ECG Dataset

Total Records: 45,152

Sampling Rate: 500 Hz

Input Size: 12 × 5000

Target Classes

Sinus Bradycardia (SB)

Sinus Rhythm (SR)

Sinus Tachycardia (ST)

Atrial Flutter (AFL)

Atrial Fibrillation (AFIB)

Model Architecture

The system uses:

CNN with ResNet and SE blocks for feature extraction

BiLSTM for temporal pattern learning

Attention layer to focus on important signals

Softmax classifier for output prediction

Implementation

Language: Python

Framework: PyTorch

Platform: Google Colab

GPU: NVIDIA T4

Epochs: 35

Batch Size: 64

Results

Overall Accuracy: 91%

High performance for sinus rhythm classes

Minor confusion between AFIB and AFL

How to Run

Install dependencies:

pip install torch numpy pandas matplotlib wfdb

Run training:

python train.py

Conclusion

The project successfully demonstrates a deep learning-based approach for ECG arrhythmia classification. The hybrid architecture improves accuracy and provides an efficient automated diagnostic solution.
