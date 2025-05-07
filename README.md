# 🧠 Grammar Scoring Engine for Spoken English
This project focuses on developing a Grammar Scoring Engine that evaluates the grammatical correctness of spoken English using machine learning techniques. The engine is designed to predict a continuous grammar score ranging from 0 to 5, based on the Mean Opinion Score (MOS) Likert scale.

# 🎯 Objective
To build a system that automatically assesses the grammar quality of spoken language samples (each approximately 45–60 seconds long), enabling scalable and consistent evaluation for language learning and assessment applications.

# 📊 Dataset
Training Set: 444 audio samples

Testing Set: 195 audio samples

Each sample is labeled with a human-rated grammar score (0–5), following MOS guidelines.

# 🛠️ Methodology
Feature Extraction: Audio representations are extracted using Wav2Vec2, a state-of-the-art self-supervised speech model.

Modeling: A Random Forest Regressor is trained on the extracted features to predict the grammar scores.

Evaluation: The model is evaluated using standard regression metrics (e.g., MAE, RMSE, R²) to ensure accuracy and generalization.

