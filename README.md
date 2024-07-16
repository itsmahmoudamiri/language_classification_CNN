# Audio Classification with VGG16

## Description

This project demonstrates how to classify audio segments into different languages (German, Farsi, and English) using a Convolutional Neural Network (CNN) based on the VGG16 architecture. The workflow involves converting audio segments into Mel-Spectrogram images and training a neural network to perform the classification.

## Project Overview

The goal of this project is to classify 1-second audio segments into one of three languages: German, Farsi, and English. The process involves the following steps:

1. Convert audio segments into frequency spectrum images using Mel-Spectrogram.
2. Use these images to train a VGG16-based Convolutional Neural Network (CNN) to classify the languages.

## Dataset

The dataset consists of audio files in German, Farsi, and English. These audio files are split into 1-second segments, and each segment is converted into a Mel-Spectrogram image.

## Pre-requisites

1. Python 3.6 or higher
2. TensorFlow 2.x
3. NumPy
4. Librosa
5. SciPy
6. Matplotlib
7. Seaborn
8. PIL (Pillow)
9. scikit-learn

## Usage

### Audio Processing

1. Convert audio segments into Mel-Spectrogram images:

- Adjust the path and output_path variables in AudioProcessor.ipynb to point to your audio files and desired output directory.
- Run the script to process the audio files and save the images: ./AudioProcessor.ipynb
  

### Model Training

2. Train the VGG16-based CNN model:

- Ensure your processed images are in the ./processed_data directory.
- Run the training script to train the model: ./ImageClassifier.ipynb
  

## Results

The model is evaluated on a test set, and the accuracy and confusion matrix are displayed. For example:

- Test accuracy: 0.87

The confusion matrix is visualized using a heatmap.

## Contributing

Contributions are welcome! Please create an issue to discuss any changes or improvements.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
