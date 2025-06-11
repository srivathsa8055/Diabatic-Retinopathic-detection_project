# Diabetic Retinopathy Detection using ConvNeXt-Tiny

An AI-driven deep learning project for early and automated detection of Diabetic Retinopathy (DR) from retinal fundus images using the ConvNeXt-Tiny architecture and FastAI framework.

## 📌 Overview

Diabetic Retinopathy (DR) is a complication of diabetes that can lead to blindness if not detected early. This project aims to build a scalable and non-invasive diagnostic tool to automatically classify the severity of DR from retinal images. The model classifies images into five stages: **No-DR, Mild, Moderate, Severe, and Proliferative DR**.

## 🚀 Key Features

- Utilizes **ConvNeXt-Tiny** CNN architecture for high-accuracy image classification.
- Achieved **85% validation accuracy** on a curated retinal fundus image dataset.
- Built using the **FastAI** library for efficient training and transfer learning.
- Supports **real-time inference (~20ms per image)**.
- Class-wise performance analysis and qualitative visualizations included.

## 🧠 Technologies Used

- Python 3.8+
- FastAI
- PyTorch
- OpenCV
- Matplotlib, Seaborn
- Jupyter Notebook

## 📂 Dataset

- Publicly available dataset of **6,148 labeled retinal fundus images**.
- Images were augmented (rotation, zoom, flipping) and normalized for training.
- Labels correspond to 5 DR severity classes.

## 🏗️ Project Structure

```
├── data/                   # Retinal fundus images
├── models/                 # Trained model checkpoints
├── notebooks/              # Training and evaluation notebooks
├── results/                # Predicted samples and metrics
├── dr_model.py             # ConvNeXt-Tiny model definition
├── train.py                # Training script using FastAI
├── infer.py                # Inference on new images
├── requirements.txt        # Python dependencies
└── README.md               # Project overview
```

## ⚙️ How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/diabetic-retinopathy-detection.git
   cd diabetic-retinopathy-detection
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Train the model**
   ```bash
   python train.py
   ```

4. **Run inference**
   ```bash
   python infer.py --image path_to_image.jpg
   ```

## 📊 Results

| Model          | Accuracy (%) |
|----------------|--------------|
| ResNet50       | 82           |
| ResNet101      | 83           |
| YOLOv8         | 77           |
| **ConvNeXt-Tiny** | **85**      |

- Visual results and training curves are available in the `results/` folder.

## 📈 Future Work

- Improve model generalization with more diverse datasets.
- Integrate Grad-CAM for explainable AI.
- Build a user-friendly web interface for clinical deployment.
- Enable integration with telemedicine platforms.

## 👨‍💻 Contributors

- Srivathsa A  
- P Sai Sudheer  
- Praneet Mane  
- Sandeep Kulkarni  
- Varun M K  

## 📜 License

This project is for educational and research purposes only. All rights reserved.
