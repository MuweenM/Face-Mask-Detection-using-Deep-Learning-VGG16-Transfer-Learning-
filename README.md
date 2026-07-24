# 😷 Face Mask Detection using Deep Learning (VGG16 Transfer Learning)

A Deep Learning-based Face Mask Detection system built using **TensorFlow/Keras**, **OpenCV**, and **VGG16 Transfer Learning**. The model classifies whether a person is **wearing a face mask** or **not wearing a face mask** from an input image.

---

## 📌 Project Overview

This project uses a pre-trained **VGG16 Convolutional Neural Network (CNN)** as the feature extractor and applies Transfer Learning to perform binary image classification.

The dataset contains two classes:

- 😷 With Mask
- 🙂 Without Mask

The model is trained on resized face images (224 × 224 pixels) and can later be used for real-time face mask detection with a webcam.

---

## 🚀 Features

- Image preprocessing using OpenCV
- Data normalization
- Transfer Learning with VGG16
- Binary classification
- Training & validation split
- Model evaluation
- Save trained model
- Predict mask / no-mask images
- Easily extendable to real-time webcam detection

---

## 🛠 Technologies Used

- Python 3.x
- TensorFlow / Keras
- OpenCV
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## 📂 Project Structure

```
Face-Mask-Detection/
│
├── train/
│   ├── with_mask/
│   └── without_mask/
│
│
├── face_mask_detector_session.ipynb
├── mask_detector.keras
├── README.md
└── requirements.txt
```

---

## 📊 Dataset

The dataset consists of two categories:

| Class | Label |
|--------|-------|
| With Mask | 0 |
| Without Mask | 1 |



## 🧠 Model Architecture

The project uses **Transfer Learning** with **VGG16**.

Architecture:

```
Input Image
      │
      ▼
Pre-trained VGG16
      │
Feature Extraction
      │
Global Average Pooling
      │
Dense Layer
      │
Dropout
      │
Output Layer (2 Classes)
```

---

## ⚙️ Data Preprocessing

The preprocessing pipeline includes:

- Loading images
- Image resizing (224 × 224)
- Label encoding
- Dataset shuffling
- NumPy array conversion
- Pixel normalization
- Train/Test split

---

## 📈 Training

The model is trained using:

- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Metrics: Accuracy

Training includes:

- Validation dataset
- Transfer Learning

---

## 📊 Evaluation Metrics

After training, the model can be evaluated using:

- Training Accuracy
- Validation Accuracy
- Test Accuracy
- Loss
- Confusion Matrix
- Classification Report

---

## 📦 Installation

Clone the repository

```bash
git clone https://github.com/your-username/Face-Mask-Detection.git
```

Navigate into the project

```bash
cd Face-Mask-Detection
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Notebook

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open

```
face_mask_detector_session.ipynb
```

Run all cells.

---

## 📸 Prediction

After training, load the saved model and predict:

```python
prediction = model.predict(image)
```

Output:

```
With Mask
```

or

```
Without Mask
```

---

## 📚 Future Improvements

- Real-time webcam detection
- Face detection using Haar Cascade or DNN
- Mobile deployment using TensorFlow Lite
- Improve accuracy with data augmentation
- Deploy as a Flask/Django web application
- Deploy using Streamlit

---

## 📈 Results

The model successfully learns to classify face images into:

✅ With Mask

✅ Without Mask

using Transfer Learning with VGG16.

---

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository
2. Create a feature branch

```bash
git checkout -b feature-name
```

3. Commit your changes

```bash
git commit -m "Added new feature"
```

4. Push to GitHub

```bash
git push origin feature-name
```

5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License.


---
⭐ If you found this project helpful, consider giving it a star on GitHub!
