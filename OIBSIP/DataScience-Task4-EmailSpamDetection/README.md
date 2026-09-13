# 📧 Email Spam Detection

<div align="center">

## Oasis Infobyte — Data Science Internship

### 📩 Task 4: Email Spam Detection Using Machine Learning

**👨‍💻 Author:** Himanshu Chavda

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical-blue?logo=numpy)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E?logo=scikitlearn)
![NLTK](https://img.shields.io/badge/NLTK-NLP-success)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-success)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-4B8BBE)
![WordCloud](https://img.shields.io/badge/WordCloud-Visualization-purple)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)

</div>

---

# 📑 Table of Contents

- Project Overview
- Objective
- Dataset Information
- Project Workflow
- Technologies Used
- Text Preprocessing
- Exploratory Data Analysis
- Feature Extraction
- Machine Learning Models
- Model Evaluation
- WordCloud Visualization
- Project Structure
- Results
- Key Insights
- Future Improvements
- License
- How to Run
- Author

---

# 📌 Project Overview

This project develops an end-to-end Natural Language Processing (NLP) system capable of classifying SMS messages as **Spam** or **Ham (Legitimate)** using Machine Learning.

The notebook follows a complete Data Science workflow beginning with dataset validation, exploratory data analysis, professional text preprocessing, TF-IDF feature extraction, model training, evaluation, visualization, and final model selection.

Two classification algorithms are trained and compared to determine the best-performing spam detection model.

---

# ✨ Project Highlights

✔ Complete NLP Pipeline

✔ Professional Data Validation

✔ Data Cleaning

✔ Text Preprocessing

✔ Stopword Removal

✔ Porter Stemming

✔ TF-IDF Feature Extraction

✔ Exploratory Data Analysis (EDA)

✔ Multinomial Naive Bayes

✔ Logistic Regression

✔ Model Comparison

✔ Confusion Matrix

✔ Classification Report

✔ WordCloud Visualization

✔ Saved Trained Model (.pkl)

✔ Professional Documentation

---

# 📦 Requirements

Install all required libraries:

```bash
pip install -r requirements.txt
```

Libraries used:

- pandas
- numpy
- matplotlib
- seaborn
- nltk
- scikit-learn
- wordcloud
- joblib
- jupyter

---

# 🎯 Objective

The primary objective of this project is to build an intelligent Machine Learning model capable of accurately distinguishing spam SMS messages from legitimate messages.

The project includes:

- Dataset Validation
- Data Cleaning
- Exploratory Data Analysis
- Text Preprocessing
- TF-IDF Vectorization
- Machine Learning Model Building
- Performance Evaluation
- Model Comparison
- WordCloud Visualization

---

# 📂 Dataset Information

Dataset Used:

**SMS Spam Collection Dataset**

The dataset contains real-world SMS messages labeled as either:

- Ham (Legitimate)
- Spam

### Dataset Features

| Feature | Description |
|----------|-------------|
| label | Target variable (ham / spam) |
| message | SMS text message |

---

# 🔬 Project Workflow

```text
Load Dataset
      │
      ▼
Dataset Validation
      │
      ▼
Data Cleaning
      │
      ▼
Missing Value Analysis
      │
      ▼
Duplicate Removal
      │
      ▼
Text Preprocessing
      │
      ▼
Lowercase Conversion
      │
      ▼
Remove Punctuation
      │
      ▼
Remove Numbers
      │
      ▼
Stopword Removal
      │
      ▼
Porter Stemming
      │
      ▼
TF-IDF Vectorization
      │
      ▼
Train-Test Split
      │
      ▼
Multinomial Naive Bayes
      │
      ▼
Logistic Regression
      │
      ▼
Model Evaluation
      │
      ▼
Model Comparison
      │
      ▼
WordCloud Visualization
      │
      ▼
Save Best Model
      │
      ▼
Conclusion
```

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| Pandas | Data Cleaning & Analysis |
| NumPy | Numerical Computing |
| NLTK | Natural Language Processing |
| Regular Expressions | Text Cleaning |
| TF-IDF | Feature Extraction |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Visualization |
| WordCloud | Keyword Visualization |
| Scikit-Learn | Machine Learning |
| Joblib | Model Serialization |
| Jupyter Notebook | Development Environment |

---

# 🧹 Text Preprocessing

The raw SMS messages were cleaned using a professional NLP preprocessing pipeline.

The preprocessing steps include:

- Convert text to lowercase
- Remove punctuation
- Remove numbers
- Remove extra spaces
- Remove stopwords
- Apply Porter Stemming

Example:

```text
Original:

WINNER!! Claim your FREE prize now!!!

↓

Processed:

winner claim free prize
```

---

# 📊 Exploratory Data Analysis

The notebook includes:

- Dataset Inspection
- Missing Value Analysis
- Duplicate Record Analysis
- Class Distribution
- Pie Chart
- Count Plot
- Message Length Distribution
- Spam vs Ham Comparison

---

# 📝 TF-IDF Feature Extraction

TF-IDF stands for:

**Term Frequency – Inverse Document Frequency**

It measures how important a word is within an individual SMS message compared to all messages in the dataset.

Common words receive lower importance while informative words receive higher weights.

The cleaned text was converted into a sparse numerical matrix using:

```python
TfidfVectorizer()
```

This matrix becomes the input for Machine Learning algorithms.

---

# 🤖 Machine Learning Models

Two classification algorithms were implemented.

## 1️⃣ Multinomial Naive Bayes

A probabilistic classifier widely used for text classification.

Advantages:

- Extremely fast
- Excellent baseline model
- Performs well on sparse TF-IDF features

---

## 2️⃣ Logistic Regression

A linear classification algorithm capable of producing highly accurate predictions for binary classification tasks.

Advantages:

- High accuracy
- Robust performance
- Better decision boundaries
- Strong generalization capability

---

# 📈 Model Evaluation

The models were evaluated using:

| Metric | Purpose |
|---------|----------|
| Accuracy | Overall prediction accuracy |
| Precision | Correct spam predictions |
| Recall | Ability to detect spam |
| F1 Score | Balance of Precision & Recall |
| Confusion Matrix | Classification visualization |
| Classification Report | Detailed evaluation |

The best-performing model was selected based on:

- Highest Accuracy
- Highest Precision
- Highest Recall
- Highest F1 Score

---

# 🏆 Model Performance

| Model | Accuracy | Precision | Recall | F1 Score |
|-------|---------:|----------:|-------:|---------:|
| Multinomial Naive Bayes | XX.XX% | XX.XX% | XX.XX% | XX.XX% |
| Logistic Regression | XX.XX% | XX.XX% | XX.XX% | XX.XX% |

✅ **Best Model:** Logistic Regression *(Replace after training if different.)*

---

# 💼 Real-World Applications

The developed spam detection system can be used in:

- 📩 Email Filtering Systems
- 📱 SMS Spam Detection
- 🏦 Banking Fraud Alert Systems
- 🛒 E-commerce Notification Filtering
- 📞 Telecommunication Services
- 🤖 AI-powered Messaging Platforms

---

# ☁️ WordCloud Visualization

The notebook generates two professional WordClouds:

- Spam Messages
- Ham Messages

These visualizations highlight the most frequently occurring words in each category.

---

# 📁 Project Structure

```text
DataScience-Task4-EmailSpamDetection/
│
├── 📂 data/
│   └── spam.csv
│
├── 📂 images/
│   ├── class_distribution_pie.png
│   ├── class_distribution.png
│   ├── confusion_matrix_logistic_regression.png
│   ├── confusion_matrix_naive_bayes.png
│   ├── ham_wordcloud.png
│   ├── model_comparison.png
│   ├── sms_message_class_distribution.png
│   └── spam_wordcloud.png
│
├── 📂 notebook/
│   └── email_spam_detection.ipynb
│
├── 📂 outputs/
│   └── cleaned_spam_dataset.csv
│
├── README.md
└── requirements.txt
```

---

# 📷 Project Visualizations

## 📊 Class Distribution

```text
images/class_distribution.png
```

---

## ☁️ Spam WordCloud

```text
images/spam_wordcloud.png
```

---

## ☁️ Ham WordCloud

```text
images/ham_wordcloud.png
```

---

## 📉 Naive Bayes Confusion Matrix

```text
images/nb_confusion_matrix.png
```

---

## 📉 Logistic Regression Confusion Matrix

```text
images/lr_confusion_matrix.png
```

---

## 📈 Model Comparison

```text
images/model_comparison.png
```

---

# 📈 Results

The project successfully developed a Machine Learning model capable of accurately classifying SMS messages as spam or legitimate.

Both classification algorithms were trained and evaluated using identical datasets and performance metrics.

Among the evaluated models, the best-performing classifier demonstrated superior accuracy and F1-score while maintaining excellent recall for spam detection.

The trained model was exported for future inference using Joblib.

---

# 💡 Key Insights

- Spam messages frequently contain promotional and urgent words.
- Proper text preprocessing significantly improves classification accuracy.
- TF-IDF effectively converts text into numerical representations.
- Logistic Regression generally achieves higher overall accuracy.
- Naive Bayes offers excellent speed and competitive performance.
- Recall is critical because missing spam messages may expose users to scams or malicious content.
- WordCloud visualization provides intuitive insights into common vocabulary.

---

# 🚀 Future Improvements

Potential enhancements include:

- Hyperparameter Tuning using GridSearchCV
- Support Vector Machine (SVM)
- XGBoost Classifier
- Deep Learning (LSTM)
- BERT Transformer Models
- K-Fold Cross Validation
- SHAP Explainability
- Interactive Streamlit Dashboard
- Flask/FastAPI REST API
- Docker Containerization
- CI/CD with GitHub Actions

---

# 📄 License

This project was developed for educational purposes as part of the **Oasis Infobyte Data Science Internship Program**.

---

# ▶️ How to Run

Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Navigate to the project folder:

```bash
cd DataScience-Task4-EmailSpamDetection
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
notebook/email_spam_detection.ipynb
```

Run all notebook cells from top to bottom.

---

# 🤝 Connect with Me

**Himanshu Chavda**

💼 Business Analyst | Data Analyst | Data Science | Machine Learning | Artificial Intelligence

- GitHub: https://github.com/YOUR_USERNAME
- LinkedIn: https://linkedin.com/in/YOUR_PROFILE

---

# 📌 Internship

This project was completed as part of the **Oasis Infobyte Data Science Internship Program**.

⭐ If you found this project useful, consider giving the repository a star.