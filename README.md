# Twitter-Sentiment-Analysis-System
# Project Description
This project implements a sentiment analysis system using various Convolutional Neural Network (CNN) architectures. The model is trained to classify the sentiment of text data as either positive or negative.

## Dataset
The dataset used is the Sentiment140 dataset, which contains 1.6 million tweets labeled as positive or negative.

## Techniques and Tools Used
#### Data Preprocessing
The Sentiment140 dataset is loaded and shuffled to ensure randomness. Sentiment labels are adjusted to binary values (0 for negative and 1 for positive). Text data is preprocessed by converting to lowercase, removing punctuation, numbers, and stopwords, tokenizing the text, and retaining unique words longer than three characters.

#### Feature Extraction
Word Embeddings: FastText pre-trained embeddings are used to represent words as dense vectors.
Padding Sequences: Embedded word sequences are padded to ensure consistent input length for the CNN models.

#### Model Architectures
1. CNN with Multiple Kernel Sizes:
A custom CNN model with multiple kernel sizes (2, 3, 5) to capture various n-gram features.
Uses Conv1D layers followed by Dropout and BatchNormalization.
Outputs are concatenated and passed through a dense layer with sigmoid activation.

2. Custom CNN Module:
A function to create a CNN module with various Conv1D layers and pooling operations.
Uses multiple Conv1D layers with different kernel sizes to capture diverse features.
Outputs are concatenated and passed through a dense layer.

3. VGG-16 Model Architecture

## Model Training and Evaluation
Models are trained using the binary cross-entropy loss function and the Adam optimizer and evaluated on a test set using classification reports and confusion matrices.

## Results
Classification Reports: Detailed classification reports are generated for each model, displaying precision, recall, and F1-score for both classes.
Confusion Matrices: Confusion matrices are plotted to visualize the performance of the models.

#### Feel free to explore, modify, and extend this project to suit your needs. Happy coding!
