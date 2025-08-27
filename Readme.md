# 🫁 Lung Cancer Detection using Convolutional Neural Networks (CNN)

![Header](https://img.shields.io/badge/AI%20for%20Good-Deep%20Learning-blueviolet?style=for-the-badge)  
![Status](https://img.shields.io/badge/Status-Study%20Project-green?style=for-the-badge)  
![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python)  
![TensorFlow](https://img.shields.io/badge/TensorFlow-CNN-orange?style=for-the-badge&logo=tensorflow)  

---

## 📌 Overview  
This project explores the use of **Convolutional Neural Networks (CNNs)** for **automated lung cancer classification** from **CT scan images**.  

The model classifies scans into:  
- ✅ **Normal cases** (healthy lungs)  
- 🟢 **Benign cases** (non-cancerous tumors)  
- 🔴 **Malignant cases** (cancerous tumors)  

⚠️ **Disclaimer:** This is a **study project** only.  
It is **not medically certified** and should **not be used for clinical diagnosis**.  

---

## 📂 Dataset Samples  

Below are some sample CT scans from the dataset:  

<img width="840" height="754" alt="image" src="https://github.com/user-attachments/assets/958bad0f-ffc1-49bc-974f-5ceeac9ec891" />


---

## 🧠 Why CNNs?  

Medical images (like CT scans) contain **spatial patterns** that are hard to detect with traditional ML methods.  

- **Convolutional layers** → capture features such as edges, textures, and lesions.  
- **Pooling layers** → reduce noise and focus on important features.  
- **Fully connected layers** → classify features into categories (Normal, Benign, Malignant).  

### Example CNN Pipeline  
<img width="875" height="468" alt="image" src="https://github.com/user-attachments/assets/2e7b282b-7a73-4141-b267-b89f0a91f58a" />



---

## ⚙️ Training Process  

- **Framework:** TensorFlow / Keras  
- **Optimizer:** Adam  
- **Loss function:** Categorical Crossentropy  
- **Batch size:** 32  
- **Epochs:** 20  
- **Validation Split:** 20%  

During training, images were preprocessed by:  
- Resizing to a uniform size  
- Normalizing pixel values  
- Data Augmentation (rotation, zoom, flipping) to prevent overfitting  

---

## 📈 Model Performance  

### Accuracy vs Epochs
<img width="809" height="736" alt="image" src="https://github.com/user-attachments/assets/7685fc97-2b1f-4b4a-bf81-ef80afb67efb" />


- Training Accuracy → **~95%**  
- Validation Accuracy → **~95%**  
- The curves are close → strong generalization  

### Loss vs Epochs  
- Training & Validation loss steadily decreased  
- No signs of major overfitting  

---

## 🛠️ Tech Stack  
- **Language:** Python 🐍  
- **Deep Learning:** TensorFlow / Keras  
- **Data Handling:** NumPy, Pandas  
- **Visualization:** Matplotlib, Seaborn  
- **Preprocessing:** OpenCV, Scikit-learn  

---

## 🚀 How to Run  

1️⃣ Clone the repo:  
```bash
git clone https://github.com/yourusername/lung-cancer-detection.git
cd lung-cancer-detection
jupyter notebook Lung_cancer_predection_ML.ipynb
