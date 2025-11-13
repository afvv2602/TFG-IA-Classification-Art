# 🎨 AI-Powered Artwork Classification App (Android & iOS)

This project is my **Bachelor's Final Degree Project**, consisting of a
complete end-to-end system capable of **classifying artworks into their
corresponding artistic period** using **Deep Learning and Computer
Vision**.

The solution includes:

-   A **mobile application** for Android & iOS (Flutter)
-   A **Python backend** deployed on a local mini-server
-   A **Convolutional Neural Network (CNN)** trained to classify
    artworks across movements such as Baroque, Renaissance,
    Neoclassicism, Impressionism, and Cubism

## 🚀 Features

### 📱 Mobile Application

-   Crossplatform development using **Flutter** and **VSCode**
-   Full classification workflow:
    -   Capture a photo or select one from the gallery
    -   Send the image to the backend
    -   Display the prediction result in real time
-   Clean and educational UI focused on user simplicity
-   Additional sections featuring museums and notable artworks
-   Small social module to share images and browse posts from other
    users

## 🧠 Artificial Intelligence

-   Custom-trained **Convolutional Neural Network (CNN)** for artwork
    classification
-   Dataset preprocessing: normalization, noise reduction, and data
    augmentation
-   Classification across major art movements
-   Model exported for lightweight server-side inference
-   Evaluation and tuning to enhance accuracy and generalization

## 🌐 Backend Architecture

-   Python backend using a lightweight REST framework
-   API endpoints for:
    -   Receiving images from the mobile app
    -   Running inference using the CNN model
    -   Returning classification results
-   Deployment on a local **mini-PC** acting as the model server
-   Basic user management system supporting the social features

## 🏗️ System Architecture

    Mobile App (Android & iOS)
          ↓
      HTTP Request (image)
          ↓
       Python Backend
          ↓
     CNN Model Inference
          ↓
     Classification Result
          ↓
      Response to Client

## 📁 Repository Structure

    TFG-IA-Classification-Art/
    │
    ├── backend/               # Python backend (API + inference)
    ├── model/                 # Trained CNN model + training scripts
    ├── android-app/           # Android Studio project
    ├── ios-app/               # iOS Xcode project
    ├── dataset/               # Dataset or dataset link
    ├── docs/                  # Documentation, diagrams, notes
    └── README.md              # Project overview

## 🛠️ Tech Stack

### Mobile

-   Android/ios (Flutter)

### Backend

-   Python
-   REST API
-   Pillow / OpenCV
-   NumPy

### Machine Learning

-   CNN-based classification
-   TensorFlow / Keras or PyTorch *(adapt this depending on your model)*
-   Data preprocessing & augmentation

## 📦 Installation & Setup

### Backend Setup

``` bash
cd backend
pip install -r requirements.txt
python server.py
```

The backend will start locally (e.g., `http://192.168.1.x:5000/`).\
Ensure the mobile device is connected to the same network.

### Mobile App Setup

#### Android

1.  Open the `android-app/` folder in Android Studio\
2.  Update the backend IP in the configuration file\
3.  Build and run on a device

#### iOS

1.  Open the `ios-app/` folder in Xcode\
2.  Update the backend IP\
3.  Build and run on a physical device (recommended)

## ▶️ Usage

1.  Launch the app\
2.  Capture or upload an image of an artwork\
3.  The app sends the image to the backend\
4.  The backend processes it using the CNN\
5.  The classification result is displayed in the app\
6.  Optionally, share the result via the social module

## 🖼️ Screenshots

    ![Home Screen](docs/screenshots/home.png)
    ![Result](docs/screenshots/result.png)
    ![Museum Info](docs/screenshots/museums.png)

## 📈 Future Improvements

-   On-device inference using TensorFlow Lite\
-   Expanded social functionality\
-   Migration to cloud-based deployment\
-   Improved CNN architectures (ResNet, EfficientNet, etc.)\
-   Larger and more diverse dataset

## 👤 Author

**Adrián Fernández-Vaillo**\
Software Engineer\
- Android & iOS Development\
- Machine Learning & Python\
- Automation
- Email: afvv26002@gmail.com

## 📜 License

This project is for educational and research purposes.\
Contact me if you'd like to reuse or extend any part of the code.

