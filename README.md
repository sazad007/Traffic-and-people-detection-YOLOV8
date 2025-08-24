# Traffic and people detection using YOLOV8

This repository demonstrates how to train and run inference for **traffic and people detection** using [YOLOv8](https://github.com/ultralytics/ultralytics).  
It includes scripts for both training on the [VisDrone dataset](https://www.kaggle.com/datasets/banuprasadb/visdrone-dataset) and performing predictions on video files.

---

## 📂 Repository Contents
- **`traffic_and_people_detection_training_yolov8.py`**  
  Script to train a YOLOv8 model on the VisDrone dataset.

- **`traffic_and_people_detection_predict_yolov8.py`**  
  Script to run inference on video files using the trained model.

- **`nyc-annotated.mp4`**  
  Example annotated video showing predictions in action.

---

## 🚦 Workflow
1. **Training**  
   - The training script uses the **VisDrone dataset** from Kaggle and fine-tunes a YOLOv8 model (`yolov8n.pt`).  
   - After training, the best weights are saved as `visdrone-yolov8.pt`.

2. **Prediction**  
   - The prediction script loads the trained weights and performs detection on input video (`nyc.mp4`).  
   - Results (bounding boxes for people, vehicles, etc.) are saved along with an annotated output video.

---

## 🎥 Example Result
Below is an example of the detection results on a video (`nyc-annotated.mp4`):

https://github.com/user-attachments/assets/d8c5e084-f42a-4389-8257-9313591eb4b1
---

## ⚙️ Key Features
- Fine-tuning YOLOv8 on the **VisDrone dataset**.
- Detection of **pedestrians, cars, buses, and other traffic objects**.
- Video inference with bounding box annotations.

---

## 📝 Notes
- The scripts are designed for **Google Colab** and use **Google Drive** for dataset and model storage.
- Modify paths in the scripts as needed if running locally.
- Dataset: [VisDrone on Kaggle](https://www.kaggle.com/datasets/banuprasadb/visdrone-dataset).


