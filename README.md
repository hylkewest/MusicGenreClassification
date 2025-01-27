
# Music Genre Classification

This repository contains the implementation of a music genre classification project, including feature extraction, model training, and evaluation.

## Environment Setup

1. Create a new conda environment:
   ```bash
   conda create --name musicgenreclassification python=3.10
   ```
2. Activate the environment:
   ```bash
   conda activate musicgenreclassification
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Project Structure

- **`dataset/`**: Contains the original dataset files downloaded from [Kaggle's GTZAN Dataset](https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification/data).

- **`checkpoints/`**: Stores model checkpoints during training.

- **`dataset_extracted/`**: Includes a CSV file with features extracted using our custom 3-second data extraction method.

- **`music_genre_classification_feature_extraction.py`**: Our implementation of the 3-second feature extraction method, resulting in the file found in `dataset_extracted`.

- **`music_genre_classification_training_1.py`**: Explores hyperparameter tuning and trains initial models on the original dataset's 3-second extracted features.

- **`music_genre_classification_training_2.py`**: Uses the hyperparameters from `training_1` to train new Feedforward Neural Networks (FFNNs) and Convolutional Neural Networks (CNNs) on our custom 3-second extracted features.

- **`music_genre_classification_evaluation.py`**: Generates graphs and visualizations from the final models for the report.

## Acknowledgments

- Dataset: [GTZAN Dataset - Music Genre Classification](https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification/data)