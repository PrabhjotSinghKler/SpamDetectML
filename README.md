
# Email Spam Detection with Naive Bayes Classifier  

This project implements an **email spam detection system** using a **Naive Bayes classifier**. It leverages machine learning techniques to classify emails as either "spam" or "ham" (non-spam), aiming to enhance email filtering systems for improved reliability and security.

---

## 📖 Table of Contents  

1. [Introduction](#introduction)  
2. [Problem Statement](#problem-statement)  
3. [Dataset](#dataset)  
4. [Methodology](#methodology)  
5. [Results](#results)  
6. [Technologies Used](#technologies-used)  
7. [How to Use](#how-to-use)  
8. [Acknowledgements](#acknowledgements)  

---

## 🔍 Introduction  

Email spam is a persistent issue, disrupting user experiences and burdening email systems. This project addresses the inefficiencies of traditional spam filters by employing a machine learning-based approach to accurately detect and filter spam emails.  

---

## ❓ Problem Statement  

Traditional spam detection systems struggle to adapt to evolving spam patterns, leading to:  
- False positives: Legitimate emails marked as spam.  
- False negatives: Spam emails bypassing the filter.  

This project focuses on developing a robust model that minimizes false negatives, ensuring harmful content is effectively blocked.  

---

## 📊 Dataset  

The dataset used contains:  
- **5572 emails**  
  - 86.6% categorized as "ham."  
  - 13.4% categorized as "spam."  
- After preprocessing:  
  - Duplicate rows: 415 removed.  
  - Missing values: None detected.  
- Features extracted using **Bag-of-Words**.  

---

## ⚙️ Methodology  

### 1. Data Preprocessing  
- Removed duplicates and missing values.  
- Transformed categorical labels ("ham" → 0, "spam" → 1).  

### 2. Model Training  
- Split dataset: 75% training, 25% testing.  
- Model: **Naive Bayes classifier** with **CountVectorizer** for feature extraction.  

### 3. Evaluation Metrics  
- **Accuracy**  
- **Precision, Recall, F1-score**  
- **ROC-AUC Curve**  

---

## 📈 Results  

- **Accuracy**: 98.85% on the test set.  
- **Recall**: 93.5% for spam detection, prioritizing the reduction of missed spam.  
- **Train ROC-AUC**: 98.33%  
- **Test ROC-AUC**: 96.61%  

These results validate the model's robustness and suitability for real-world email filtering systems.  

---

## 🛠️ Technologies Used  

- **Languages**: Python  
- **Libraries**:  
  - Data Manipulation: `pandas`, `numpy`  
  - Visualization: `matplotlib`, `seaborn`, `wordcloud`  
  - Machine Learning: `scikit-learn`  

---

## 🖥️ How to Use  

1. **Clone the Repository**  
   ```bash  
   git clone https://github.com/yourusername/SpamDetectML.git  
   cd SpamDetectML  
   ```  

2. **Install Dependencies**  
   Ensure you have Python and pip installed. Then, run:  
   ```bash  
   pip install -r requirements.txt  
   ```  

3. **Run the Project**  
   - Place your dataset (`Mail Data.csv`) in the project directory.  
   - Execute the Python script:  
     ```bash  
     python spam_detection.py  
     ```  

4. **Results**  
   The script will display evaluation metrics, plots, and classification results.  

---

## 🙏 Acknowledgements  

This project was built as part of a learning initiative to explore machine learning in cybersecurity applications.

### References  
1. Dataset: [SMS Spam Collection Dataset](https://www.kaggle.com/datasets/bhaskarreddy072/mail-datacsv)  
2. Libraries:  
   - [Scikit-learn](https://scikit-learn.org/)  
   - [Pandas](https://pandas.pydata.org/)  
   - [Matplotlib](https://matplotlib.org/)  
   - [Seaborn](https://seaborn.pydata.org/)  
   - [WordCloud](https://github.com/amueller/word_cloud)  
