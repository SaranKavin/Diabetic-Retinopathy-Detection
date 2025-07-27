# Diabetic-Retinopathy-Detection
Here is a complete `README.md` file you can use for your **Diabetic Retinopathy Detection Web Application**:

---

# Diabetic Retinopathy Detection - Web Application

This web application allows users to upload retinal images and detect the stage of Diabetic Retinopathy (DR) using a deep learning model built with TensorFlow/Keras.

---

## 📁 Folder Structure

```
project/
├── app.py
├── model/
│   └── dr_model.h5
├── static/
│   └── uploads/
├── templates/
│   ├── index.html
│   └── analyze.html
├── requirements.txt
└── README.md
```

---

## 🚀 How to Run the Application

### 1. **Clone or Download the Repository**

```bash
git clone https://github.com/your-username/diabetic-retinopathy-app.git
cd diabetic-retinopathy-app
```

### 2. **Set Up Virtual Environment**

```bash
python -m venv venv
venv\Scripts\activate        # Windows
# source venv/bin/activate   # macOS/Linux
```

### 3. **Install Required Packages**

```bash
pip install -r requirements.txt
```

If you don't have `requirements.txt`, manually install:

```bash
pip install flask tensorflow pillow numpy
```

### 4. **Place the Model File**

Put the trained model file `dr_model.h5` in the `model/` directory.

> 🔗 You can download a sample DR model from:
> [Kaggle Models for DR](https://www.kaggle.com/arunprasadh/deep-learning-models-for-dr-classification)

### 5. **Run the Flask Server**

```bash
python app.py
```

### 6. **Open in Browser**

Open your browser and visit:
📍 `http://127.0.0.1:5000`

---

## 📷 How to Use

1. On the homepage, click **Choose File** to upload a retinal image.
2. Click **Submit**.
3. The app will display:

   * Detected class (e.g., *Moderate*)
   * Prediction confidence
   * Probability for all DR stages
   * Uploaded image preview

---

## 🤖 Model Information

* **Model Format**: `.h5` (TensorFlow Keras)
* **Input Size**: 224x224 RGB image
* **Classes**:

  * No DR
  * Mild
  * Moderate
  * Severe
  * Proliferative DR
* **Architecture**: Likely CNN-based (e.g., MobileNet, VGG16, or custom CNN)

---

## ✅ Accuracy

> Depends on the model used. If you're using a Kaggle pretrained model, accuracy may range between **70%–90%**.

---

## 🛠 Future Improvements

* Add heatmap visualization (Grad-CAM)
* Add more model options
* Support drag-and-drop uploads
* Deploy on cloud (Heroku, Render, etc.)

---
