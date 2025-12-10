🎭 Emotion Detection — Browser-Based AI Emotion Classifier

Emotion Detection is a real-time, interactive web tool built completely in React and powered by TensorFlow.js.
It uses your webcam (with permission) to detect your face and classify emotions such as:

😀 Happy • 😔 Sad • 😡 Angry • 😮 Surprised • 😐 Neutral • 😨 Fearful • 🤢 Disgusted

All processing happens inside your browser, ensuring complete privacy and zero data upload.

🌟 Overview

This project demonstrates how modern deep learning models can run entirely on the client side.
With TensorFlow.js providing GPU-accelerated inference and face-api.js handling face analysis, users get instant feedback on their expressions without installing anything.

The application is designed to be simple, clean, and highly accessible — perfect for learning, demos, and emotion-aware UI exploration.

📂 Folder & File Structure

A clear breakdown of the key directories and their purpose:

Emotion-Detection/
│
├── public/
│   ├── models/
│   │   └── Pre-trained ML models for face & emotion detection
│   └── Static files accessible directly by the browser
│
├── src/
│   ├── components/
│   │   └── EmotionDetector.jsx  → Core component managing webcam, detection, overlay, UI
│   │
│   ├── App.jsx                 → Main UI layout and routing container
│   ├── main.jsx                → Application entry point for rendering React
│   └── styles.css              → Global UI styling for layout and components
│
├── index.html                   → Base HTML template where the app is mounted
├── package.json                 → Project metadata, dependencies, and scripts
├── vite.config.js               → Build and optimization settings for Vite
└── README.md                    → Documentation (this file)

🤖 How the Emotion Detection Works

The app follows a streamlined AI flow:

Webcam Activation
The user grants permission for the browser to access their camera.

Model Loading
Deep learning models for face detection, facial landmark detection, and emotion recognition are loaded from public/models.

Real-time Analysis
Using TensorFlow.js and face-api.js, each video frame is processed to detect a face and extract key emotional signals.

Emotion Classification
The AI predicts emotions like happy, sad, angry, surprised, neutral, disgusted, or fearful — updating instantly.

Visual Feedback
Bounding boxes and emotion labels are displayed on top of the video feed for an interactive experience.

Everything happens locally — there is no backend server.

🧰 Technology Stack (Explained Simply)

React — Organizes the UI into reusable components

Vite — Fast development tooling for modern React apps

TensorFlow.js — Runs deep learning directly in the browser

face-api.js — Provides pretrained face detection and emotion models

WebGL — Accelerates AI inference using your device’s GPU

The combination of React and TensorFlow.js makes this project lightweight yet powerful.

🔒 Privacy & Safety

Your webcam data stays completely on your device.
No images are uploaded, recorded, stored, or transmitted to any server.

You remain in full control at all times — simply close the tab to stop the process instantly.

🎯 Use Cases

This tool can be used for:

Learning about browser-based AI

Classroom demonstrations

Emotion-aware UI research

Human-computer interaction studies

Interactive experiences & games

Portfolio projects showcasing AI skills

🚀 Future Improvements

Planned enhancements:

Multi-face emotion detection

Emotion history timeline and graphs

Screenshot & download feature

Audio or visual reactions based on emotion

Dark/light theme support

Optimized mobile layout

More advanced deep learning models

🤝 Contributing

Ideas, improvements, and collaborations are welcome!
You may:

Suggest features

Improve UI/UX

Enhance model accuracy

Add documentation

Feel free to open issues or submit pull requests.

📜 License

This project is open-source and free for learning, experimentation, and innovation.

🙌 Final Note

Thank you for exploring this project!
Emotion Detection shows how far browser-based AI has come — running complex models entirely on your device with no setup required.
Feel free to build on top of this, experiment with your own expressions, or integrate the detector into creative web apps.