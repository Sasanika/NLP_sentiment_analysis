# Hate Speech Detection in Tweets

This project focuses on detecting hate speech in tweets using various machine learning models. The models are trained to classify tweets as either hate speech (racist/sexist) or non-hate speech.

## Project Structure

- `preprocessing.py`: Contains functions for data preprocessing including removing patterns, special characters, and short words.
- `feature_extraction.py`: Implements feature extraction using TF-IDF vectorization.
- `models.py`: Contains code for training and evaluating different machine learning models (Logistic Regression, SVC, Random Forest).
- `predict.py`: Script to preprocess, vectorize, and predict hate speech in new tweets using trained models.
- `README.md`: This file.

## Installation

1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <repository_directory>
2. Install packages:
   ```bash
   pip install -r requirements.txt
   
## Usage
### Training Models

Ensure the dataset Twitter_Sentiments.csv is placed in the project directory.
Run the training script to train the models:

```bash
  python models.py
```

## Predicting Hate Speech
Preprocess and predict hate speech for a single tweet:

```bash
  from predict import predict_hate_speech

tweet = "I hate this person! #racism"
prediction = predict_hate_speech(tweet)

print(prediction)
```

To predict multiple tweets, preprocess them and pass them to the predict_hate_speech function.

##mModel Evaluation
The models are evaluated using accuracy and F1-score metrics.

Logistic Regression: Achieved an accuracy of 94.7% and F1-score of 49.8%.
SVC: Achieved an accuracy of 94.3% and F1-score of 54.1%.
Random Forest: Achieved an accuracy of 95.0% and F1-score of 52.3%.

## Future Work
Explore more advanced preprocessing techniques.
Experiment with additional machine learning algorithms.
Fine-tune model parameters for better performance.

## Acknowledgments
NLTK and scikit-learn libraries for natural language processing and machine learning functionalities.
Kaggle for providing the dataset used in this project.
