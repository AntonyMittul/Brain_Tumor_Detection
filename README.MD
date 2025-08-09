# BRAIN TUMOR DETECTION

## 🧠 Brain Tumor Detection using CNN

This project implements a **deep learning model** for automated classification of **brain MRI images** into four categories:

* **Glioma Tumor**
* **Meningioma Tumor**
* **No Tumor**
* **Pituitary Tumor**

It leverages **Convolutional Neural Networks (CNNs)** to analyze MRI scans and detect tumors with high accuracy, helping in early diagnosis and reducing manual workload for radiologists.

---

### 📌 Key Features

* **Multi-Class Classification** – Identifies the exact tumor type from MRI scans.
* **Data Augmentation** – Improves generalization using rotation, shifting, zooming, and flipping.
* **Custom CNN Architecture** – Built from scratch with convolution, pooling, dropout, and dense layers.
* **Performance Evaluation** – Accuracy, loss plots, confusion matrix, and classification report.
* **Visualization** – Displays tumor distribution and sample MRI images for each class.

---

### 🗂 Dataset

* **Source**: Brain MRI dataset stored in Google Drive (Kaggle origin).
* **Categories**: `glioma`, `meningioma`, `notumor`, `pituitary`.
* **Image Preprocessing**:

  * Resized to **150×150 pixels**.
  * Normalized pixel values to \[0,1].
  * Applied **ImageDataGenerator** augmentations:

    * Rotation: 20°
    * Width/Height Shift: 10%
    * Shear: 10%
    * Zoom: 10%

---

### ⚙️ Technologies Used

* **Python** – Programming language.
* **TensorFlow/Keras** – Model development and training.
* **Matplotlib & Seaborn** – Visualization.
* **Pandas & NumPy** – Data handling.
* **OpenCV** – Image preprocessing.

---

### 📊 Model Architecture

1. **Conv2D** + **MaxPooling2D** layers for feature extraction.
2. **Flatten** layer to convert feature maps into vectors.
3. **Dense** layers for classification, with **Dropout** for regularization.
4. **Softmax** activation for multi-class output.

---

### 🚀 Training & Results

* **Epochs**: 50
* **Batch Size**: 32
* **Optimizer**: Adam
* **Loss Function**: Categorical Crossentropy
* Achieved **high classification accuracy** across training and validation sets.
* Stable learning curve without major overfitting.

---

### 📌 Future Enhancements

* Implement **Transfer Learning** with pre-trained models (VGG16, ResNet50) for better accuracy.
* Add **Grad-CAM visualization** to explain model predictions.
* Deploy as a **web app** for real-time MRI classification.

---
