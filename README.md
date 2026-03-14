# Fake News Detector System

## 📌 Project Overview

This project is a Fake News Detection Web Application** that analyzes a news article and predicts whether it is Fake,Suspicious**, or **Likely Real**.
The system works using a rule-based Natural Language Processing (NLP) approach where the user provides suspicious keywords, and the program checks if those keywords appear in the news text.

The application also performs sentiment analysis to examine the emotional tone of the article. Based on the number of suspicious keywords detected and the sentiment score, the system classifies the news.

This project demonstrates basic concepts of:

* Natural Language Processing (NLP)
* Sentiment Analysis
* Rule-based text classification
* Simple web interface using Python

---

## 🚀 Features

* User can enter any news headline or article
* User can define suspicious keywords
* Detects whether the news is:

  * 🚨 Fake News
  * ⚠ Suspicious News
  * ✅ Likely Real News
* Displays:

  * Detected keywords
  * Keyword score
  * Sentiment score
* Simple web interface

---

## 🛠 Technologies Used

* Python
* Gradio – for creating the web interface
* TextBlob – for sentiment analysis
* HTML & CSS styling (inside the interface)
* Google Colab– for running the project

---

## ⚙️ How the System Works

### 1. User Input

The user provides:

* A news article or headline
* A list of suspicious keywords (comma separated)

Example:

```
News: Secret government cure for cancer exposed
Keywords: secret, miracle, shocking, cure
```

---

### 2. Text Preprocessing

The system converts the news text to lowercase to ensure accurate keyword matching.

Example:

```
Secret Government Cure → secret government cure
```

---

### 3. Keyword Detection

The program searches the news text for suspicious keywords.

Example:

 Keyword  | Found 
 secret       ✔     
 miracle      ✘    
 shocking     ✘     
 cure         ✔ 

Keyword Score = 2

---

### 4. Sentiment Analysis

The project uses **TextBlob** to determine the sentiment polarity of the text.

Sentiment values range from:

 Score | Meaning       
  
 -1   -  Very negative 
  0   -   Neutral       
 +1   -  Very positive 

Fake news often contains emotionally exaggerated language
---

## 📊 Example Output

```
Result: Suspicious News
Keywords Found: ['secret','cure']
Keyword Score: 2
Sentiment Score: 0.1
```

---


## 📂 Project Structure

```
Fake-News-Detector
│
├── fake_news_detector.ipynb
├── README.md
└── requirements.txt
```

---

## ⚠ Limitations

* Uses a rule-based approach
* Accuracy depends on keywords provided by the user
* Does not use machine learning models
* Cannot fully understand context of the news article

---

## 🔮 Future Improvements

Possible improvements include:

1. **Machine Learning Models**

   * Logistic Regression
   * Naive Bayes
   * Support Vector Machine

2. **Advanced NLP**

   * TF-IDF feature extraction
   * Word embeddings

3. **Deep Learning**

   * LSTM networks
   * Transformer models like BERT

4. **Source Credibility Checking**

   * Detect unreliable news sources

5. **Social Media Integration**

   * Detect misinformation from platforms such as Twitter and Facebook

---

## 🎯 Learning Outcomes

Through this project, the following concepts were explored:

* Text processing in Python
* Sentiment analysis using NLP
* Rule-based classification
* Building simple AI applications
* Deploying interactive interfaces

---

## 📌 Conclusion

This project provides a basic prototype for detecting fake news using simple NLP techniques. While it is not as powerful as machine learning models, it demonstrates how text analysis and keyword detection can help identify suspicious news articles.

---

⭐ If you like this project, feel free to **fork the repository and contribute improvements.**
