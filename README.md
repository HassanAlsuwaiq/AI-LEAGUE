#Digital Twin for Stadium Crowd and Parking Detection

This repository contains models and data for **Crowd Detection** and **Parking Space Detection** systems for stadiums and sporting events. The goal is to enhance crowd flow management and optimize parking space usage.

## Models Overview
1. **Crowd Detection Model (YOLOv8)**:  
   - Detects crowd density and analyzes crowd flow in stadiums.
   - Provides real-time detection of crowd sizes, areas of congestion, and potential safety hazards.

2. **Parking Space Detection Model (YOLOv8)**:  
   - Detects vacant and occupied parking spaces in real-time.
   - Helps in guiding visitors to empty parking spots quickly, reducing traffic congestion.

## Data Sources
- **Crowd Detection**:  
  - 70% training data (2355 images), 15% validation data (506 images), 15% test data (504 images).
  - Data gathered from various sources like **Kaggle**, **Roboflow**, and **GitHub**.

- **Parking Space Detection**:  
  - 70% training data (2339 images), 15% validation data (558 images), 15% test data (226 images).
  - Also sourced from **Kaggle**, **Roboflow**, and **GitHub**.

## Dependencies
- **YOLOv8**: Object detection model used for both crowd and parking space detection.
- **Roboflow**: Platform for dataset management and model versioning.
- **OpenCV**: Computer vision library for image processing.
- **PyTorch**: Deep learning framework used for training the models.

Install required dependencies:
```bash
pip install -r requirements.txt
