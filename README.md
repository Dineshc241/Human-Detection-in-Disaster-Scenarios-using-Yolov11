# Human Detection in Disaster Scenarios using YOLOv11

This project implements a robust human detection system for disaster scenarios using the YOLOv11 deep learning model. The project integrates advanced preprocessing techniques, including Bilateral Filtering and CLAHE, to enhance image quality and improve detection performance in noisy, low-light, and crowded environments.

## Project Overview

Disaster situations like floods, earthquakes, and fires pose challenges for detecting victims due to poor visibility, noise, and occlusion. Using the C2A dataset, this project trains the YOLOv11 model, leveraging preprocessing to tackle these challenges. The goal is to improve the accuracy and reliability of human detection, aiding efficient search and rescue operations.

## Methods

1. **Dataset**: The C2A dataset, consisting of synthetic images simulating disaster scenarios, is used for training and testing.
2. **Preprocessing**:
   - **Bilateral Filtering**: Reduces noise while preserving edges for clearer image details.
   - **CLAHE (Contrast Limited Adaptive Histogram Equalization)**: Enhances image contrast, particularly in low-light conditions.
3. **Model Development**:
   - **YOLOv11**: A cutting-edge object detection model with enhanced feature extraction and multi-scale representation capabilities.
   - **Training Parameters**: Models trained over 25 epochs with a batch size of 32 and an image size of 640x640.
4. **Evaluation Metrics**:
   - Precision, Recall, mAP@50, and mAP@50-95 are used to evaluate detection performance.

## Results

- **YOLOv11 with Preprocessing**:
  - Precision: 0.987
  - Recall: 0.989
  - mAP@50: 0.989
  - mAP@50-95: 0.989
- Preprocessing techniques significantly enhanced model performance in challenging environments.

## Libraries Used

- Python 3.8+
- TensorFlow
- PyTorch
- OpenCV
- NumPy
- Matplotlib
- Pandas
- Ultralytics YOLO

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Dineshc241/Human-Detection-in-Disaster-Scenarios-using-Yolov11.git
   cd Human-Detection-in-Disaster-Scenarios-using-Yolov11
```

2. Install Dependencies:
```bash
pip install -r requirements.txt

```

3. Download the dataset:

The project utilizes the [C2A Dataset](https://www.kaggle.com/datasets/rgbnihal/c2a-dataset), which provides synthetic images tailored for disaster scenarios. It includes various challenging conditions such as low visibility, noise, and cluttered environments. Download the dataset from Kaggle and place it in the `dataset` directory.
 