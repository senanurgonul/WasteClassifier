# WasteClassifier

**WasteClassifier** is a classification model that distinguishes between household and recyclable waste using image processing. This project was developed to promote environmental awareness and automate waste management.

With increasing consumption habits today, the amount of waste has also risen significantly. Proper separation of waste is critical for effective recycling. We developed a solution to this problem: an AI model that can classify waste types from images.

---

## 🎯 Project Goals

- Support recycling systems through the **automatic classification of waste**  
- Develop a model trained with **real-world examples**  
- Achieve **high accuracy** using data augmentation and transfer learning techniques  

---

## 📁 Dataset

The dataset is located in the `images/` directory.

---

## 🧠 Method

- **Model:** MobileNetV3 Small (via transfer learning)  
- **Data Augmentation:** Color distortion, rotation, scaling, blurring  
- **Transformations:** Normalize, Resize (256x256)  
- **Evaluation Metrics:** Accuracy, Confusion Matrix, Classification Report  

The data is split into 60% training, 20% validation, and 20% testing. During training, both training and validation losses and accuracies are monitored.

---

## 🔧 Requirements

```bash
pip install torch torchvision matplotlib scikit-learn pillow
```

---

## 🚀 Usage

```bash
git clone https://github.com/kullaniciadi/WasteClassifier.git
cd WasteClassifier

jupyter notebook ‘recyclable and household waste classification.ipynb’
```

You can load the data, train the model, and test it by following the steps in the notebook.


---

