# Dysarthric-Speech-to-Text
Smart speech-to-text system designed for slurred or impaired dysarthric speech. Helping voices be heard—clearly and confidently.

# Inspiration:
Conventional ASR systems often fail when used by individuals with speech impairments. This project was born out of a desire to bridge that accessibility gap—to make voice-driven technologies more inclusive by training models on real-world dysarthric speech data. The goal is simple but powerful: Everyone deserves to be understood.

# About the Project
This project aims to build a customized automatic speech recognition (ASR) system (without the use of any Pre-trained model) that can accurately transcribe dysarthric speech—a type of slurred or unintelligible speech caused by motor control issues due to neurological conditions.

I used a deep learning pipeline combining:

🧠 2D Convolutional Neural Networks (CNNs) to extract spatial features from spectrograms

🔁 Recurrent Neural Networks (RNNs) to model the temporal sequence of speech

🔗 Connectionist Temporal Classification (CTC) loss for aligning variable-length audio with text transcriptions without the need for manual alignment

This approach is inspired by DeepSpeech2, known for its robust performance on various speech styles and conditions.

I trained and tested the model on the TORGO dataset, which is specifically designed for dysarthric speech research. The dataset includes recordings from both dysarthric and control speakers, making it ideal for developing inclusive and accessible ASR systems.
For evaluation, I used Word Error Rate (WER)—a standard metric that calculates the number of substitutions, insertions, and deletions in the predicted transcription compared to the actual text. This is computed using the jiwer package.

# Dataset
This drive link contains all the audio files used for training the model : https://drive.google.com/drive/folders/159wAKlArcp2Jc-FxDZvfG0QWznU4QIVH?usp=drive_link
