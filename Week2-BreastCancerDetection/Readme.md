# 🧪 Breast Cancer Detection Using Histopathological Images  

This project is part of **Week 2** of my internship practice series. The goal was to build and train **Convolutional Neural Networks (CNNs)** and apply **Transfer Learning** to classify breast histopathological images as **benign (non-cancerous)** or **malignant (cancerous)**.  

---

## 📊 Dataset  
- **Source**: [Kaggle Breast Histopathology Images](https://www.kaggle.com/paultimothymooney/breast-histopathology-images)  
- **Subset Used**: ~500+ images for training/testing  
- **Classes**:  
  - `benign` (non-cancerous)  
  - `malignant` (cancerous)  

---

## 🔧 Data Preprocessing  
- Resized all images to **128×128** (or **224×224** for pre-trained models)  
- Normalized pixel values to **[0, 1]**  
- Converted grayscale images to **RGB** if required  
- Used **PyTorch `ImageFolder` and `DataLoader`** for dataset loading and batching  

---

## 🧠 Model Architectures  

### 1️⃣ Custom CNN (Baseline)  
- 3 Convolutional layers with ReLU + MaxPooling  
- Fully connected classifier  
- Achieved ~**73% accuracy**  

### 2️⃣ VGG16 (Transfer Learning)  
- Pre-trained VGG16 from `torchvision.models`  
- Frozen convolutional base, replaced classifier with **Linear(4096 → 2)**  
- Initial training showed poor accuracy due to incorrect freezing; corrected later  

### 3️⃣ ResNet50 (Transfer Learning)  
- Pre-trained ResNet50  
- Replaced fully connected layer with custom classifier  
- Performance varied due to freezing/unfreezing; ResNet18 suggested for small datasets  

---

## 📈 Evaluation Metrics  
- Training and validation **accuracy & loss**  
- Loss function: **CrossEntropyLoss**  
- Optimizer: **Adam**  
- Observed issues:  
  - Accuracy stuck around ~50% if normalization or freezing not applied properly  
- Best results came from **custom CNN** for this dataset  

---

## 📷 Visualization  
- Used `matplotlib` to display random images from each class  
- Predicted individual test images and displayed labels  

---

## 📌 How to Run  
1. Download the dataset from Kaggle  
2. Preprocess images (resize, normalize)  
3. Choose the model to train:  
   - Custom CNN  
   - VGG16 (Transfer Learning)  
   - ResNet50 (Transfer Learning)  
4. Train for **10–25 epochs**  
5. Evaluate and visualize results  

---

## 🛠️ Technologies Used  
- **Python 3.x**  
- **Deep Learning**: PyTorch, torchvision  
- **Data Handling**: DataLoader, ImageFolder  
- **Visualization**: matplotlib  
- **Platform**: Google Colab (GPU), Kaggle  

---

## ✨ Author  
**Varisha Sajjad**  
🌐 [GitHub](https://github.com/VarishaSajjad)
