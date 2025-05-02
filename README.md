# Music Genre Classification Project Using Deep Learning

🎶 Hello and welcome to the directory for the Music Genre Classification Project! This repository contains Python code and other resources how to use deep learning based approaches to recognize musical genres using audio data. It combines convolutional neural networks (CNNs) and recurrent neural networks (RNNs) to pick up on patterns in sound to classify music automatically. Feel free to dive in and explore the code!

## Project Overview

Throughout history, music has been a powerful tool in culture, as a source of entertainment and expression of personal identity. Given the importance of music, this project aims to streamline music discovery and help develop a more organized personal music experience, through the creation of a music genre classification program that will automatically identify the genre of a given piece of music. 

## Approach

### 1. Data Collection & EDA

The GTZAN dataset (available on Kaggle) was used. It contains 10 genres: blues, classical, reggae, country, disco, hiphop, jazz, metal, pop, and rock. Each genre consists of 100 audio clips, each 30 seconds long and stored in WAV format. 

The library librosa was used for the primary audio loading and pydub to handle any loading exceptions, ensuring robustness with any format inconsistencies.

### 2. Model Architecture 

Convolutional Neural Networks (CNNs) were utilized to learn patterns from spectrograms and tempograms, visual representations of music automatically developed for this purpose. The networks process the data through convolution, ReLU, dropout, and pooling layers to abstract and reduce spatial variability. 

Recurrent Neural Networks (RNNs) were used to capture the temporal features in the audio signals, focusing on musical dynamics and rhythmic characteristics.

When combined, classification accuracy was improved and ensured optimal model performance.

![ModelArchitecture](https://github.com/user-attachments/assets/f8963ddc-6cd0-4988-a93b-052671b1fed5)

Figure 1. Model Architecture

### 3. Training & Evaluation

The model was trained, validated, and tested using the dataset. Training involved tuning various hyperparameters to achieve the best performance. The final model achieved accuracies of 77.80%, 61.81%, and 79.60% in training, validation, and testing datasets, respectively.

<img width="576" alt="Accuracy Plot" src="https://github.com/user-attachments/assets/d9067b4a-0fe1-4c99-aff5-868871971629" />

Figure 2: Plot of Train vs. Validation Accuracy

### Front End Results

To present the qualitative results of the model, an interactive front-end was designed. Readers can input an audio file (e.g., a file with a .wav extension) and receive a genre classification utilizing the model with a certain degree of accuracy. The following diagram illustrates the steps taken when a piece of disco genre music is uploaded to the model and correctly classified.

<img width="991" alt="Diagram" src="https://github.com/user-attachments/assets/9dbe4993-893a-42b3-9342-9a4666f477b8" />

## Acknowledgements

- [GTZAN dataset](https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification) from Kaggle.
- Libraries used: 
  - [librosa](https://librosa.org/): A Python package for music and audio analysis.
  - [pydub](https://pydub.com/): A library for manipulating audio with a simple and easy-to-use interface.
  - [TensorFlow](https://www.tensorflow.org/): An open-source platform for building and deploying machine learning models.
  - [PyTorch](https://pytorch.org/): A framework for building deep learning models and is commonly used in applications like image recognition and language processing.
