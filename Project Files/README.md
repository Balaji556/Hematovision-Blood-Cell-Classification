🩸 HematoVision: Advanced Blood Cell Classification Using Transfer Learning

HematoVision is a deep learning–powered web application designed to classify blood cell images using transfer learning techniques.  
The system integrates a pre-trained Convolutional Neural Network (CNN) with a Flask-based web interface to provide real-time predictions from uploaded microscopic blood smear images.

---

## 🚀 Project Overview

Accurate blood cell classification plays a crucial role in medical diagnostics, particularly in detecting hematological disorders.  
HematoVision leverages transfer learning to build a robust, high-accuracy image classification system capable of identifying different types of blood cells from microscopic images.

The project demonstrates:

- End-to-end deep learning pipeline
- Transfer learning using pre-trained CNN models
- Model deployment using Flask
- Frontend–backend integration
- Real-time image prediction

---

## 🧠 Model Architecture

This project uses **Transfer Learning**, where a pre-trained CNN model is fine-tuned on a blood cell image dataset.

### Key Components:

- Pre-trained base model (e.g., ResNet50 / VGG16 / MobileNet)
- Custom classification head
- Softmax output layer
- Image preprocessing pipeline
- Model saved in `.keras` format

Transfer learning significantly reduces training time while improving accuracy on limited medical datasets.

---

## 🏗️ System Architecture

User Upload → Flask Server → Image Preprocessing → Trained Model → Prediction → UI Display

---

## 🛠️ Tech Stack

### Backend
- Python
- TensorFlow / Keras
- Flask
- NumPy
- PIL / OpenCV

### Frontend
- HTML5
- CSS3 (Animated gradients + Glassmorphism UI)
- Jinja2 Templating

### Development Environment
- Google Colab
- pyngrok (for testing)
- GitHub

---

## 📁 Project Structure


HematoVision/
│
├── app.py
├── model.keras
├── static/
│ └── uploads/
├── templates/
│ ├── home.html
│ └── result.html
├── README.md
└── requirements.txt


---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository

```bash
git clone https://github.com/yourusername/HematoVision.git
cd HematoVision
2️⃣ Install Dependencies
pip install -r requirements.txt

If requirements.txt is not included:

pip install flask tensorflow numpy pillow
3️⃣ Run the Application
python app.py

Open browser and navigate to:

http://127.0.0.1:5000/
🔍 How It Works

User uploads a microscopic blood cell image.

Image is resized and normalized.

Converted into tensor format.

Passed into the trained CNN model.

Model predicts the blood cell category.

Prediction is displayed on the result page.

📊 Model Training Process

Dataset split into training and validation sets.

Data augmentation applied to improve generalization.

Transfer learning applied by freezing base layers.

Fine-tuning performed on top layers.

Model evaluated using accuracy and loss metrics.

📈 Performance

High classification accuracy achieved using transfer learning.

Reduced overfitting via augmentation and dropout.

Efficient inference suitable for real-time prediction.

(Add actual accuracy metrics here if available.)

🎨 Web Application Features

Modern animated gradient UI

Smooth transitions

Image preview after upload

Real-time prediction display

Responsive design

🔮 Future Enhancements

Add model confidence score

Support multiple image uploads

Deploy on cloud platform (AWS / Render / Railway)

Integrate database for prediction logging

Add Grad-CAM visualization for explainability

Build REST API version

🧪 Deployment Options

Local deployment using Flask

Colab testing with ngrok

Cloud deployment via:

AWS EC2

Render

Railway

Heroku

📚 Learning Outcomes

Understanding transfer learning in medical imaging

CNN fine-tuning techniques

Image preprocessing for deep learning

Flask web deployment

End-to-end ML system integration
