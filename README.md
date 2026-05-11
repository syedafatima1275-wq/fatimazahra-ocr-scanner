## project 2 

## Project Overview: Intelligent Document Processing (IDP) System


This project is an AI-powered **Intelligent Document Processing (IDP) System** developed using **Python, OCR, Machine Learning, and FastAPI**. The system automatically analyzes uploaded document images, identifies their type, and extracts important information such as dates and amounts.

### Main Goal

The objective of the project was to automate document handling by:

* Reading scanned document images
* Extracting text using OCR
* Classifying documents into categories
* Extracting useful information
* Providing results through a REST API



## Technologies Used

* **Python**
* **FastAPI** – REST API framework
* **Tesseract OCR (pytesseract)** – Text extraction from images
* **Scikit-learn** – Machine learning model training
* **TF-IDF Vectorization** – Text feature extraction
* **Logistic Regression** – Document classification
* **Joblib** – Saving trained models



## Document Categories

The system was trained to classify:

1. **Invoices**
2. **Receipts**
3. **Contracts**



## Project Workflow

### 1. Data Collection

Datasets were collected from Kaggle and organized into separate folders for each document category.

### 2. OCR Text Extraction

Using Tesseract OCR, text was extracted from scanned images.

### 3. Feature Engineering

TF-IDF Vectorizer converted extracted text into numerical features for machine learning.

### 4. Model Training

A Logistic Regression classifier was trained on **127 documents**.

### 5. Model Saving

The trained files were saved as:

* `vectorizer.pkl`
* `classifier.pkl`

### 6. REST API Development

A FastAPI application was created with:

* `GET /` → Health check endpoint
* `POST /classify` → Upload and classify documents

### 7. Information Extraction

Regex patterns were used to extract:

* Dates
* Currency amounts
* Total values


## Final Outcome

The project successfully demonstrated how OCR and Machine Learning can automate document processing tasks. The deployed FastAPI service can be integrated into real-world systems for:

* Automated bookkeeping
* Receipt management
* Invoice processing
* Legal document organization
* Enterprise document automation



## Conclusion

This IDP system provides a complete pipeline from document upload to intelligent classification and data extraction. It shows the practical use of AI and OCR in reducing manual paperwork and improving business automation.






