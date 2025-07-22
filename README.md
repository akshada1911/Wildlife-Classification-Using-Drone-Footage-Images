# Wildlife-Classification-Using-Drone-Footage-Images 

This project leverages drone technology and the YOLOv9 object detection model for **real-time wildlife monitoring**, ensuring **accurate species detection** with minimal human intervention. **Data augmentation** techniques enhance model performance, leading to improved **precision and recall**, making this system a scalable and efficient tool for wildlife conservation.  

---

## 📌 Table of Contents  
- [Introduction](#introduction)  
- [Problem Statement](#problem-statement)  
- [Importance of This Project](#importance-of-this-project)  
- [Methodology](#methodology)  
- [Results and Performance](#results-and-performance)  
- [Conclusion](#conclusion)  

## Introduction  
Wildlife conservation is a critical global challenge, yet **traditional monitoring methods** are inefficient, labor-intensive, and prone to errors. This project **automates wildlife monitoring** using **drone footage based images** equipped with **YOLOv9**, a state-of-the-art object detection model. By providing **real-time, accurate, and noninvasive monitoring**, this system significantly enhances conservation efforts while minimizing human interference.  

---

## Problem Statement  
Manual wildlife monitoring is:  
- **Time-consuming and error-prone**  
- **Inconsistent**, relying on human observations  
- **Limited by environmental factors**  

This project aims to **overcome these challenges** by leveraging deep learning and drone technology.  

---

## Importance of This Project  
✅ **Boosting Conservation Efforts**: Provides **real-time** data for informed decision-making  
✅ **Reducing Human Impact**: Minimizes **disturbance to natural habitats**  
✅ **Improving Accuracy**: Uses **AI-driven object detection** for **reliable species classification**  

---
## ⚙️ Methodology  

### 📌 Data Preparation  
- **Resizing**: Images scaled to `320×320` and `640×640` for consistency  
- **Normalization**: Pixel values scaled to `[0,1]` for training efficiency  
- **Augmentation**: Applied techniques like **flipping, rotation, scaling, HSV adjustments, mosaic, mixup, and copy-paste**  
- **Caching**: Storing images in memory to speed up training
- **Class Labels**: The dataset includes the following wildlife species: 
  - Zebra   
  - Camel  
  - Sheep  
  - Cattle
  - Elephant
  - Seal


### 📌 Model Selection: YOLOv9  
- **Speed & Precision**: Optimized for **real-time** applications  
- **Advanced Feature Extraction**: **Superior small-object detection** for diverse wildlife  

### 📌 Training Process  
| Parameter | Value |  
|-----------|--------|  
| **Model** | YOLOv9 |  
| **Epochs** | 30 |  
| **Batch Size** | 16 |  
| **Image Size** | 640×640 |  
| **Optimizer** | AdamW |  
| **Learning Rate** | Adaptive (starting at `0.01`) |  
| **Regularization** | Weight decay `0.0005` |  

- **Early Stopping** applied to prevent overfitting  

---

## 📊 Results and Performance  

✅ **Loss Analysis**  
📉 **Training & Validation Loss** decreased steadily, indicating effective learning.  

✅ **Precision & Recall**  
✔ **Precision** improved consistently, reaching **90%**.  
✔ **Recall** showed a steady increase, reducing misclassification.  

✅ **mAP@50**  
🚀 Demonstrated continuous improvement over epochs, ensuring **accurate detection & classification**.  

---

## 🏁 Conclusion  
- The **gradual reduction in loss** confirms that the model is learning effectively.  
- **Precision & Recall improvements** indicate enhanced species classification.  
- The project proves that **drones + AI** can **revolutionize wildlife monitoring**.  

---

