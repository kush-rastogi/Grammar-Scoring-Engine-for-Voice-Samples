# Grammar-Scoring-Engine-for-Voice-Samples

# Project Summary: Grammar Scoring Engine using Wav2Vec2
This project implements a machine learning pipeline to automatically score spoken grammar on a scale of 0–5 using audio recordings. It leverages Facebook's Wav2Vec2 model for extracting meaningful speech representations, and uses a Random Forest classifier for predicting grammar proficiency levels.

# Key Components
Wav2Vec2 (facebook/wav2vec2-base-960h): Pretrained transformer model used to extract deep audio features from 16kHz sampled speech.

Feature Extraction: Audio files are processed into embeddings by averaging over Wav2Vec2 hidden states.

Label Encoding & Balancing: Grammar labels are encoded and the dataset is class-balanced using upsampling to handle class imbalance.

Random Forest Classifier: Trained on extracted features to predict discrete grammar scores.

# Evaluation Metrics:

Classification Report (Precision, Recall, F1-Score)

Root Mean Squared Error (RMSE)

Pearson Correlation Coefficient

Confusion Matrix

Boxplot of prediction distribution (replaces traditional histogram)

# Output
Evaluation results on validation data, showing classification performance and error metrics.

Boxplot visualizing the distribution of predicted scores grouped by true labels.

submission.csv file generated for test predictions, ready for leaderboard submission.

