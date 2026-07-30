# 🎬 IMDb Movie Review Sentiment Analysis using Classical NLP

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![NLP](https://img.shields.io/badge/NLP-TF--IDF-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

An end-to-end Natural Language Processing (NLP) project that classifies IMDb movie reviews as **Positive** or **Negative** using **TF-IDF** feature extraction and **Logistic Regression**.

Unlike many sentiment analysis projects that focus only on achieving high accuracy, this project emphasizes understanding the reasoning behind every preprocessing step, feature engineering decision, and model prediction. The classifier is designed to be both accurate and interpretable, making it suitable for learning classical NLP techniques and explaining model behavior during interviews.

---

## Table of Contents

- Project Overview
- Features
- Dataset
- Objectives
- Workflow
- Technologies Used
- Results
- Evaluation Beyond Accuracy
- Model Interpretation
- Key Learning Outcomes
- Repository Structure
- Installation
- How to Run
- Future Improvements
- License

## ✨ Features

- End-to-end Classical NLP pipeline
- HTML tag removal using BeautifulSoup
- Lowercasing and text normalization
- Contraction expansion
- URL and punctuation removal
- Lemmatization using NLTK
- Negation-aware stopword removal
- TF-IDF vectorization with unigrams and bigrams
- Logistic Regression classifier
- Comprehensive model evaluation
- Interpretation of learned feature coefficients
- Custom review prediction on unseen text

---

# 📊 Dataset

The project uses the **IMDb Movie Reviews Dataset**, containing **50,000** labeled movie reviews equally divided into positive and negative sentiments.

| Attribute | Details |
|-----------|---------|
| Dataset | IMDb Movie Reviews |
| Total Reviews | 50,000 |
| Classes | Positive, Negative |
| Class Distribution | Balanced (25,000 each) |
| Task | Binary Text Classification |

The balanced nature of the dataset makes it an excellent benchmark for evaluating traditional NLP techniques.

---

# 🎯 Project Objectives

The primary objectives of this project are:

- Build a complete end-to-end sentiment analysis pipeline.
- Understand the purpose of every preprocessing step.
- Transform raw text into numerical representations using TF-IDF.
- Train an interpretable machine learning classifier.
- Evaluate the classifier using multiple performance metrics.
- Analyze the learned feature importance instead of treating the model as a black box.

---

# ⚙️ Project Workflow

```text
IMDb Reviews
      │
      ▼
HTML Removal
      │
      ▼
Lowercasing
      │
      ▼
Contraction Expansion
      │
      ▼
URL Removal
      │
      ▼
Punctuation Removal
      │
      ▼
Lemmatization
      │
      ▼
Negation-aware Stopword Removal
      │
      ▼
TF-IDF Vectorization
      │
      ▼
Train-Test Split
      │
      ▼
Logistic Regression
      │
      ▼
Model Evaluation
      │
      ▼
Model Interpretation
```
---

# 🛠️ Technologies Used

| Category | Technologies |
|----------|--------------|
| Programming Language | Python |
| Data Manipulation | Pandas, NumPy |
| NLP | NLTK, BeautifulSoup, contractions |
| Feature Engineering | TF-IDF Vectorizer |
| Machine Learning | Logistic Regression (Scikit-learn) |
| Model Evaluation | Accuracy Score, Classification Report, Confusion Matrix |
| Visualization | Matplotlib |
| Development Environment | Jupyter Notebook, VS Code |

---

# 📈 Results

The Logistic Regression classifier achieved strong performance on the IMDb Movie Reviews dataset using TF-IDF features.

### Performance Summary

| Metric | Score |
|--------|-------|
| Accuracy | **89.9%** |
| Model | Logistic Regression |
| Feature Extraction | TF-IDF (Unigrams + Bigrams) |

### Confusion Matrix

<p align="center">
<img src="images/Confusion_matrix.png" width="500">
</p>

### Classification Report

<p align="center">
<img src="images/Classification_report.png" width="600">
</p>

### Performance Comparison

<p align="center">
<img src="images/Performance_table.png" width="700">
</p>

---

# 📊 Evaluation Beyond Accuracy

Rather than relying solely on accuracy, this project evaluates the classifier using multiple complementary metrics.

- **Accuracy** measures overall correctness.
- **Precision** evaluates how reliable positive and negative predictions are.
- **Recall** measures the model's ability to identify all relevant reviews for each class.
- **F1-score** provides a balanced measure of Precision and Recall.
- **Confusion Matrix** highlights the distribution of correct predictions and misclassifications.

Because the IMDb dataset is balanced, accuracy is an appropriate metric. However, combining these evaluation measures provides a more comprehensive assessment of model performance and reliability.

---

# 🧠 Model Interpretation

Most sentiment analysis projects stop after reporting the model's accuracy. This project goes one step further by analyzing **why** the model makes its predictions.

Since Logistic Regression is an interpretable machine learning algorithm, every TF-IDF feature receives a learned coefficient.

- Positive coefficients increase the probability of a **Positive** prediction.
- Negative coefficients increase the probability of a **Negative** prediction.
- Larger absolute coefficient values indicate stronger influence on the final prediction.

By examining these coefficients, the project identifies the most influential positive and negative words learned during training, providing valuable insights into the classifier's decision-making process instead of treating it as a black box.

---

# 🔍 Key Learning Outcomes

Throughout this project, I explored not only how to build a sentiment classifier but also why each design decision matters.

Key takeaways include:

- Understanding the role of text preprocessing in NLP.
- Preserving negation words to retain sentiment information.
- Comparing TF-IDF with simpler Bag-of-Words representations.
- Learning how Logistic Regression uses feature coefficients for prediction.
- Interpreting model decisions instead of focusing only on evaluation metrics.
- Building an end-to-end NLP pipeline suitable for real-world text classification tasks.

---

# 📂 Repository Structure

# 📂 Repository Structure

```text
Movie-Review-Sentiment-Analysis/
│
├── Dataset/
│   └── IMDB Dataset.csv
│
├── Notebook/
│   ├── 01_Classical_NLP/
│   │   ├── movie_review.ipynb
│   │   └── README.md
│   │
│   └── 02_BERT/
│       ├── movie_review_BERT.ipynb
│       └── README.md
│
├── images/
│   ├── Classical_NLP/
│   │    ├── Confusion_matrix.png
│   │    ├── Classification_report.png
│   │    └── Performance_table.png
│   │
│   └── BERT/
│       ├── Confusion_matrix.png
│       └── Classification_report.png
│
├── README.md
├── requirements.txt
├── .gitignore
└── LICENSE
```

---

# ⚙️ Installation

## Clone the repository

```bash
git clone https://github.com/ankith-b-kumar/IMBD-Movie-Reviews-Sentimental-Analysis-Classification-.git
cd Movie-Review-Sentiment-Analysis
```

## Install dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ How to Run

1. Clone the repository.
2. Install the required Python packages.
3. Open the notebook located in the `Notebook` directory.
4. Update the dataset path if necessary.
5. Run all notebook cells sequentially to reproduce the complete workflow.

The notebook covers:

- Data loading
- Text preprocessing
- Feature engineering using TF-IDF
- Model training
- Performance evaluation
- Model interpretation
- Prediction on custom reviews

---

# 🚀 Future Improvements

Potential enhancements for this project include:

- Compare Classical NLP with Transformer-based models such as BERT and DistilBERT.
- Perform hyperparameter tuning using GridSearchCV.
- Experiment with additional feature extraction techniques.
- Deploy the trained model as a web application using Streamlit or Flask.
- Extend the classifier to support multi-class sentiment analysis.

---

# 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

If you find a bug or have ideas to improve the project, feel free to open an issue or submit a pull request.

---

# 👨‍💻 Author

**B Ankith Kumar**

Computer Science Engineering (Data Science) Student

Interested in:
- Natural Language Processing (NLP)
- Machine Learning
- Data Analytics
- Generative AI

If you found this project helpful, consider giving it a ⭐ on GitHub.