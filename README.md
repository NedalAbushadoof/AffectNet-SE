# AffectNet-SE  
### An Attention-Based Facial Emotion Recognition System for Imbalanced Real-World Data  

AffectNet-SE is a deep learning based Facial Emotion Recognition (FER) system designed to work on **small, noisy, and imbalanced real-world datasets**. The system classifies facial images into five emotion categories: **Angry, Fear, Happy, Sad, and Surprise**.

This project was developed as part of the **Pattern Recognition and Information Analysis** course at the **University of Jordan (KASIT)**.

---

## Motivation

Facial Emotion Recognition in real-world conditions is challenging due to:

- Subtle and visually similar expressions  
- Varying lighting, pose, and image quality  
- Limited training data  
- Strong class imbalance  

The dataset used in this project was **manually collected by university students**, making it realistic but noisy. AffectNet-SE was designed specifically to handle these challenges.

---

## Method Overview

The system is based on a deep neural network that combines:

- **EfficientNet-B0** pretrained on ImageNet for feature extraction  
- **Squeeze-and-Excitation (SE) Attention** to emphasize important facial features  
- **Focal Loss with class weighting** to address data imbalance  
- **Weighted random sampling** during training  

This architecture enables the model to focus on key facial regions such as the eyes, eyebrows, and mouth, which are critical for distinguishing emotions.

---

## Dataset

The dataset consists of five emotion classes:

| Emotion   | Images |
|----------|--------|
| Angry    | 95     |
| Fear     | 192    |
| Happy    | 230    |
| Sad      | 142    |
| Surprise | 86     |

Images were captured in real environments and included multiple formats (HEIC, JPG, PNG), requiring preprocessing and normalization.

---

## Results

AffectNet-SE achieved strong and balanced performance across all emotions, including minority classes. The final system reached approximately:

- **95% accuracy**  
- **0.93 Macro-F1 score**  
- **0.95 Weighted-F1 score**  

These results demonstrate the effectiveness of attention-based learning and imbalance-aware training for FER on real-world data.

---

## Team

This project was developed by:

- Nedal Abushadouf  
- Mohammed Alhassanat  
- Wasan Alhabahbeh  
- Cynthea Qaqish  
- Mohammed Abulathoa  
- Khalil Alhileh  

University of Jordan – King Abdullah II School of Information Technology (KASIT)
