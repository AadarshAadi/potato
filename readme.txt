# 🥔 Potato Disease Classifier (PotatoDie)

> An end-to-end deep learning application that detects potato leaf diseases using Convolutional Neural Networks (CNNs).

The model classifies potato leaves into three categories:

- 🌱 Healthy
- 🍂 Early Blight
- 🍁 Late Blight

---

## 📖 Overview

Plant diseases can significantly reduce agricultural productivity and crop yield. This project provides an automated disease detection system that helps farmers, researchers, and agricultural professionals identify potato diseases quickly and accurately from leaf images.

The model is trained on the **PlantVillage Dataset** and deployed as a web application for real-time predictions.

---

## ✨ Features

- 🔍 Real-time potato leaf disease detection
- 🤖 CNN-based deep learning model
- ⚡ FastAPI backend for inference
- 🌐 Web-based interface for image uploads
- 📈 High prediction accuracy
- 🚀 End-to-end pipeline from training to deployment

---

## 🛠️ Tech Stack

| Category | Technologies |
|-----------|-------------|
| Language | Python |
| Deep Learning | TensorFlow, Keras |
| Data Processing | NumPy, Pandas |
| Visualization | Matplotlib |
| Backend | FastAPI |
| Frontend Hosting | Vercel |
| Dataset | PlantVillage |

---

## 📊 Dataset

### Source
PlantVillage Dataset (Kaggle)

### Distribution

| Class | Images |
|---------|---------:|
| Early Blight | 1000 |
| Late Blight | 1000 |
| Healthy | 152 |
| **Total** | **2152** |

### Data Split

| Split | Percentage |
|---------|----------:|
| Training | 80% |
| Validation | 10% |
| Testing | 10% |

---

## 🔄 Data Preprocessing

The following preprocessing techniques were applied:

### Image Processing
- Image resizing
- Pixel normalization

### Data Augmentation
- Horizontal Flip
- Random Rotation (`0.1`)
- Random Zoom (`0.1`)

These techniques improve model generalization and reduce overfitting.

---

## 🧠 Model Architecture

The classifier is built using a **Convolutional Neural Network (CNN)** consisting of:

- Conv2D Layers + ReLU Activation
- MaxPooling Layers
- Dropout Layers
- Fully Connected Dense Layers
- Softmax Output Layer

### Workflow

```text
Input Image
      ↓
Convolution Layers
      ↓
Max Pooling
      ↓
Dropout
      ↓
Dense Layers
      ↓
Prediction
```

---

## 📈 Model Performance

| Metric | Score |
|---------|-------:|
| Accuracy | 98.99% |
| Loss | 0.0176 |

The model achieves excellent classification performance with very low prediction error.

---

## 🌐 Live Demo

Try the deployed application:

🔗 **https://potatodieleafs.vercel.app/**

---

## 📷 How It Works

1. Upload a potato leaf image.
2. The model processes the image.
3. Disease class is predicted instantly.
4. Results are displayed to the user.

### Supported Classes

- 🌱 Healthy
- 🍂 Early Blight
- 🍁 Late Blight

---

## 🚀 Run Locally

### 1. Clone the Repository

```bash
git clone https://github.com/anurag23o2/PotatoDie.git
```

### 2. Navigate to the Project

```bash
cd PotatoDie
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Start the FastAPI Server

```bash
uvicorn main:app --reload
```

### 5. Open in Browser

```text
http://localhost:8000
```

---

## 📂 Project Structure

```text
PotatoDie/
│
├── dataset/
├── models/
├── notebooks/
├── api/
├── frontend/
├── main.py
├── requirements.txt
└── README.md
```

---

## ⚠️ Limitations

- Supports only potato leaf images
- Performance may vary with image quality
- Dataset diversity is limited
- Real-world field conditions may affect predictions

---

## 🔮 Future Improvements

- 🌾 Support additional crop diseases
- 📈 Expand dataset size and diversity
- 📱 Mobile application development
- 📷 Real-time field detection
- 🌍 IoT-based agricultural monitoring
- ☁️ Cloud-based prediction services

---

## 👨‍💻 Author

Developed as a deep learning project for automated potato disease detection.

If you found this project useful, consider giving it a ⭐ on GitHub.
