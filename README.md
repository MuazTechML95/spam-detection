# Spam Detection Project

## Overview
This project is a **Spam Detection system** using Python.  
It uses **TF-IDF vectorization** and **Logistic Regression** to classify messages as **Spam** or **Ham** (normal message).  

The project is implemented in a **Jupyter Notebook** (`.ipynb`) and can be run in **Google Colab** or locally.

---

## Features
- Custom text preprocessing using regex
- TF-IDF vectorization of text messages
- Logistic Regression model for classification
- Evaluation with **Precision**, **Recall**, and **F1-score**
- Save and reuse the trained model using **joblib**
- Interactive user input to classify new messages

---

## Dataset
- The dataset file is `spam.csv`.  
- It contains two columns:
  - `label` → `spam` or `ham`
  - `text` → Message content

> **Note:** Make sure the dataset file is in the same folder as the notebook if running locally.

---

## How to Run
1. Open the notebook `spam_detection.ipynb` in **Google Colab** or **Jupyter Notebook**.
2. Run all cells sequentially.
3. The model will train on the dataset and save a pipeline (`spam_detection_pipeline.pkl`).
4. To test your own messages:
    - Type the message in the input cell.
    - Type `stop` to exit the input loop.

Example:
```python
Enter your message: Free iPhone! Click here to claim
Result: 📩 Spam

Enter your message: Are we meeting tomorrow?
Result: 📨 Ham
