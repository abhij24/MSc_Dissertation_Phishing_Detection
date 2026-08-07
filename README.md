# AI-Based Phishing Email Detection using Machine Learning and Transformer Models

## Project Overview

This project investigates phishing email detection using traditional machine learning and transformer-based deep learning models. The system applies Natural Language Processing (NLP), feature engineering, TF-IDF vectorization, deep learning, and transformer architectures to accurately classify phishing and legitimate emails.

## Models Used

- Logistic Regression
- Random Forest
- Linear SVM
- Multinomial Naive Bayes
- XGBoost
- Bidirectional LSTM (BiLSTM)
- DistilBERT

---

## Implementation

The project is implemented using a modular notebook-based workflow, where each notebook performs a specific stage of the phishing email detection pipeline.

### Notebook 1 – Data Understanding and Feature Engineering

- Load and explore the phishing email dataset.
- Perform data cleaning and preprocessing using NLP techniques.
- Generate handcrafted features such as:
  - Email Length
  - Word Count
  - URL Count
  - Uppercase Ratio
  - Special Character Count
  - Phishing Keyword Count
  - Credential Keyword Count
  - Finance Keyword Count
  - Vocabulary Richness
- Apply TF-IDF vectorization for traditional machine learning models.
- Save the processed dataset for subsequent notebooks.

### Notebook 2 – Traditional Machine Learning Models

Implemented and evaluated:

- Logistic Regression
- Random Forest
- Linear SVM
- Multinomial Naive Bayes
- XGBoost

For each model:

- Train using TF-IDF features.
- Generate predictions on the test dataset.
- Evaluate using:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - ROC-AUC
- Generate Confusion Matrix and ROC Curve.
- Perform Cross Validation (where applicable).
- Save trained models using Joblib.

### Notebook 3 – Bidirectional LSTM

- Tokenize and pad email text.
- Build a Bidirectional LSTM neural network using TensorFlow/Keras.
- Train using preprocessed text.
- Evaluate using Accuracy, Precision, Recall, F1-score, Confusion Matrix and ROC-AUC.

### Notebook 4 – DistilBERT

- Fine-tune the DistilBERT transformer using the Hugging Face Transformers library.
- Tokenize emails using the DistilBERT tokenizer.
- Train using the Hugging Face Trainer API.
- Generate predictions and evaluate using Accuracy, Precision, Recall, F1-score and ROC-AUC.

### Notebook 5 – Model Comparison and Analysis

Compare the performance of all seven models:

- Logistic Regression
- Random Forest
- Linear SVM
- Multinomial Naive Bayes
- XGBoost
- Bidirectional LSTM
- DistilBERT

Generate:

- Performance comparison table
- Accuracy comparison chart
- Precision, Recall and F1-score comparison
- ROC-AUC comparison
- Training time comparison
- Final CSV report containing model performance metrics

---

## Pretrained Model Weights

Due to GitHub file size limits, the trained model checkpoints and weights are hosted on Google Drive.

**Download Project Source Code (.zip)**

https://drive.google.com/file/d/1IY-xaBQynRryjkZ7c6Z8R1cHAqCudgt9/view?usp=drive_link

---

## Project Structure

```
data/
│
├── raw/
├── processed/
│
models/
│
notebooks/
│   ├── 01_Data_Understanding_and_Feature_Engineering.ipynb
│   ├── 02_Advanced_Models.ipynb
│   ├── 03_LSTM_Model.ipynb
│   ├── 04_BERT_Model.ipynb
│   └── 05_Model_Comparison_and_Analysis.ipynb
│
results/
│
requirements.txt
README.md
```

---

## Requirements

- Python 3.11+

Install all required dependencies:

```bash
pip install -r requirements.txt
```

---

## Run Order

1. 01_Data_Understanding_and_Feature_Engineering.ipynb
2. 02_Advanced_Models.ipynb
3. 03_LSTM_Model.ipynb
4. 04_BERT_Model.ipynb
5. 05_Model_Comparison_and_Analysis.ipynb

Run the notebooks sequentially to reproduce the experimental results.

---

## Author

**Abhishek Prasad Jagtap**

MSc Data Analytics

National College of Ireland
