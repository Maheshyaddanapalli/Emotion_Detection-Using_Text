# Emotion_Detection-Using_Text
🌟 About This Project

Understanding emotions from text is an important part of Natural Language Processing. In this project, we built an emotion classification system that not only predicts emotions from text but also explains why a particular emotion was predicted.

Most models act like a black box. Our goal was to open that box and make the predictions transparent using Explainable AI techniques.

🎯 What We Tried to Solve

Can we accurately classify emotions from text?

Can we handle class imbalance properly?

Can we make machine learning predictions understandable to humans?

This project answers all three.

📚 Dataset Information

We combined two datasets:

• ISEAR Dataset – Contains emotions like Anger, Fear, Joy, and Sadness
• Emotion Sentiment Dataset – Contains multiple emotions such as Love, Happiness, Neutral, Hate, Surprise, Worry, etc.

After combining both datasets:

✔ Selected 2000 samples per class
✔ Created a balanced dataset
✔ Reduced bias caused by class imbalance

🧹 Data Cleaning Steps

Before training the model, we cleaned the text carefully:

🔹 Converted text to lowercase
🔹 Removed URLs and HTML tags
🔹 Removed emails and numbers
🔹 Removed punctuation and special characters
🔹 Removed stopwords
🔹 Cleared extra white spaces

This helped in making the data consistent and meaningful.

🧠 Feature Engineering

We converted text into numerical format using:

📌 TF-IDF with n-grams (1–3)
📌 Bag of Words with n-grams (1–3)

Using n-grams allowed us to capture not just single words but also meaningful word sequences.

🤖 Machine Learning Models Used

We experimented with multiple models to compare performance:

✔ XGBoost
✔ Support Vector Machine (Linear)
✔ Support Vector Machine (RBF)
✔ Random Forest
✔ Decision Tree
✔ Logistic Regression

Each model was evaluated to see which performed best for multi-class emotion classification.

🔎 Making the Model Explainable

This is the most important part of our project.

Instead of stopping at prediction, we used Explainable AI techniques:

💡 LIME

Explains individual predictions by highlighting which words influenced the result.

📊 SHAP

Provides both local and global explanations using Shapley values.
Shows how each feature contributes positively or negatively.

🧩 ANCHOR

Generates simple IF-THEN rules that explain predictions with high confidence.

These methods helped us understand the reasoning behind model decisions.
