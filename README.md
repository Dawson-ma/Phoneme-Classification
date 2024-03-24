# Phoneme Classification

This project focuses on the classification of phonemes in speech signals. The model has demonstrated a notable accuracy rate of **74.82%** on the task.

## Data Preprocessing

The data underwent preprocessing to transform it into a 39-dimensional vector using mel-frequency cepstrum. Initially, the signal was converted into the frequency domain using Discrete Fourier Transform to obtain a spectrum. Subsequently, a filter bank, log transform, and Discrete Cosine Transform were applied to construct the vector. A window size of 25ms and a step size of 10ms were utilized. As a complete phoneme might not be contained within a 25ms window, 11 consecutive vectors were flattened into a 429-dimensional vector for model training. The processed dataset is stored [here](https://drive.google.com/file/d/1VVtc1chpLGlEst3h65eN1aX5V6iTl8qT/view?usp=drive_link).

## Neural Network

The neural network architecture is meticulously designed and implemented to effectively capture intricate patterns present in the data.

## Model Training

The constructed neural network undergoes rigorous training using the preprocessed dataset to optimize its parameters and attain the desired predictive performance.

## Phoneme Classification

An ensemble technique is employed to predict outcomes using ten randomly initialized neural network layer's length.

## Dataset

The TIMIT dataset serves as the primary data source for this project, accessible [here](https://academictorrents.com/details/34e2b78745138186976cbc27939b1b34d18bd5b3).  
  
For further details on the implementation and usage of the model, please refer to the [code](https://github.com/Dawson-ma/Phoneme-Classification/blob/main/PhonemeClassification.ipynb) provided.
