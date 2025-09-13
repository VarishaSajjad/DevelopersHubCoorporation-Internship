# 🩺 Medical Image Classification: Skin Cancer & Pneumonia Detection

This project applies deep learning to classify medical images for two tasks:  

1. **Skin Cancer Detection** using the ISIC Skin Cancer dataset.  
2. **Pneumonia Detection** using the Kaggle Chest X-Ray dataset.  

It includes preprocessing, model training, evaluation, and visualization of results.

---

## 📂 Project Structure


---

## 🧪 Task 1: Skin Cancer Detection

- **Dataset**: Subset of [ISIC Skin Cancer Dataset](https://www.isic-archive.com/) (500–1000 images).  
- **Preprocessing**:
  - Resize images to **128×128 pixels**  
  - Normalize pixel values to `[0, 1]`  
- **Model**:
  - Pre-trained **ResNet50** with **Transfer Learning**  
  - Custom dense layer for binary classification (Cancer / Non-Cancer)  
- **Training**:
  - Loss: **Binary Crossentropy**  
  - Optimizer: **Adam**  
- **Evaluation**:
  - Metric: **Accuracy**  
  - Plots: Training vs Validation Accuracy, Loss Graphs  

---

## 🧪 Task 2: Pneumonia Detection

- **Dataset**: Subset of [Kaggle Chest X-Ray Dataset](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia).  
- **Preprocessing**:
  - Resize images to **128×128 pixels**  
  - Normalize pixel values `[0, 1]`  
- **Model**:
  - Custom **CNN** with 2 convolutional layers, pooling, and dense output  
- **Training**:
  - Loss: **Binary Crossentropy**  
  - Optimizer: **Adam**  
- **Evaluation**:
  - Metrics: **Accuracy**, **ROC Curve**  
  - Plots: Accuracy Graphs, ROC Curve  

---

## 📊 Results & Outcomes

- **Skin Cancer Detection (ResNet50)**:
  - Achieved high accuracy due to transfer learning  
  - Generalized well on limited dataset size  

- **Pneumonia Detection (CNN)**:
  - Simple CNN performed effectively on X-Ray images  
  - ROC Curve visualizes classification performance  

- **Deliverables**:
  - Trained models (`.h5` or `.pt` files)  
  - Evaluation plots (Accuracy, Loss, ROC Curve)  
  - Short summary report (1–2 pages)  

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/medical-image-classification.git
   cd medical-image-classification


---

# Author: VarishaSajjad