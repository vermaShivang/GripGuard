
# GripGuard 🚗🛡️  
**Snap, Scan, Secure your Ride**  

GripGuard is an AI-powered image processing application that automatically detects tyre defects using convolutional deep learning techniques. This project uses state-of-the-art models like ResNet101 and EfficientNetB5 to classify tyre images into `good` or `defective` categories, enabling predictive maintenance, enhancing safety, and reducing manual inspection effort.

---

## 🧠 Project Highlights

- 🔍 **Use Case**: Tyre quality inspection via visual classification (good vs. defective)
- 🧰 **Deep Learning Models**: ResNet101 and EfficientNetB5 with transfer learning
- 📸 **Dataset**: 1,854 labelled tyre images (defective & good)
- ⚙️ **Frameworks**: TensorFlow, Keras, Gradio (optional UI)
- 📈 **Performance**:
  - ResNet101: 94.88% validation accuracy, 98.87% test accuracy
  - EfficientNetB5: 92.99% validation accuracy, 97.63% test accuracy

---

## 📁 Dataset

You can access the dataset here:
- [Mendeley Tyre Dataset](https://data.mendeley.com/datasets/bn7ch8tvyp/1)
- [Kaggle Tyre Classification](https://www.kaggle.com/datasets/warcoder/tyre-quality-classification)

**Structure**:
```
/data/
    /defective/
    /good/
```

---

## 🚀 Features

- 📊 Class balancing using `compute_class_weight`
- 🧪 Evaluation using confusion matrix & classification report
- 🔧 EDA for data quality insights
- 📱 Optional Gradio integration for live predictions
- 📦 Exportable models for web/mobile deployment

---

## 🛠️ How It Works

1. **Data Preprocessing**: Images resized to 256x256, normalized
2. **Model Architecture**:
   - Use pre-trained ResNet101/EfficientNetB5
   - GlobalAveragePooling + Dense (softmax) layer for binary classification
3. **Training**:
   - Optimizer: Adam
   - Loss: `sparse_categorical_crossentropy`
   - Early stopping for efficient training
4. **Evaluation**:
   - Accuracy, Loss, Precision, Recall, F1-score
   - Confusion Matrix
5. **Deployment Ready**:
   - Gradio UI (optional)
   - Can be converted to web/mobile using Flask, Django, React Native

---

## 🧪 Results

| Model         | Val Accuracy | Test Accuracy | F1-Score |
|---------------|--------------|---------------|----------|
| EfficientNetB5| 92.99%       | 97.63%        | 0.98     |
| ResNet101     | 94.88%       | 98.87%        | 0.99     |

---

## 🔮 Future Work

- Mobile/web app deployment with Flask + React Native
- Vision Transformers and EfficientNetV2 experimentation
- Grad-CAM explainability integration
- Continuous learning via online data pipelines

---

## 📚 References

1. [Tire Crack Detection - Scientific Reports](https://doi.org/10.1038/s41598-023-35227-z)
2. [Tire Quality via Deep Vision - IJERT](https://www.ijert.org/research/quality-inspection-of-tire-using-deep-learning-based-computer-vision-IJERTV8IS110337.pdf)
3. [Tire Defect X-Ray Detection - arXiv](https://arxiv.org/abs/2402.18527)

---

## 👨‍🎓 Author

**Shivang Verma**  
B.Tech CSE  
Graphic Era Deemed University  
Under guidance of Mr. Krishna Yadav  

---

> **“Better Tyres. Safer Rides.” – Powered by AI**
