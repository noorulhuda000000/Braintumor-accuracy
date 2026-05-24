# 🧠 Brain Tumor MRI Classification (Re-run Pipeline)

## 📌 Overview
This project implements a deep learning pipeline to classify brain tumor MRI images into different categories.  

As instructed, the notebook was **re-run cell by cell** on top of the existing notebook to ensure reproducibility and verify results.

---

## ⚙️ 1. Setup & Data Import

- Dataset is imported from Kaggle.
- Directory structure is verified for training and testing data.



---

## 📚 2. Import Required Libraries

The following libraries are used:

- `os`, `numpy`, `pandas` → data handling  
- `matplotlib`, `seaborn` → visualization  
- `sklearn` → evaluation metrics  
- `tensorflow`, `keras` → deep learning  



---

## 🧹 3. Data Preprocessing

### 3.1 Load Data
- Custom functions (`train_df`, `test_df`) are used to:
  - Read image paths  
  - Assign labels  
  - Store data in DataFrame format  

---

### 3.2 Data Exploration
- Class distribution is analyzed for:
  - Training dataset  
  - Testing dataset  

This helps detect imbalance between classes.


---

### 3.3 Train–Validation–Test Split
- Testing data is further divided into:
  - Validation set  
  - Final test set  
- Stratified sampling is used to maintain class balance  

📷 *(Insert screenshot of split results here)*

---

### 3.4 Data Generators & Preprocessing
- Images are:
  - Resized  
  - Normalized  

- `ImageDataGenerator` is used for:
  - Efficient batch loading  
  - Optional augmentation  

📷 *(Insert screenshot of generator setup here)*

---

### 3.5 Sample Visualization
- Class indices are retrieved  
- Sample images are displayed with labels to verify correctness  

📷 *(Insert sample images here)*

---

## 🧠 4. Model Building

- Input shape is defined (e.g., 299×299×3)  
- Deep learning model is constructed (CNN / transfer learning)  
- Model is compiled using:
  - Loss function  
  - Optimizer  
  - Accuracy metric  

📷 *(Insert model architecture diagram here)*

---

## 🏋️ 5. Model Training

- Model is trained using:
  - Training generator  
  - Validation generator  

- Metrics tracked:
  - Accuracy  
  - Loss  

📷 *(Insert training logs / epochs screenshot here)*

---

### 5.1 Performance Visualization

- Training vs Validation Accuracy  
- Training vs Validation Loss  

📷 *(Insert accuracy & loss graphs here)*

---

## 🧪 6. Testing & Evaluation

### 6.1 Model Evaluation
- Model performance is evaluated on:
  - Training set  
  - Validation/Test set  

📷 *(Insert evaluation output here)*

---

### 6.2 Predictions
- Predictions are generated on test data  
- Probabilities are converted into class labels  

📷 *(Insert prediction output here)*

---

### 6.3 Confusion Matrix
- Confusion matrix is computed to analyze classification performance  

📷 *(Insert confusion matrix heatmap here)*

---

### 6.4 Classification Report
Includes:
- Precision  
- Recall  
- F1-score  

📷 *(Insert classification report screenshot here)*

---

### 6.5 Custom Image Prediction
- A function `predict(img_path)` is implemented to:
  - Test new MRI images  
  - Output predicted class  

📷 *(Insert example prediction on custom image here)*

---

## 🎯 Final Goals

- Build a complete deep learning pipeline for MRI classification  
- Ensure reproducibility by re-running all notebook cells  
- Achieve high classification accuracy (~99%)  
- Evaluate model using multiple metrics  
- Enable prediction on new/unseen images  

---

## 🚀 Conclusion

This project demonstrates how deep learning can be applied to classify brain tumor MRI images with high accuracy.  

Re-running the pipeline ensures reliability and reproducibility while providing a full workflow from data preprocessing to final predictions.

---
