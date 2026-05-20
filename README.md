# AI-Powered Interactive Learning Assistant for Classrooms

## 🚀 Overview

**AI-Powered Interactive Learning Assistant** is a multimodal AI system designed to enhance classroom learning experiences by enabling real-time interaction between students and an AI assistant. It processes **text**, **voice**, and **visual queries** and provides **contextual answers**, **visual aids**, and **student engagement monitoring** via facial expressions and head pose detection.

---

## 🎯 Objective

- Dynamically answer student queries in real-time using:
  - 📝 Text input
  - 🎤 Voice input (speech-to-text)
  - 🖼️ Visual input (images, diagrams)
- Analyze student **engagement and attention** via webcam.
- Provide **contextual explanations** with **charts and diagrams**.

---

## 🛠 Features

| Feature                          | Description |
|----------------------------------|-------------|
| ✅ Text & Voice-based QA         | Ask questions using text or voice input and receive detailed AI-generated explanations. |
| ✅ Visual Question Answering     | Upload images, diagrams, or screenshots and ask contextual questions related to them. |
| ✅ AI-generated Study Notes      | Generates structured learning content and explanations for classroom topics. |
| ✅ Quiz Generation               | Automatically creates MCQ-based quizzes from generated explanations for self-assessment. |
| ✅ Engagement Detection          | Detects student attention and engagement using webcam-based emotion and head pose analysis. |
| ✅ Disengagement Alerts          | Triggers alerts when students appear distracted or disengaged during learning sessions. |
| ✅ Flask-based Web Interface     | Interactive single-page web application integrating all AI modules together. |

---

## 🧠 Models Used

| Task                           | Model / Technology Used                              | Framework / API |
|--------------------------------|------------------------------------------------------|-----------------|
| Text & Voice Question Answering | Gemini 2.0 Flash                                    | Google Generative AI API |
| Visual Question Answering      | Gemini Multimodal Processing                         | Google Generative AI API |
| Emotion Recognition            | `emotions-recognition-retail-0003`                  | OpenVINO |
| Head Pose Estimation           | `head-pose-estimation-adas-0001`                    | OpenVINO |
| Face Detection                 | `face-detection-retail-0004`                        | OpenVINO |
| Speech-to-Text                 | SpeechRecognition + Google STT                      | Python Library |

---

## 🧰 Tech Stack

### Languages
- Python 3
- HTML5 / CSS3 / JavaScript

### Backend
- Flask – Handles routes, API integration, image uploads, and template rendering.
- Requests – Used for HTTP communication with Gemini APIs.
- SpeechRecognition – Converts voice input into text.
- OpenCV – Webcam processing and real-time video analysis.
- OpenVINO Toolkit – Emotion recognition, face detection, and head pose estimation.
- Base64 / JSON / OS / Tempfile – File handling and API request processing.

### Frontend
- HTML + CSS – Responsive user interface for classroom interaction.
- JavaScript – Handles voice recording, quiz interaction, webcam integration, and dynamic UI updates.

---

## ⚙ Core Features & Technologies

### 1. Text Question Answering
- Accepts student questions through text input.
- Uses Gemini 2.0 Flash to generate contextual educational explanations.
- Produces structured and easy-to-understand learning content.

### 2. Voice-based Learning Assistant
- Supports voice input using browser speech recognition.
- Converts speech into text and processes it using the AI backend.
- Returns detailed answers for spoken classroom questions.

### 3. Visual Question Answering
- Allows students to upload images, diagrams, or screenshots.
- Uses multimodal AI processing to answer image-related questions.
- Supports educational diagrams and classroom visual materials.

### 4. Quiz Generation
- Generates MCQ quizzes automatically from AI-generated explanations.
- Helps students perform self-assessment and knowledge evaluation.
- Displays scores and highlights correct answers interactively.

### 5. Engagement & Attention Monitoring
- Detects student emotions such as happy, sad, angry, or neutral.
- Tracks head movement using yaw, pitch, and roll estimation.
- Helps monitor classroom attention and participation.

### 6. Disengagement Alerts
- Detects distracted behavior or lack of attention.
- Sends alerts when students look away for long durations.
- Improves interactive classroom learning experiences.

---

## 📁 Project Structure

```bash
AI-Learning-Assistant/
│
├── app.py                     # Main Flask application
├── templates/
│   └── index.html             # Frontend user interface
├── static/                    # CSS, JavaScript, images
├── uploads/                   # Uploaded image storage
├── requirements.txt           # Python dependencies
└── README.md                  # Project documentation

## ▶ How to Run (Basic)

Install dependencies:

```bash
pip install -r requirements.txt
```

Set the Gemini API key (for example, by replacing `API_KEY` in `app.py` or loading it from the environment).

Start the Flask app:

```bash
python app.py
```

Open the app in a browser at:

```bash
http://127.0.0.1:5000/
```
