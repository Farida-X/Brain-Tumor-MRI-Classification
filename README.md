# 🧠 Brain Tumor MRI Classification using Deep Learning

## 📌 Overview

This project presents a comprehensive deep learning approach for **Brain Tumor MRI Classification** using TensorFlow and Keras. Two neural network architectures were developed, trained, and evaluated to classify brain MRI images into four categories:

* Glioma
* Meningioma
* Pituitary Tumor
* No Tumor

The objective is to compare the performance of a **Feedforward Neural Network (FFNN)** and a **Convolutional Neural Network (CNN)** in terms of classification accuracy, generalization ability, computational efficiency, and robustness.

---

## 📂 Dataset

The dataset used in this project is publicly available on Kaggle and is not included in this repository due to GitHub storage limitations.

📥 **Dataset:**
https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset

### Dataset Structure

```text
Training/
├── Glioma
├── Meningioma
├── Pituitary
└── No Tumor

Testing/
├── Glioma
├── Meningioma
├── Pituitary
└── No Tumor
```

During preprocessing, the training dataset is automatically split into:

* **80% Training**
* **20% Validation**

All images are resized to **128 × 128** pixels before training.

---

## 🚀 Project Highlights

* MRI image preprocessing and normalization
* Dataset exploration and visualization
* Class distribution analysis
* Duplicate filename verification
* TensorFlow data pipeline optimization
* Feedforward Neural Network (FFNN)
* Convolutional Neural Network (CNN)
* Early Stopping for overfitting prevention
* Dropout regularization
* Performance evaluation using multiple metrics
* Model comparison and benchmarking
* Hyperparameter optimization experiments

---

## 🛠️ Technologies & Libraries

* Python
* TensorFlow & Keras
* NumPy
* Pandas
* Matplotlib
* Scikit-learn

---

## 🧠 Model Architectures

### Feedforward Neural Network (FFNN)

* Flatten Layer
* Dense (512, ReLU)
* Dropout (0.3)
* Dense (256, ReLU)
* Dropout (0.3)
* Softmax Output Layer

### Convolutional Neural Network (CNN)

* Conv2D (32 Filters)
* MaxPooling2D
* Conv2D (64 Filters)
* MaxPooling2D
* Conv2D (128 Filters)
* MaxPooling2D
* Flatten Layer
* Dense (128, ReLU)
* Dropout (0.4)
* Softmax Output Layer

---

## 📊 Evaluation Metrics

Model performance was evaluated using:

* Accuracy
* Loss
* Precision
* Recall
* F1-Score
* Classification Report
* Training Time
* Average Epoch Time
* Inference Speed

---

## 🔬 Optimization Experiments

### CNN Experiments

* High Learning Rate
* Low Learning Rate
* Removing Dropout
* Data Augmentation

### FFNN Experiments

* High Learning Rate
* Low Learning Rate
* Removing Dropout
* Deeper Architecture
* Batch Normalization

---

## 📈 Visualizations

The project includes several visual analyses, including:

* Class Distribution
* Sample MRI Images
* Learning Curves
* Accuracy Comparison
* Loss Comparison
* Training Time Comparison
* Inference Speed Comparison
* Validation Accuracy Comparison for Optimization Experiments

---

## ▶️ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YourUsername/Brain-Tumor-MRI-Classification.git
```

### 2. Install the required packages

```bash
pip install -r requirements.txt
```

### 3. Download the dataset

Download the dataset from Kaggle and place the **Training** and **Testing** folders in the project directory.

### 4. Run the project

Execute the notebook or Python script to train and evaluate the models.

---

## 📌 Results

The experimental results demonstrate that the **Convolutional Neural Network (CNN)** significantly outperformed the **Feedforward Neural Network (FFNN)** in medical image classification.

Key findings include:

* Higher classification accuracy
* Better Precision, Recall, and F1-Score
* Stronger generalization on unseen MRI images
* Reduced overfitting
* More stable learning behavior

Although the CNN required slightly more training time, it achieved considerably better overall performance, making it the preferred architecture for this task.

---

## 📁 Repository Structure

```text
Brain-Tumor-MRI-Classification/
│
├── Brain_Tumor_Classification.ipynb
├── README.md
├── requirements.txt
├── Training/
├── Testing/
└── Results/
```

---

## 👩‍💻 Author

Farida Mohamed

Computer Science Student with a strong interest in Artificial Intelligence, Machine Learning, Deep Learning, and Data Analytics. Passionate about building AI-driven solutions and applying data science techniques to solve real-world problems.

LinkedIn: https://www.linkedin.com/in/farida-mohamed-3b3b17328?utm_source=share_via&utm_content=profile&utm_medium=member_android

This project was developed as part of a Deep Learning study to explore and compare neural network architectures for automated Brain Tumor MRI Classification using TensorFlow and Keras.
