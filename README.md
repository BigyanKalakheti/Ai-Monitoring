# 👁️ Real-Time Face Verification System

A real-time face verification system built with **React**, **MediaPipe**, and **FaceAPI.js**. This application verifies a user's identity using face recognition and alerts on unauthorized or suspicious face activity.

---

## 🚀 Features

* ✅ **Face Enrollment** – Enroll a single user's face
* 🧠 **Real-Time Face Recognition**
* 🢍 **Alerts on No Face / Multiple Faces / Unauthorized Face**
* 🔊 **Audio and Vibration Notifications**
* 📜 **Live Event Logs**
* 🖼️ **Canvas Overlay for Face Detection**

---

## 🛠️ Technologies Used

* React
* @mediapipe/face\_detection
* face-api.js
* react-toastify
* HTML5 Canvas
* Web Audio API
* Vibration API

---

## 📦 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Download FaceAPI Models

Download the following models from [face-api.js GitHub](https://github.com/justadudewhohacks/face-api.js/tree/master/weights) and place them in `public/models/`:

* `face_landmark_68_model-weights_manifest.json`
* `face_recognition_model-weights_manifest.json`
* `tiny_face_detector_model-weights_manifest.json`

**Folder structure should look like:**

```
public/
  └── models/
        ├── face_landmark_68_model-weights_manifest.json
        ├── face_recognition_model-weights_manifest.json
        └── tiny_face_detector_model-weights_manifest.json
```

### 4. Run the App

```bash
npm run dev
```

Visit: [http://localhost:5173](http://localhost:5173)

---

## 🡩‍🏫 Usage Instructions

1. Click on **"Enroll Face"** to capture and register your face.
2. Keep your face visible and steady in front of the webcam.
3. The system will:

   * ✅ Show "Authorized Face Detected" if matched
   * ⚠️ Show warning if no face or multiple faces are seen
   * 🚨 Alert if an unauthorized face is detected

All events are logged with timestamps and displayed on the page.

---

## 📁 Project Structure

```
src/
├── components/
│   └── RealTimeFaceVerification.jsx
├── App.jsx
└── index.js

public/
└── models/
    ├── face_landmark_68_model-weights_manifest.json
    ├── face_recognition_model-weights_manifest.json
    └── tiny_face_detector_model-weights_manifest.json
```

---

## ✅ Future Improvements

* Multi-user enrollment
* Spoof detection (anti-photo attack)
* Log export as PDF/CSV
* Admin dashboard for monitoring

---

## 🧑 Author

**Bigyan Kalakheti**
*Cybersecurity & AI Enthusiast*

---

## 📄 License

This project is licensed under the MIT License.
