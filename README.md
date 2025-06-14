 Fake-News-Classify-NLP-Logistic-Regression-BERT

📌 Project Highlights

 - BERT-based classifier trained using HuggingFace's Transformers library.
 - Logistic Regression model using TF-IDF for efficient, interpretable prediction.
 - Explainability with LIME to highlight important words that influence predictions.
 - Custom data preprocessing for noise removal and vectorization.

Dataset Combines
 -Fake.csv
 -True.csv
  and each entry contains `title`, `text`, and a `label` (`0` = Fake, `1` = Real)

Technologies Used
  Python
  Pandas, NumPy, Matplotlib, Seaborn
  Scikit-learn
  HuggingFace Transformers (BERT)
  LIME (Local Interpretable Model-agnostic Explanations)
  Torch (PyTorch)

Model Overview

 1. Logistic Regression (Baseline Model)
 -TF-IDF vectorization (5000 features)
 -Accuracy: ~95%+
 -LIME used for word-based explanation

 2. BERT Fine-tuned Model
 -Tokenization using `bert-base-uncased`
 -Fine-tuned on custom dataset using `Trainer`
 -Robust performance on unseen news articles
