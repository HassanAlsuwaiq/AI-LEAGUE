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
How to Use
Training the Models
Clone the repository:

bash
Copy
Edit
git clone <your-repository-url>
Navigate to the project directory:

bash
Copy
Edit
cd <your-project-directory>
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Train the models using the provided scripts:

For crowd detection:

bash
Copy
Edit
python train_crowd_model.py
For parking space detection:

bash
Copy
Edit
python train_parking_model.py
Testing the Models
You can test the trained models using the following commands:

For crowd detection:

bash
Copy
Edit
python test_crowd_model.py --image <image-path>
For parking space detection:

bash
Copy
Edit
python test_parking_model.py --image <image-path>
Model Performance
Crowd Detection Model (YOLOv8):
Precision: 96.37%

Recall: 90.46%

mAP50: 96.73%

mAP50-95: 71.51%

Parking Space Detection Model (YOLOv8):
Precision (Empty Spaces): 94.1%

Precision (Occupied Spaces): 95.4%

mAP50: 97.3%

mAP50-95: 86.9%

Ethical Considerations
Privacy and Data Protection: All data collected from cameras will only be used for crowd and parking detection purposes, ensuring privacy is respected.

Transparency: Users will be informed about the usage of surveillance cameras in the system, and how their data will be handled securely.

Challenges and Future Work
Current Challenges:
3D Digital Twin: We have yet to create the 3D model of the stadium and integrate the detection models with the digital twin.

Real-time Integration: We are working on connecting the models with real-time surveillance cameras for live detection.

Future Work:
Develop the 3D Digital Twin Model: We will create a 3D model of the stadium to simulate crowd flow more accurately.

Real-Time Integration: Linking the models to live camera feeds for real-time crowd and parking space detection.
