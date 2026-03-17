# Fake News Detection using Machine Learning

<p>
  <img src="https://img.shields.io/badge/Language-Python-3776AB?logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-F7931E?logo=scikitlearn&logoColor=white"/>
  <img src="https://img.shields.io/badge/NLP-TF--IDF-blue"/>
  <img src="https://img.shields.io/badge/Notebook-Jupyter-F37626?logo=jupyter&logoColor=white"/>
  <img src="https://img.shields.io/badge/Data-Pandas-150458?logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/Computation-NumPy-013243?logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/Visualization-Matplotlib-11557C"/>
  <img src="https://img.shields.io/badge/Visualization-Seaborn-4C72B0"/>
</p>

## Turning misinformation into a measurable classification problem

This project builds an end-to-end machine learning pipeline to classify news articles as **fake or real** using natural language processing and supervised learning techniques. The goal is to demonstrate how machine learning can be used to combat misinformation at scale.

## Why this project matters
Fake news spreads rapidly across social platforms, news channels, and online communities. Organizations in media, government, healthcare, and technology need scalable ways to identify misleading content before it affects public trust, decision‑making, or safety.

This project explores how classical machine learning can be used to detect misinformation with strong performance and interpretable evaluation metrics.

## Project snapshot
- **Course:** Machine Learning
- **Problem:** Binary text classification for fake news detection
- **Dataset:** WELFake dataset from Kaggle
- **Original size:** 72,134 news articles
- **Post-cleaning size:** 71,537 news articles after removing missing values
- **Best model:** Support Vector Machine (SVM)
- **Best result:** **93.4% accuracy** and **93.5% F1-score** on the test set

## Business value
This type of solution can support:
- **Social media platforms** by flagging suspicious articles or posts
- **Journalism teams** by assisting content verification workflows
- **Government and public-sector organizations** by monitoring misinformation trends
- **Healthcare organizations** by reducing the spread of harmful false claims

## What was built
This project implements a full NLP classification workflow from raw text to model comparison:

### 1. Data preprocessing
- Removed missing values from article title and text fields
- Verified duplicate rows
- Normalized text to lowercase
- Removed stopwords and non‑alphanumeric content
- Tokenized article text for downstream processing

### 2. Exploratory data analysis
- Compared fake vs real news distribution
- Analyzed title-length and text-length distributions
- Generated word frequency visualizations

### 3. Feature engineering
- Converted article text into numerical features using **TF‑IDF vectorization**

### 4. Model training
Three machine learning models were implemented and compared:

- Logistic Regression
- Multinomial Naive Bayes
- Support Vector Machine (SVM)

### 5. Model evaluation
Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC curves
- Confusion matrices

## Results

| Model | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| Logistic Regression | 91.4% | 91.2% | 89.8% | 90.5% |
| Naive Bayes | 84.2% | 85.2% | 83.6% | 84.4% |
| **Support Vector Machine** | **93.4%** | **92.9%** | **94.2%** | **93.5%** |

### Key takeaway
Among the evaluated models, **SVM delivered the strongest overall performance**, making it the best-performing classifier for this task.

## Technical highlights
- Applied **NLP preprocessing** to large-scale text data
- Used **TF‑IDF** to transform unstructured articles into machine learning features
- Compared multiple classification algorithms
- Evaluated model performance using confusion matrices and ROC curves
- Demonstrated a practical ML solution for misinformation detection

## Tech stack
- Python
- Pandas
- NumPy
- scikit-learn
- Matplotlib
- Seaborn
- NLTK
- spaCy
- WordCloud
- Jupyter Notebook

## Repository structure
```text
fake-news-detection-ml/
│
├── README.md
├── notebooks/
│   └── fake_news_detection.ipynb
├── report/
│   └── Fake News Detection Report.docx
├── presentation/
│   └── ML Presentation.pptx
└── data/
    └── dataset_link.txt
```

## Dataset
- **Source:** WELFake dataset
- **Link:** https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification

Instead of uploading the full dataset to GitHub, include the dataset link in:

data/dataset_link.txt

## How to run

1. Clone the repository
2. Download the dataset from Kaggle
3. Update the dataset path inside the notebook
4. Install dependencies
5. Run the notebook

Example:

pip install pandas numpy scikit-learn matplotlib seaborn nltk spacy wordcloud

## Future improvements
- Hyperparameter tuning for all models
- Using n‑grams and advanced text features
- Experimenting with deep learning models such as LSTM or Transformers
- Building a real‑time inference API for fake news detection

## Resume-ready impact statement
Built a fake news detection pipeline using NLP preprocessing, TF‑IDF vectorization, and supervised learning models on **71K+ news articles**, achieving **93.4% accuracy** and **93.5% F1-score** with SVM while comparing Logistic Regression and Naive Bayes using ROC curves and confusion matrices.
