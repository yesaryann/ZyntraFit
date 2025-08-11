



# 🏋️‍♂️ ZyntraFit - Smart Fitness Coach with Automated Movement Recognition & Rep Tracking

Welcome to **ZyntraFit** – the future of fitness! This innovative AI-driven platform combines cutting-edge Computer Vision, Advanced Pose Detection, and Deep Learning technologies to revolutionize your workout experience by providing intelligent repetition monitoring and real-time exercise analysis.


🎥 **Demo Video:** [Watch on YouTube](https://www.youtube.com/watch?v=CX7c1tH-Zr4)

---

## 📊 Research Foundation

This application is built upon rigorous academic research:

- **Paper:** "Real-Time Fitness Exercise Classification and Counting from Video Frames"
- **Dataset:** [Kaggle - Real-Time Exercise Recognition Dataset](https://www.kaggle.com/datasets)
- **Research Link:** [ArXiv Paper](https://arxiv.org)

---

## 🎯 Key Features

### 🔥 Core Capabilities

- **Intelligent Exercise Detection**: Automatically identifies workout movements in real-time
- **Precision Rep Counting**: Tracks repetitions with exceptional accuracy
- **Live Webcam Integration**: Train with instant feedback using your camera
- **Video Analysis Tools**: Upload workout videos for comprehensive analysis
- **AI Fitness Assistant**: Get personalized guidance through our smart chatbot

### 💡 What Makes It Special

- Real-time pose estimation using MediaPipe
- BiLSTM neural networks for robust exercise classification
- Angle-based movement analysis for precise repetition detection
- User-friendly web interface powered by Streamlit
- Comprehensive exercise library with form demonstrations

---

## 🛠️ Technical Architecture

### 📁 Project Organization
```

├── main.py                           # Streamlit application entry point
├── ExerciseAiTrainer.py             # Exercise-specific pose analysis engine
├── AiTrainer\_utils.py               # Image processing and calculation utilities
├── PoseModule2.py                   # MediaPipe pose estimation handler
├── chatbot.py                       # OpenAI-powered fitness assistant
├── extract\_features.py              # Video landmark and angle extraction
├── create\_sequence\_of\_features.py  # Dataset generation with 30-frame sequences
├── train\_bidirectionallstm.py      # BiLSTM model training pipeline
├── requirements.txt                 # Python dependencies
├── shoulder\_press\_form.mp4          # Exercise demonstration video
├── thesis\_bidirectionallstm\_label\_encoder.pkl  # Pre-trained label encoder
├── thesis\_bidirectionallstm\_scaler.pkl         # Feature scaling model
└── final\_forthesis\_bidirectionallstm\_and\_encoders\_exercise\_classifier\_model.h5  # Trained BiLSTM model

````

---

## 🚀 Quick Start Guide

### 📋 Prerequisites

- Python 3.7 or higher
- Virtual environment (recommended)
- Webcam (for real-time features)

### ⚡ Installation Steps

**1. Clone the Repository**
```bash
git clone https://github.com/yesaryann/ZyntraFit.git
cd ZyntraFit
````

**2. Create Virtual Environment**

```bash
python -m venv fitness_env
source fitness_env/bin/activate  # Windows: fitness_env\Scripts\activate
```

**3. Install Dependencies**

```bash
pip install -r requirements.txt
```

**4. Launch Application**

```bash
streamlit run main.py
```

---

## 🎮 Application Features

### 🎯 Navigation Menu

The intuitive sidebar provides access to four main modules:

#### 📹 Video Analysis Suite

* Upload workout recordings for detailed movement analysis
* Automated rep counting based on pose estimation
* Exercise form evaluation and feedback

#### 🔴 Live Webcam Mode

* Real-time exercise monitoring through your camera
* Instant repetition counting with visual feedback
* Perfect for guided workout sessions

#### 🤖 Auto-Classification Engine

* Automatically identifies exercises as you perform them
* Intelligent rep counting for recognized movements
* Supports multiple exercise types simultaneously

#### 💬 AI Fitness Mentor

* Powered by OpenAI's advanced language model
* Provides personalized fitness guidance and tips
* Answers workout-related questions intelligently

---

## 🧠 Technical Deep Dive

### 🏃‍♂️ Exercise Recognition System

Our classification engine leverages multiple high-quality datasets:

* **Real-World Data**: Kaggle Workout Dataset
* **Synthetic Training**: InfiniteRep Dataset
* **Diverse Variations**: Additional online sources

The system uses LSTM and BiLSTM architectures to process body landmarks and classify exercises using joint angles and movement patterns—optimized for accuracy, precision, recall, and F1-score.

---

### 🔢 Repetition Counting Algorithm

#### Manual Mode

* User selects specific exercise type
* Angle-based threshold detection for rep counting
* Customizable sensitivity settings

#### Automatic Mode

* BiLSTM model performs real-time classification
* Dynamic counting logic adapts to movement
* Tracks complete "up" and "down" motion cycles

---

### 🤖 Intelligent Chatbot System

* Built with **OpenAI GPT-3.5-turbo**
* Integrated via **LangChain** for context retention
* Provides real-time guidance with a professional disclaimer

---

## 💻 Technology Stack

| Component        | Technology                             |
| ---------------- | -------------------------------------- |
| Pose Detection   | MediaPipe for body landmark extraction |
| Machine Learning | LSTM & BiLSTM networks                 |
| Web Framework    | Streamlit                              |
| Computer Vision  | OpenCV                                 |
| AI Assistant     | OpenAI GPT via LangChain               |

---

## ⚠️ Important Notes

### 🔧 Current Model Configuration

* Deployed model is the **"BiLSTM Invariant"** version
* Uses normalized angles/distances (no raw x, y, z)
* Optimized in `train_bidirectionallstm.py`

### 📹 Video Content Notice

* Includes `shoulder_press_form.mp4`
* Additional videos require separate download
* Full library available in complete repo

---

## 🤝 Connect & Contribute

### 📧 Contact Information

* Email: [i.rajaryann@gmail.com](mailto:i.rajaryann@gmail.com)
* GitHub: [yesaryann](https://github.com/yesaryann)

---

## 🌟 Show Your Support

If this project helped improve your fitness journey, please consider giving it a ⭐ on GitHub!

---

## 📜 License

This project is open-source and available under the **MIT License**.

---

## 🔮 Future Enhancements

* Additional exercise types and variations
* Advanced form correction algorithms
* Mobile app development
* Integration with fitness wearables
* Social features and progress sharing

---

**Transform your fitness routine with ZyntraFit – where AI meets fitness! 💪**

