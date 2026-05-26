# DoorShield AI
AI-Powered Weapon Detection and Smart Home Security System

DoorShield AI is an intelligent home security system that uses the YOLOv5 object detection model to detect weapons such as guns and knives in real-time through live video feeds. Unlike traditional CCTV systems that only record footage, DoorShield AI provides proactive threat detection by identifying dangerous objects instantly and displaying alerts through a live monitoring interface.

Developed as part of the ICT304 AI System Design assignment, this project demonstrates the integration of deep learning, computer vision, and real-time video processing into a practical smart security solution.

## 📌 Features
🔍 Real-time weapon detection using YOLOv5
📹 Live webcam/video feed monitoring
🚨 Immediate visual alerts upon weapon detection
🖥️ User-friendly live dashboard interface
📊 Detection confidence score display
🧠 Transfer learning using pretrained YOLOv5 weights
⚡ Near real-time inference performance (~20–30 FPS)
## 🛠️ Technologies Used
Technology	Purpose
Python	Core programming language
YOLOv5	Object detection model
PyTorch	Deep learning framework
OpenCV	Video processing and webcam handling
Google Colab	Model training environment
Streamlit	Live dashboard/UI
GitHub	Version control
Trello	Project management
Google Drive	File sharing and collaboration
## 🧠 AI Model

The system uses YOLOv5s, a lightweight object detection model optimized for real-time performance.

Why YOLOv5?
Fast inference speed
Lightweight architecture
Strong object detection accuracy
Suitable for real-time surveillance systems
Detected Classes
Knife
Gun

## 📊 Model Performance
Metric	Result
Precision	~0.91
Recall	~0.87
mAP@0.5	~0.92
mAP@0.5:0.95	~0.70
Inference Speed	~20–30 FPS

The best-performing model configuration was:

--img 640 --batch 16 --epochs 50 --weights yolov5s.pt --patience 5
## 🧪 Testing Conducted
✅ Unit Testing
Bounding box accuracy
Frame preprocessing
Alert triggering system
✅ End-to-End Testing
Live webcam threat simulation
Positive and negative detection scenarios
✅ Perturbation Testing

Tested under:

Low lighting
Different camera angles
Background clutter
Partial weapon occlusion
✅ UI Testing
Real-time updates
Responsive live feed
Detection label visibility
## 📸 Sample Output
Weapon Detected
Red bounding box
Confidence score displayed
Real-time alert triggered
No Weapon Detected
No false alert
Stable live feed maintained
## 🚀 Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/your-username/doorshield-ai.git
cd doorshield-ai
2️⃣ Create a Virtual Environment

Using Anaconda:

conda create -n doorshield python=3.9
conda activate doorshield
3️⃣ Install Dependencies
pip install -r requirements.txt

Or manually install:

pip install torch torchvision opencv-python matplotlib streamlit ultralytics numpy pandas pillow
4️⃣ Run the Live Detection System
python webcam_detection.py

Or launch the Streamlit dashboard:

streamlit run streamlit_app.py
🧹 Dataset Preprocessing

The dataset underwent:

Random shuffling
Train/test/validation split
Label standardization
Data augmentation:
Rotation
Flipping
Brightness adjustment
Hue/saturation changes

These preprocessing steps improved class balance and detection robustness.

## 📈 Training Workflow
Collect YOLO-formatted weapon datasets
Preprocess and augment data
Train YOLOv5 using transfer learning
Evaluate model performance
Deploy into live detection pipeline
## ⚠️ Challenges Faced
Limited GPU resources in Google Colab
Dataset imbalance between guns and knives
Long training times
Runtime interruptions/timeouts
Difficulty implementing motion anomaly detection
## 🔮 Future Improvements
Upgrade to YOLOv8 or larger YOLO models
Improve detection under occlusion and clutter
Add motion anomaly detection
Mobile notifications and SMS alerts
Historical detection logs
Cloud deployment support
Enhanced UI/dashboard experience
## 👥 Team Members
Salwa Sanaullah Khan,
Syeda Zainab Fathimay,
Regina Wangsaputri Suroto
## 📚 References
YOLOv5 Documentation by Ultralytics
PyTorch Documentation
OpenCV Documentation
Research papers on AI-powered weapon detection and surveillance systems
## 📄 License

This project was developed for educational purposes as part of the ICT304 AI System Design module.

## ⭐ Acknowledgements

Special thanks to:

Our lecturer and project supervisor
Open-source contributors
Ultralytics YOLO community
Google Colab for GPU resources
