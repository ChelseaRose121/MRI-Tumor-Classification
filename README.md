# Brain Tumor Classification Using CNN

## Project Overview
This project builds a Convolutional Neural Network (CNN) to classify MRI images of brain scans into four categories of tumor presence. The goal is to support early, accurate diagnosis and assist healthcare professionals in improving patient outcomes through timely treatment.

---

## Dataset
MRI scans across four classes:

| Class            | Training Images | Testing Images |
|------------------|-----------------|----------------|
| Glioma           | 1321            | 300            |
| Meningioma       | 1339            | 306            |
| No Tumor         | 1595            | 405            |
| Pituitary Tumor  | 1457            | 300            |

---

## Preprocessing
- Removed blurred/duplicate images to enhance dataset quality
- Normalized pixel values to range [0, 1]
- Encoded labels into numerical form
- Applied data augmentation for better generalization
- Split dataset: 80% training, 20% testing

---

## Model Architecture
Implemented a CNN using TensorFlow/Keras with the following layers:
- Convolutional layers with ReLU activation
- MaxPooling layers
- Dropout layers to prevent overfitting
- Dense layers leading to softmax output

Trained for **20 epochs** with **early stopping** to avoid overfitting.

---

## Model Performance
- **Test Accuracy**: 94.95%
- **Evaluation Metrics**:
  - Confusion matrix and classification report
  - High precision, recall, and F1-scores across all classes
  - Macro and weighted average F1-score: **0.95**

---

## Key Takeaways & Recommendations
- CNN can effectively classify brain tumors from MRI scans with high accuracy
- Model could be integrated into clinical workflows to support radiologists
- Future versions should be trained on more diverse real-world datasets
- User-friendly front-ends could improve adoption in hospital settings

---

## Future Work
- Expand dataset (higher resolution images, more diversity)
- Experiment with advanced architectures (3D CNNs, ResNet, ensembles)
- Validate model on live clinical data
- Incorporate patient metadata (age, symptoms, etc.) for a hybrid diagnostic tool

---

## How to Use
- Run the Jupyter notebook provided in the `notebooks/` directory
- Make sure required libraries (TensorFlow, Keras, NumPy, etc.) are installed
- Ensure the dataset folder is structured correctly before execution


