## 🩺 Automated Pneumonia Detection from Chest X-rays using Deep Learning

### 🔍 Overview

This project demonstrates a deep learning pipeline for **pneumonia detection** using chest X-ray images. By building and comparing models like **Simple CNN**, **ResNet50V2**, and **VGG16**, the aim was to develop a reliable tool that can assist radiologists in faster, more accurate screening.

---

### 🎯 Objectives

* Build deep learning models to classify X-ray images as either **normal** or showing signs of **pneumonia**.
* Compare performance of a custom CNN with transfer learning models.
* Present model performance through clear visualizations and metrics.
* Provide a foundation for future deployment in clinical screening tools.

---

### 🧠 Models Implemented

| Model          | Accuracy | Key Notes                    |
| -------------- | -------- | ---------------------------- |
| **Simple CNN** | \~94.70% | Lightweight and efficient    |
| **ResNet50V2** | \~95.56% | Best-performing model        |
| **VGG16**      | \~92.82% | Solid transfer learning base |

---

### 🛠️ Technologies Used

* **Python**
* **TensorFlow / Keras**
* **OpenCV** for image handling
* **Seaborn & Matplotlib** for visualizations
* **Transfer Learning** for ResNet50V2 and VGG16

---

### ⚙️ How It Works

* Input images are preprocessed (grayscale conversion, resizing to 150×150).
* Data augmentation is applied during training to improve generalization.
* Each model is trained using a balanced dataset with class weights to address label imbalance.
* Evaluation includes accuracy/loss plots, classification reports, and confusion matrices.

---

### 🧪 To Run the Project

```bash
# Install dependencies
pip install tensorflow opencv-python matplotlib seaborn scikit-learn

# Make sure to organize your data into:
# data/
#   └── train/
#         ├── PNEUMONIA/
#         └── NORMAL/
#   └── val/
#   └── test/

# Then run the main script or notebook
python pneumonia_detection.py
```

> ⚠️ *Dataset not included in this repository due to copyright and size limitations. Please use your own dataset of labeled chest X-ray images.*

---

### 📈 Results Overview

* **ResNet50V2** gave the best classification results across all metrics.
* Evaluation metrics like confusion matrix, precision, recall, and F1-score are included.
* Visualizations such as accuracy/loss curves help interpret model performance clearly.

---

### 🚀 Future Additions

* Convert best model into a web app (e.g., Streamlit)
* Add model interpretability using Grad-CAM or heatmaps
* Deploy using TensorFlow Lite for mobile use

---

### 👤 Author

**Sesha Sai Ramineni**
Graduate Student | Health Informatics, Michigan Tech
Passionate about AI in Healthcare and Biomedical Imaging

---

### 📄 License

This project is open for educational and research purposes. Feel free to fork and build on it!
