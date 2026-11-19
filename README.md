# 🌿 Plant Disease Recognition System Using Deep Learning

An AI-powered web application that identifies plant diseases from leaf images using a Convolutional Neural Network (CNN). The system allows users to upload a leaf image and receive a disease prediction with its confidence score, along with relevant treatment recommendations.

## 📌 Project Overview

Agricultural productivity is significantly affected by plant diseases. Early identification can help farmers take preventive measures and reduce crop losses.

This project uses Deep Learning and Computer Vision to classify plant leaf images into healthy or diseased categories. It provides a simple web interface where users can upload images and obtain predictions automatically.

## ✨ Features

- **Leaf Image Upload:** Upload plant leaf images through a user-friendly web interface.
- **Disease Classification:** Identifies plant diseases using a trained CNN model.
- **38 Disease Categories:** Classifies images into 38 plant disease and healthy categories.
- **Prediction Confidence:** Displays the confidence score of the predicted class.
- **Treatment Recommendations:** Provides relevant disease management suggestions.
- **Web-Based Interface:** Simple and responsive frontend built using HTML, CSS, and JavaScript.

## 🧠 Model Information

The system uses a Convolutional Neural Network (CNN) trained on the PlantVillage dataset.

| Parameter          | Details            |
| ------------------ | ------------------ |
| Model Architecture | CNN                |
| Dataset            | PlantVillage       |
| Total Images       | 54,303             |
| Number of Classes  | 38                 |
| Reported Accuracy  | 96%                |
| Model Format       | `.keras`           |
| Framework          | TensorFlow / Keras |

**Note:** The reported 96% accuracy is the result obtained during model evaluation. Real-world performance may differ due to variations in lighting, backgrounds, image quality, and leaf conditions.

## 📂 Dataset

The project uses the PlantVillage dataset, which contains images of healthy and diseased plant leaves.

- Total images: 54,303
- Total categories: 38
- Includes multiple crops and disease conditions.

Dataset source: [PlantVillage Dataset](https://github.com/spMohanty/PlantVillage-Dataset)

## 🛠️ Technology Stack

**Frontend**

- HTML5
- CSS3
- JavaScript

**Backend**

- Python
- Flask

**Machine Learning**

- TensorFlow
- Keras
- NumPy
- CNN

**Deployment**

- GitHub
- Render

## 📁 Project Structure

```text
Plant-Disease-Recognition/
│
├── app.py
├── model.keras
├── plant_disease.json
├── templates/
│   └── index.html
│
├── static/
│   ├── style.css
│   └── script.js
│
├── README.md
└── .gitignore
```

## ⚙️ Installation and Setup

Follow these steps to run the project locally.

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the project directory

```bash
cd Plant-Disease-Recognition
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

Activate it:

**Windows:**

```bash
venv\Scripts\activate
```

**Linux / macOS:**

```bash
source venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the application

```bash
python app.py
```

### 6. Open in browser

```text
http://127.0.0.1:5000
```

## 🔍 How It Works

1. The user uploads a plant leaf image.
2. The frontend sends the image to the Flask backend.
3. The backend preprocesses the image.
4. The trained CNN model analyzes the image.
5. The model predicts the corresponding disease category.
6. The application displays the predicted disease and confidence score.
7. Relevant treatment recommendations are presented to the user.

## 🚀 Deployment

The application can be deployed using Render.

1. Push the project to GitHub.
2. Create a new Web Service on Render.
3. Connect your GitHub repository.
4. Configure the build command:

```bash
pip install -r requirements.txt
```

5. Configure the start command:

```bash
gunicorn app:app
```

6. Deploy the application and access it through the generated public URL.

## 📊 Future Improvements

- Improve model generalization using real-world leaf images.
- Introduce data augmentation and transfer learning.
- Add support for more crops and disease categories.
- Integrate multilingual support for farmers.
- Develop a mobile-friendly application.
- Provide more detailed disease prevention and treatment recommendations.
- Explore explainable AI techniques such as Grad-CAM.

## 👨‍💻 Author

**Deepak Sheokand**

Bachelor of Technology – Computer Science and Engineering

Interested in Artificial Intelligence, Machine Learning, and Software Development.

## 📄 License

This project is intended for educational and research purposes. Add an appropriate open-source license if you intend to distribute the source code.

---

⭐ If you find this project useful, consider giving the repository a star!
