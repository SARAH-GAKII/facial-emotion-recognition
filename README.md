# Facial Emotion Recognition using Deep Learning

## Overview
This project develops a deep learning-based computer vision system to classify human facial expressions into emotional categories. Facial emotion recognition is a key component of affective computing, enabling machines to interpret human emotional states from visual cues.

The model performs multi-class classification on grayscale facial images to identify four emotions:
- Happy  
- Sad  
- Surprise  
- Neutral  

---

## Dataset
The dataset consists of labeled facial images organized into:
- Train set  
- Validation set  
- Test set  

**Key characteristics:**
- Image resolution: 48 × 48 pixels  
- Grayscale images  
- 4 emotion classes: happy, sad, surprise, neutral  

---

## Project Workflow

### 1. EDA & Data Preprocessing 
- Class distribution analysis  
- Validation of image quality
- Image normalization  
- Data augmentation  

### 2. Model Development

#### Custom CNN Architectures 
#### Transfer Learning Models
- Benchmarked against:
  - VGG16  
  - ResNet  
  - EfficientNet  

---

## Evaluation Strategy
Models were evaluated using:
- Accuracy  
- Loss  
- Precision  
- Recall  
- F1-score  

Additionally:
- Class-level performance analysis  
- Confusion matrix evaluation  
- Generalization and overfitting assessment  

---

## Results

| Model | Test Accuracy | Test Loss | Precision | Recall | F1-Score |
|------|--------------|----------|-----------|--------|----------|
| CNN Model 1 | 71.9% | 0.665 | 0.73 | 0.72 | 0.72 |
| VGG16 | 72.7% | 0.728 | 0.75 | 0.73 | 0.73 |
| ResNet | 75.0% | 0.828 | 0.76 | 0.75 | 0.75 |
| EfficientNet | 75.8% | 0.808 | 0.78 | 0.76 | 0.76 |
| Complex CNN | 81.3% | 0.707 | 0.81 | 0.81 | 0.81 |
| CNN Model 2 | **83.6%** | **0.454** | 0.84 | 0.84 | 0.84 |

- Best custom CNN achieved:
  - ~84% test accuracy  
  - Lowest loss among all models  
- Transfer learning models underperformed compared to custom CNNs  

---

## Key Insights

#### Custom CNNs outperformed transfer learning models
- Domain-specific architectures performed better than pretrained models  
- Likely due to mismatch between ImageNet features and grayscale FER data  

#### Expression-specific difficulty varies
- High-intensity emotions (happy, surprise) are easier to classify  
- Subtle emotions (neutral, sad) show higher confusion  

#### Model complexity does not guarantee better performance
- Deeper models did not consistently improve results  
- Simpler architectures with better generalization performed best  

#### Generalization matters 
- Model selection was based on both accuracy and loss  
- Lower loss indicated better confidence and stability  

---

## Model Behavior

- Stable training dynamics  
- Good generalization performance  
- No strong signs of overfitting

- <img width="1388" height="490" alt="image" src="Training Performance.png" />

---

## Technologies Used

- Python  
- TensorFlow / Keras  
- OpenCV  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Google Colab (GPU training)  

---

## Real-World Applications

- Emotion-aware virtual assistants  
- Mental health monitoring systems  
- Customer experience analytics  
- Human-computer interaction systems
- Driver fatigue and emotion detection systems
- Education technology

---

## Repository Content

- **[Facial Emotion Detection Notebook](Facial_Emotion_Detection_Project.ipynb)**
 
 
