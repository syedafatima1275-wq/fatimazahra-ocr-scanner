# 📄 OCR Document Scanner (Tesseract + EasyOCR)

👩‍💻 **Author:** Syeda Fatima Zahra
🎓 **Degree:** BS Electronics
🏫 **University:** Quaid-i-Azam University, Islamabad

---

## 📌 Project Overview

This project demonstrates **Optical Character Recognition (OCR)** using:

* Tesseract OCR
* EasyOCR

The system extracts text from receipt images and improves accuracy using **OpenCV preprocessing techniques**.

---

## 🚀 Features

* 📷 Text extraction from images
* 🔍 Tesseract OCR implementation
* 🤖 EasyOCR implementation
* 🧹 Image preprocessing (grayscale, blur, thresholding)
* 📊 Comparison of OCR results before and after preprocessing
* 🧾 Synthetic receipt generation (no dataset required)

---

## 🛠️ Technologies Used

* Python
* OpenCV
* Tesseract OCR
* EasyOCR
* PIL (Python Imaging Library)
* Matplotlib

---

## 📂 Project Structure

```
├── notebook.ipynb
├── receipt.png
├── README.md
```

---

## ▶️ How to Run (Kaggle)

1. Open Kaggle Notebook
2. Install EasyOCR:

   ```bash
   !pip install easyocr
   ```
3. Run all cells step by step
4. The system will:

   * Generate a sample receipt
   * Extract text using OCR
   * Improve accuracy using preprocessing

---

## 📈 Results

* Successfully extracted text from generated receipt
* Improved OCR accuracy after preprocessing
* Compared Tesseract and EasyOCR outputs

---

## 💡 Future Improvements

* Add real dataset support
* Extract structured fields (Date, Total, Items)
* Build GUI for document scanning

---

## ⭐ Conclusion

This project builds a strong foundation for **Document Intelligence systems** and demonstrates practical OCR implementation without requiring external datasets.

---

## 📬 Contact

**Syeda Fatima Zahra**
Quaid-i-Azam University, Islamabad


## week 6 : Advanced OCR System using Image Preprocessing and CNN


#  OBJECTIVES

• Skewed aur tilted documents ko correct karna
• Noisy images ko clean karna
• Perspective distortion fix karna
• Image quality improve karna for OCR
• CNN model build karna from scratch
• MNIST dataset par high accuracy achieve karna


#  METHODOLOGY / WORKFLOW

##  Step 1: Image Preprocessing

Is phase mein hum ne image ko OCR-ready banaya:

###  Perspective Correction

Image ko straight kiya using transformation

###  Deskewing

Tilted image ko seedha kiya

###  Morphological Operations

• Erosion → noise remove
• Dilation → gaps fill
• Opening → small noise remove
• Closing → holes fill

##  Step 2: CNN Model Development

###  Dataset

MNIST (handwritten digits dataset)

### Preprocessing

• Reshape (28×28×1)
• Normalize (0–1)
• One-hot encoding

###  Model Architecture

• Conv2D layers (feature extraction)
• MaxPooling (dimension reduce)
• Dense layers (classification)
• Dropout (overfitting control)


##  Step 3: Training & Evaluation

• Optimizer: Adam
• Loss: Categorical Crossentropy
• Epochs: 10
• Batch size: 128



#  RESULTS

• Image preprocessing se OCR quality improve hui
• CNN model ne handwritten digits accurately recognize kiye
• High accuracy (~98%) achieved
• Model robust hai real-world inputs ke liye


#  KEY LEARNINGS

• Image preprocessing OCR ke liye **bohat critical hai**
• CNNs automatically features learn karte hain
• Data normalization aur architecture design important hai
• Real-world images perfect nahi hoti — preprocessing zaroori hai



