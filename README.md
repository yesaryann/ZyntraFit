🏋️‍♂️ ZyntraFit - Smart Fitness Coach with Automated Movement Recognition & Rep Tracking
Welcome to ZyntraFit - the future of fitness! This innovative AI-driven platform combines cutting-edge Computer Vision, Advanced Pose Detection, and Deep Learning technologies to revolutionize your workout experience by providing intelligent repetition monitoring and real-time exercise analysis.
🚀 Live Demo
Experience ZyntraFit in action: Watch Demo Video
📊 Research Foundation
This application is built upon rigorous academic research:

Paper: "Real-Time Fitness Exercise Classification and Counting from Video Frames"
Dataset: Available at Kaggle - Real-Time Exercise Recognition Dataset
Research Link: ArXiv Paper

🎯 Key Features
🔥 Core Capabilities

Intelligent Exercise Detection: Automatically identifies workout movements in real-time
Precision Rep Counting: Tracks repetitions with exceptional accuracy
Live Webcam Integration: Train with instant feedback using your camera
Video Analysis Tools: Upload workout videos for comprehensive analysis
AI Fitness Assistant: Get personalized guidance through our smart chatbot

💡 What Makes It Special

Real-time pose estimation using state-of-the-art MediaPipe technology
BiLSTM neural networks for robust exercise classification
Angle-based movement analysis for precise repetition detection
User-friendly web interface powered by Streamlit
Comprehensive exercise library with form demonstrations

🛠️ Technical Architecture
📁 Project Organization
├── main.py                           # Streamlit application entry point
├── ExerciseAiTrainer.py             # Exercise-specific pose analysis engine
├── AiTrainer_utils.py               # Image processing and calculation utilities
├── PoseModule2.py                   # MediaPipe pose estimation handler
├── chatbot.py                       # OpenAI-powered fitness assistant
├── extract_features.py             # Video landmark and angle extraction
├── create_sequence_of_features.py  # Dataset generation with 30-frame sequences
├── train_bidirectionallstm.py      # BiLSTM model training pipeline
├── requirements.txt                 # Python dependencies
├── shoulder_press_form.mp4          # Exercise demonstration video
├── thesis_bidirectionallstm_label_encoder.pkl  # Pre-trained label encoder
├── thesis_bidirectionallstm_scaler.pkl         # Feature scaling model
└── final_forthesis_bidirectionallstm_and_encoders_exercise_classifier_model.h5  # Trained BiLSTM model
🚀 Quick Start Guide
📋 Prerequisites

Python 3.7 or higher
Virtual environment (recommended)
Webcam (for real-time features)

⚡ Installation Steps

Clone the Repository
bashgit clone https://github.com/yesaryann/ZyntraFit.git
cd ZyntraFit

Create Virtual Environment
bashpython -m venv fitness_env
source fitness_env/bin/activate  # Windows: fitness_env\Scripts\activate

Install Dependencies
bashpip install -r requirements.txt

Launch Application
bashstreamlit run main.py


🎮 Application Features
🎯 Navigation Menu
The intuitive sidebar provides access to four main modules:
📹 Video Analysis Suite

Upload workout recordings for detailed movement analysis
Automated rep counting based on pose estimation
Exercise form evaluation and feedback

🔴 Live Webcam Mode

Real-time exercise monitoring through your camera
Instant repetition counting with visual feedback
Perfect for guided workout sessions

🤖 Auto-Classification Engine

Automatically identifies exercises as you perform them
Intelligent rep counting for recognized movements
Supports multiple exercise types simultaneously

💬 AI Fitness Mentor

Powered by OpenAI's advanced language model
Provides personalized fitness guidance and tips
Answers workout-related questions intelligently

🧠 Technical Deep Dive
🏃‍♂️ Exercise Recognition System
Our classification engine leverages multiple high-quality datasets:

Real-World Data: Kaggle Workout Dataset with authentic exercise videos
Synthetic Training: InfiniteRep Dataset featuring avatar-based movements
Diverse Variations: Additional online sources for comprehensive coverage

The system employs advanced LSTM and BiLSTM architectures to process body landmarks and classify exercises using joint angles and movement patterns, optimized for accuracy, precision, recall, and F1-score metrics.
🔢 Repetition Counting Algorithm
Manual Mode

User selects specific exercise type
Angle-based threshold detection for rep counting
Customizable sensitivity settings

Automatic Mode

BiLSTM model performs real-time exercise classification
Dynamic counting logic adapts to identified movements
Tracks complete "up" and "down" motion cycles

🤖 Intelligent Chatbot System

Built with OpenAI's GPT-3.5-turbo for natural conversations
LangChain integration maintains conversation context
Provides fitness guidance with professional disclaimer

💻 Technology Stack
ComponentTechnologyPose DetectionMediaPipe for precise body landmark extractionMachine LearningLSTM & BiLSTM networks for exercise classificationWeb FrameworkStreamlit for responsive user interfaceComputer VisionOpenCV for advanced image processingAI AssistantOpenAI GPT integration via LangChain
⚠️ Important Notes
🔧 Current Model Configuration

The deployed model is the "BiLSTM Invariant" version
Uses normalized angles and distances (excludes raw x,y,z coordinates)
Peak performance model available in train_bidirectionallstm.py

📹 Video Content Notice

Currently includes shoulder_press_form.mp4 demonstration
Additional instructional videos require separate download
Full video library available in complete repository

🤝 Connect & Contribute
📧 Contact Information

Email: i.rajaryann@gmail.com
GitHub: yesaryann

🌟 Show Your Support
If this project helped improve your fitness journey, please consider giving it a star ⭐ on GitHub!
📜 License
This project is open-source and available under the MIT License.
🔮 Future Enhancements

Additional exercise types and variations
Advanced form correction algorithms
Mobile app development
Integration with fitness wearables
Social features and progress sharing


Transform your fitness routine with ZyntraFit - where AI meets fitness! 💪
