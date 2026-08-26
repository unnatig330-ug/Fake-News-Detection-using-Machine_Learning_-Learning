# 📰 Fake News Detection using Machine Learning

## 📌 Introduction

Fake news is false or misleading information presented as news. With the rapid growth of online news and social media, identifying whether a news article is real or fake has become an important challenge.

This project uses **Machine Learning and Natural Language Processing (NLP)** techniques to classify news articles as **Fake News** or **Real News**.

The project uses **TF-IDF (Term Frequency–Inverse Document Frequency)** for converting text into numerical features and compares two Machine Learning models:

* Logistic Regression
* Random Forest Classifier

The performance of the models is evaluated using Accuracy, Precision, Recall, F1-Score, and Confusion Matrix Heatmaps.

---

## 🎯 Project Objective

The main objectives of this project are:

* To detect whether a news article is Fake or Real.
* To preprocess and transform textual news data into numerical features.
* To use TF-IDF for feature extraction.
* To implement Logistic Regression and Random Forest models.
* To compare the performance of both models.
* To evaluate the models using Accuracy, Precision, Recall, and F1-Score.
* To visualize model performance using Confusion Matrix Heatmaps.
* To predict whether a new user-provided news article is Fake or Real.

---

## 📊 Dataset Description

The project uses a dataset containing **44,898 news articles** with the following columns:

| Column    | Description                                  |
| --------- | -------------------------------------------- |
| `title`   | Title of the news article                    |
| `text`    | Main text/content of the article             |
| `subject` | Category or subject of the news              |
| `date`    | Publication date                             |
| `label`   | Target variable indicating Fake or Real news |

### Label Encoding

* `1` → Fake News
* `0` → Real News

The Fake and Real news datasets are combined, labelled, and shuffled before training the Machine Learning models.

---

## 🛠️ Technology Stack

### Programming Language

* Python

### Development Environment

* Google Colab
* Jupyter Notebook

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

### Machine Learning / NLP Techniques

* TF-IDF Vectorization
* Logistic Regression
* Random Forest Classifier
* Confusion Matrix
* Classification Metrics

---

## 🔄 Project Methodology

The project follows these major steps:

1. Import required Python libraries.
2. Load Fake and Real news datasets.
3. Explore the datasets.
4. Assign labels to Fake and Real news.
5. Combine and shuffle the datasets.
6. Analyze the dataset using Exploratory Data Analysis (EDA).
7. Select the required text and target columns.
8. Split the data into training and testing sets.
9. Convert text into numerical features using TF-IDF.
10. Train Logistic Regression and Random Forest models.
11. Evaluate both models.
12. Generate Confusion Matrix Heatmaps.
13. Compare model performance.
14. Use the best-performing model to classify new news articles.

---

## 🤖 Machine Learning Models

### 1. Logistic Regression

Logistic Regression is a classification algorithm used to predict whether a news article belongs to the Fake or Real category.

It works effectively with high-dimensional text features generated using TF-IDF.

### 2. Random Forest Classifier

Random Forest is an ensemble Machine Learning algorithm that combines multiple decision trees to make predictions.

It is used in this project to capture different patterns in the textual features and classify news articles.

---

## 📈 Model Performance

The models were evaluated using Accuracy, Precision, Recall, and F1-Score.

| Model               |   Accuracy |  Precision |     Recall |   F1-Score |
| ------------------- | ---------: | ---------: | ---------: | ---------: |
| Logistic Regression |     98.27% |     98.65% |     98.05% |     98.35% |
| Random Forest       | **98.90%** | **99.25%** | **98.64%** | **98.95%** |

### 🏆 Best Model

The **Random Forest Classifier** achieved the best overall performance with approximately **98.90% accuracy**.

Therefore, Random Forest is selected as the preferred model for predicting new news articles in this project.

---

## 📊 Model Evaluation

The following evaluation techniques are used:

### Accuracy

Measures the percentage of correctly classified news articles.

### Precision

Measures how many articles predicted as a particular class were actually from that class.

### Recall

Measures how many actual articles of a class were correctly identified.

### F1-Score

Provides a balance between Precision and Recall.

### Confusion Matrix

Confusion Matrix Heatmaps are generated for both Logistic Regression and Random Forest to visualize correct and incorrect predictions.

---

## 📉 Visualizations

The project includes:

* Fake vs Real News Distribution
* Confusion Matrix Heatmap for Logistic Regression
* Confusion Matrix Heatmap for Random Forest
* Model Performance Comparison
* Accuracy, Precision, Recall and F1-Score comparison

These visualizations help in understanding the behaviour and performance of the Machine Learning models.

---

## 🧪 New News Prediction

The project also allows the user to enter a new news article.

The text is transformed using the already trained TF-IDF vectorizer and passed to the Random Forest model for prediction.

The system provides the output as:

* **FAKE NEWS**
* **REAL NEWS**

This demonstrates how the trained model can be used to classify previously unseen news text.

> **Note:** This system is a Machine Learning-based classifier. It does not verify news against external fact-checking sources.

---

## ✅ Advantages

* High classification accuracy.
* Uses two different Machine Learning models.
* Uses TF-IDF for effective text feature extraction.
* Provides multiple evaluation metrics.
* Includes Confusion Matrix Heatmaps.
* Allows prediction of new news articles.
* Simple and easy-to-understand implementation.
* Can be further improved with advanced NLP techniques.

---

## ⚠️ Project Limitations

* The model depends heavily on the quality and diversity of the training dataset.
* It mainly analyzes the textual content of news articles.
* New styles of misinformation may not be detected correctly.
* Performance may decrease when the model encounters news from completely different sources or topics.
* The model does not verify claims using external fact-checking databases.
* A high accuracy score does not guarantee that every prediction is correct.

---

## 🚀 Future Scope

The project can be improved in the future by:

* Using advanced NLP techniques.
* Applying Deep Learning models such as LSTM or Transformers.
* Using models such as BERT for contextual understanding.
* Including additional news sources and larger datasets.
* Adding real-time news verification.
* Integrating external fact-checking APIs.
* Developing a web application for easier user interaction.

---

## ▶️ How to Run the Project

### Step 1: Open the Notebook

Open the project notebook in **Google Colab** or Jupyter Notebook.

### Step 2: Upload the Dataset

Upload the required:

* `Fake.csv`
* `True.csv`

files.

### Step 3: Run the Notebook

Run the cells sequentially from beginning to end.

### Step 4: Enter New News

At the prediction section, enter a news article when prompted.

The trained model will classify it as:

**Fake News** or **Real News**.

---

## 📁 Project Structure

```text
Project-Fake-News-Detection-using-Machine-Learning/
│
├── README.md
│
└── Fake_News_Detection_using_Machine_Learning.ipynb
```

---

## 📚 References

* Scikit-learn documentation for Machine Learning algorithms and evaluation metrics.
* Pandas documentation for data manipulation and analysis.
* Matplotlib documentation for data visualization.
* Seaborn documentation for statistical visualization.
* Dataset used for training and evaluation of the Fake News Detection model.

---

## 🏁 Conclusion

This project demonstrates how Machine Learning can be used to classify news articles as Fake or Real.

Two Machine Learning models, **Logistic Regression** and **Random Forest**, were implemented and compared using multiple evaluation metrics.

The **Random Forest Classifier achieved the best performance with approximately 98.90% accuracy**, making it the preferred model for new-news prediction in this project.

Although the model provides strong performance on the available dataset, it should not be considered a complete fact-checking system. The project can be further improved using advanced NLP, Deep Learning, Transformer models, and real-time fact-checking techniques.

---

## 👩‍💻 Author

**Unnati**

### Project

**Fake News Detection using Machine Learning**

Built using **Python, NLP, TF-IDF, Logistic Regression, and Random Forest**.
