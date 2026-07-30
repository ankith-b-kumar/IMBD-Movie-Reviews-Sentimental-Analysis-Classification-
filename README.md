# 🚀 Movie Review Sentiment Analysis: From Classical NLP to BERT

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)
![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow)
![License](https://img.shields.io/badge/License-MIT-lightgrey)



## 📖 Repository Overview

This repository documents my learning journey in **Natural Language Processing (NLP)** through two complete implementations of sentiment analysis on the IMDb Movie Reviews dataset.

Rather than focusing solely on achieving high accuracy, the repository demonstrates the evolution of NLP techniques—from traditional feature engineering using TF-IDF and Logistic Regression to modern transformer-based models using Google's BERT.

Each implementation is self-contained with detailed documentation, allowing readers to understand both the methodology and the practical trade-offs between classical machine learning and deep learning approaches.



## 🎯 Why This Repository?

The goal of this project was not simply to classify movie reviews.

Instead, it was built to understand how modern NLP techniques solve real-world text classification problems and how the same approaches can be adapted to analyze customer opinions, product reviews, support tickets, survey responses, and other forms of unstructured business data.

The IMDb dataset serves as a benchmark that makes it easier to learn, compare, and validate different NLP methodologies before applying them to real-world business scenarios.


## 📈 Learning Journey

```text
Classical NLP
(TF-IDF + Logistic Regression)
            │
            ▼
Feature Engineering
            │
            ▼
Machine Learning Pipeline
            │
            ▼
Transfer Learning
            │
            ▼
Transformer-based NLP
(BERT)
```

This progression reflects how Natural Language Processing has evolved—from handcrafted textual features to contextual language understanding using transformer architectures.


## 📂 Repository Structure

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


## 📖 Explore the Implementations

| Implementation | Description |
|---------------|-------------|
| **01_Classical_NLP** | Traditional NLP pipeline using preprocessing, TF-IDF feature extraction, and Logistic Regression. Focuses on feature engineering and model interpretability. |
| **02_BERT** | Transformer-based sentiment analysis using Hugging Face Transformers and transfer learning with Google's `bert-base-uncased` model. Focuses on contextual language understanding and modern NLP workflows. |



## 💼 Business Applications

Although this repository uses the IMDb Movie Reviews dataset, the techniques demonstrated here extend far beyond movie reviews. Sentiment analysis is one of the most widely adopted Natural Language Processing (NLP) applications across industries where organizations need to understand large volumes of unstructured text.

Some practical business applications include:

| Industry | Potential Applications |
|----------|------------------------|
| 🛒 E-commerce | Analyze product reviews, identify recurring complaints, improve recommendations, and monitor customer satisfaction. |
| ☎️ Customer Support | Prioritize negative feedback, categorize support tickets, and identify common service issues. |
| 📱 Social Media | Monitor public opinion, measure campaign effectiveness, and track brand sentiment in real time. |
| 🏦 Banking & Finance | Analyze customer feedback on banking services, identify pain points, and measure customer experience. |
| 🏥 Healthcare | Evaluate patient feedback, improve service quality, and identify operational issues. |
| 🎬 Entertainment | Understand audience reactions, evaluate content performance, and improve recommendation systems. |



## 🎯 Why the IMDb Dataset?

The IMDb Movie Reviews dataset is one of the most widely used benchmark datasets for binary sentiment classification. It contains balanced, real-world reviews written by users, making it an excellent resource for learning and evaluating NLP techniques.

I selected this dataset because it allows me to focus on understanding the complete sentiment analysis workflow—from preprocessing and feature engineering to transformer-based transfer learning—without the additional complexity of domain-specific data.

More importantly, once these techniques are validated on a benchmark dataset, they can be adapted to business domains such as customer reviews, employee feedback, survey responses, social media posts, and support tickets with minimal changes to the overall pipeline.


## 🛠️ Tech Stack

| Category | Technologies |
|----------|--------------|
| Programming Language | Python |
| Machine Learning | Scikit-learn |
| Deep Learning | PyTorch |
| Transformer Models | Hugging Face Transformers |
| NLP | TF-IDF, WordPiece Tokenization, BERT |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib |
| Development Environment | Google Colab, VS Code |


## 🎯 What This Project Demonstrates

This repository goes beyond sentiment classification to showcase a practical learning journey in Natural Language Processing (NLP). It illustrates how NLP techniques have evolved from traditional feature engineering to transformer-based language models while emphasizing their applicability to real-world text analytics.

Through this project, I explored:

- The evolution, strengths, and trade-offs between classical machine learning and transformer-based NLP approaches.
- End-to-end sentiment analysis workflows using both traditional and modern NLP techniques.
- Model evaluation using multiple performance metrics beyond overall accuracy.
- Transfer learning through fine-tuning a pre-trained BERT model.
- Building reusable NLP pipelines that can be adapted to business scenarios involving customer feedback and other forms of unstructured text.

Although the implementation uses the IMDb Movie Reviews dataset as a benchmark, the underlying methodologies are transferable to enterprise applications such as customer feedback analysis, product reviews, support ticket classification, and brand sentiment monitoring.


## 🚀 Future Scope

This repository serves as a foundation for exploring more advanced NLP applications. Potential future enhancements include:

- Fine-tuning larger transformer models such as RoBERTa and DeBERTa.
- Multi-class sentiment and emotion classification.
- Aspect-Based Sentiment Analysis (ABSA).
- Explainable AI techniques for transformer models.
- Deployment as an interactive web application using Streamlit.
- Integration with real-time customer feedback or social media data.


## 👨‍💻 Author

**B Ankith Kumar**

Computer Science Engineering (Data Science) Student

**Areas of Interest**

- Artificial Intelligence
- Machine Learning
- Natural Language Processing
- Data Analytics
- Generative AI

If you found this repository useful, consider giving it a ⭐ on GitHub.