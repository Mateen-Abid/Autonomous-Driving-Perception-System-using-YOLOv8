# 🚗 Autonomous Driving Perception System using YOLOv8

This project is a deep learning-based perception system designed for autonomous driving using the YOLOv8 object detection model. It leverages the KITTI dataset to detect and localize key objects like cars, pedestrians, and cyclists, providing foundational work for self-driving applications.

## 📌 Project Overview

The system uses the state-of-the-art YOLOv8 (You Only Look Once version 8) model to identify and track objects in real-time environments. The core idea is to build a reliable, efficient, and accurate object detection pipeline that can be further expanded for complete autonomous vehicle vision systems.

## 📂 Features

- 🚀 Fast and accurate object detection
- 🧠 YOLOv8 model trained on KITTI dataset
- 👁️ Detection of vehicles, pedestrians, and cyclists
- 🔍 High performance in daylight and occluded scenarios
- 📊 Evaluation using standard performance metrics (mAP, precision, recall)

## 📁 Dataset

- **Dataset**: KITTI Vision Benchmark Suite
- **Classes Detected**: Car, Pedestrian, Cyclist
- [KITTI Website](http://www.cvlibs.net/datasets/kitti/)

## 🛠️ Installation

Clone the repository and install dependencies:
git clone https://github.com/yourusername/driving-perceptron.git
cd driving-perceptron
pip install -r requirements.txt
▶️ Usage
To train the model:
python train.py --data data.yaml --epochs 100 --img 640 --batch 16 --weights yolov8n.pt
To test on an image or video:

python detect.py --source path/to/image_or_video --weights best.pt
📈 Results
Metric	Value
mAP@0.5	0.86
Precision	0.88
Recall	0.84

Visual output examples are available in the results/ folder.

🧪 Evaluation
Conducted evaluation using precision, recall, and mAP.

Model shows strong performance for high-frequency object classes.

Minor performance dips observed in cases of occlusion or small objects.

🌱 Future Work
Integrate LiDAR and radar data for sensor fusion

Improve performance in low-light and crowded scenarios

Extend detection to more object classes and road signs

Develop real-time video stream inference system

🤝 Contributing
Pull requests and feedback are welcome! Please make sure to update tests as appropriate.

🛡️ License
This project is licensed under the MIT License - see the LICENSE file for details.
