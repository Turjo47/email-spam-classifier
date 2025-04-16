# 📧 Spam Mail Detection using Machine Learning

This project demonstrates a simple yet effective machine learning model to detect spam emails or messages. It utilizes natural language processing (NLP) techniques and a Logistic Regression classifier to classify messages as either **"spam"** or **"ham"** (not spam).

---

## 🔍 Overview

- **Dataset:** SMS Spam Collection Dataset (5,572 labeled messages)
- **Model Used:** Logistic Regression
- **Text Vectorization:** TF-IDF (Term Frequency - Inverse Document Frequency)
- **Accuracy:** ~96.7% on both training and testing sets

---

## 🚀 How It Works

1. **Data Loading & Preprocessing:**
   - Missing values handled
   - Labels (`spam` → 0, `ham` → 1) encoded

2. **Text Vectorization:**
   - Applied `TfidfVectorizer` to convert text into numerical features

3. **Model Training:**
   - Split data into training and test sets (80/20)
   - Trained using Logistic Regression

4. **Evaluation:**
   - Achieved ~96.7% accuracy on both training and testing sets

5. **Prediction Example:**
   - Classifies new messages with the trained model

---

## 🧪 Example Prediction

```python
input_your_mail = ["This email contain a $5000 job. Just click the link below"]
prediction = model.predict(feature_extraction.transform(input_your_mail))

if prediction[0] == 1:
    print("Ham mail")
else:
    print("Spam mail")
```

---

## Dataset
[UCI SMS Spam Collection](https://archive.ics.uci.edu/dataset/228/sms+spam+collection)

---

## requirements 

Install required package using:
```bash
    pip install numpy pandas scikit-learn
```



