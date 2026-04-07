🤟 Sign Language Recognition using Machine Learning

📌 Project Overview

This project is a real-time Sign Language Recognition system that detects hand gestures using a webcam and converts them into readable text and speech. It helps bridge the communication gap between normal people and the hearing/speech impaired community.

The system uses MediaPipe for hand tracking and Machine Learning (Random Forest) for gesture classification.

---

🚀 Features

- Real-time hand gesture detection
- Alphabet (A–Z) and number (0–9) recognition
- Voice output using text-to-speech
- High accuracy with trained model
- User-friendly interface

---

🧠 Tech Stack Used

👨‍💻 Programming Language

- Python

👁 Computer Vision

- OpenCV → For webcam access and image processing
- MediaPipe → For hand detection and landmark extraction

🤖 Machine Learning

- Scikit-learn → Random Forest Classifier for prediction

🔊 Text-to-Speech

- pyttsx3 → Converts predicted text into speech

📊 Data Handling

- NumPy → Numerical operations
- Pandas → Dataset handling

💾 Model Storage

- Joblib → Save and load trained model (.pkl)

💻 Frontend / UI

- Streamlit → Web - based user interface for real-time prediction display 

🧰 Tools

- VS Code → Development environment
- Git & GitHub → Version control



## 📁 Project Structure

```
Sign-Language-Recognition/
│
├── app.py
├── collect_data.py
├── train_model.py
├── predict_live.py
│
├── dataset/
│   ├── A/
│   ├── B/
│   └── ...
│
├── gesture_model.pkl
├── label_encoder.pkl
├── requirements.txt
└── README.md
```


📸 Dataset Collection

👉 Step 1: Run data collection script

python collect_data.py

👉 Step 2: Enter label

Example:

A

👉 Step 3: Show your hand gesture in front of camera

- Images will be captured automatically
- Around 300–500 images per class are recommended

📂 Dataset Location

All collected images are stored in:
```
dataset/<label>/
```
Example:
```
dataset/A/
dataset/B/
```
---

🧹 Dataset Preparation

- Ensure images are clear and properly captured
- Maintain consistent lighting and background
- Avoid blurry or incorrect gestures

---

🏋️ Model Training

👉 Run training script

python train_model.py

🔍 What happens:

- Loads dataset
- Extracts hand landmarks using MediaPipe
- Trains Random Forest model
- Saves model files:

gesture_model.pkl
label_encoder.pkl

---

🎯 Prediction (Real-Time Detection)

👉 Run prediction

streamlit run app.py

(or)

python predict_live.py

🔍 What happens:

- Opens webcam
- Detects hand using MediaPipe
- Predicts gesture using trained model
- Displays output on screen
- Converts text → speech

---

⚙️ Installation & Setup

👉 Step 1: Clone repository

git clone https://github.com/SahuSujeeth/Sign-Language-Recognition-Using-ML.git
cd Sign-Language-Recognition-Using-ML

👉 Step 2: Install dependencies

pip install -r requirements.txt

---

▶️ How to Run Project

1️⃣ Collect dataset (optional if dataset already exists)

python collect_data.py

2️⃣ Train model

python train_model.py

3️⃣ Run real-time prediction

python app.py

---

📊 Results

- Real-time gesture recognition achieved
- Good accuracy with proper dataset
- Smooth prediction using Random Forest
- Works efficiently on CPU

---

🔮 Future Scope

- Upgrade to CNN for higher accuracy
- Deploy as mobile application
- Add sentence formation
- Improve UI using advanced frameworks
- Multi-language speech output

---

🤝 Conclusion

This project successfully demonstrates a real-time sign language recognition system using computer vision and machine learning techniques. It provides an effective solution to improve communication accessibility.

---

📌 Author

Sahu Sujeeth

---

⭐ GitHub

If you like this project, give it a ⭐ on GitHub!