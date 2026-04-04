
# Team Number – Project Title

## Team Info
- 22471A0530 — **Asritha khajjayam** ( [LinkedIn](https://www.linkedin.com/in/asritha-khajjayam-a500322b1?utm_source=share_via&utm_content=profile&utm_medium=member_android) )
_Work Done: backend_

- 22471A0563 — **Uma Bhavani Bukya** ( [LinkedIn](https://www.linkedin.com/in/bhukya-uma-bhavani-8005b1327) )
_Work Done: documents and all ppts_

- 22471A0568 — **Nandini yendati** ( [LinkedIn](https://www.linkedin.com/in/yendeti-nandini-704b63347) )
_Work Done: Frontend_

---

## Abstract
Object detection in remote sensing imagery is particularly challenging due to arbitrary object orientations, large
scale variations, and dense scene layouts. This work presents
EdgeYOLO-RS, a lightweight detection framework specifically
designed for aerial imagery. Based on the YOLOv8-OBB architecture, the proposed model leverages oriented bounding box
regression to accurately localize rotated objects such as ships,
vehicles, and infrastructure components. The system is trained
on the DOTA v2.0 dataset using a customized preprocessing
pipeline that includes label normalization, image enhancement,
and uniform resolution scaling. The training process employs
1024×1024 contrast-enhanced images and is optimized for efficient deployment on edge devices. Experimental results demonstrate that EdgeYOLO-RS delivers reliable performance in realworld scenarios such as UAV monitoring, disaster response, and
geospatial mapping. The framework also establishes a foundation
for future enhancements involving attention mechanisms and
video-based remote sensing analysis.
Index Terms—Remote Sensing, Oriented Object Detection,
YOLOv8-OBB, DOTA v2.0, Aerial Imagery, Deep Learning, Edge
Computing, Rotation-Invariant Detection, Lightweight Model,
Real-Time Detection

---

## Paper Reference (Inspiration)
👉 **[Paper Title CSPPartial-YOLO: A Lightweight YOLO-Based
Method for Typical Objects Detection in
Remote Sensing Images
  – Author NamesSiyu Xie , Mei Zhou , Chunle Wang , and Shisheng Huang
 ]([Paper URL here](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7827088))**
Original conference/IEEE paper used as inspiration for the model.

---

## Our Improvement Over Existing Paper
Our work improves upon existing methods by adopting a more efficient and practical approach for aerial object detection. Instead of using complex custom modules, we utilize a YOLOv8-based oriented bounding box model, which simplifies the architecture while maintaining strong performance.

We enhance rotation-aware detection, improve small object visibility through preprocessing, and ensure real-time performance on edge devices with a lightweight design. Overall, our approach focuses on achieving a better balance between accuracy, speed, and deployment simplicity.
---

## About the Project
What the project does:
This project develops a lightweight object detection system that identifies and localizes objects in aerial images using rotated bounding boxes. It can detect objects like vehicles, ships, and infrastructure even when they appear at different angles.

Why it is useful:
It is useful for real-world applications such as surveillance, disaster management, traffic monitoring, and environmental analysis, where aerial images contain complex scenes with objects in various orientations.

General workflow:
Input → Aerial images
Processing → Image resizing, enhancement, and label preparation
Model → YOLO-based rotation-aware detection model
Output → Detected objects with oriented bounding boxes and class labels

---

## Dataset Used
👉 **[The dataset used in this project is the DOTA v2.0]([Dataset URL](https://www.kaggle.com/datasets/chandlertimm/dota-data/data
))**

**Dataset Details:**
The dataset consists of high-resolution aerial images containing multiple object categories such as vehicles, ships, and buildings.
It includes oriented bounding box (OBB) annotations, allowing accurate detection of objects at different angles.

The images are processed to a fixed size (e.g., 1024×1024) for uniform training.
The dataset is divided into training, validation, and testing sets to evaluate model performance effectively.

---

## Dependencies Used
The project uses the following main dependencies:

Python – Programming language for implementation
PyTorch – Deep learning framework for model training
Ultralytics YOLOv8 – Object detection model and training API
OpenCV – Image and video processing
NumPy – Numerical computations
Matplotlib – Visualization of results and graphs

These tools help in data processing, model training, and result visualization.

---

## EDA & Preprocessing
EDA (Exploratory Data Analysis):
Basic analysis was performed to understand image distribution, object classes, and annotation quality. Sample images were visualized with bounding boxes to verify correctness.

Preprocessing:
Images were resized to a uniform size (1024×1024).
Contrast enhancement and sharpening were applied to improve visibility of small objects.
Invalid or missing annotations were removed, and labels were normalized to ensure consistency for training.

---

## Model Training Info
The model was trained using a YOLOv8-based architecture on aerial image data.
Training was performed for a fixed number of epochs with a defined batch size and image resolution (1024×1024).

An SGD optimizer was used, and performance metrics such as precision, recall, and mAP were monitored during training.
Early stopping and validation checks were applied to prevent overfitting and ensure stable model performance.

---

## Model Testing / Evaluation
The trained model was evaluated on a separate test dataset to measure its performance.
Key metrics used include precision, recall, and mAP to assess detection accuracy.

The model was tested on both images and video frames, ensuring it can handle real-time scenarios.
Results showed effective detection of objects with correct orientation and good performance across different scales and conditions.

---

## Results
The model achieved high detection accuracy with strong precision and recall values.
It performed well in detecting rotated objects and handled complex aerial scenes effectively.

The system also maintained real-time performance with fast inference speed, making it suitable for practical applications.
Overall, the results demonstrate a good balance between accuracy, speed, and efficiency.

---

## Limitations & Future Work
Limitations:
The model may struggle with very small or densely packed objects.
Performance can be affected by low-quality or imbalanced data.
Some classes may have lower accuracy due to fewer training samples.

Future Work:
Improve detection of small objects using advanced augmentation and multi-scale training.
Incorporate attention mechanisms to enhance feature learning.
Extend the model for real-time video analytics and further optimize it for edge devices.

---

## Deployment Info
The model is designed for deployment on edge devices and GPU-based systems.
It can be integrated with applications using Python scripts or APIs for real-time detection.

The system supports image and video input, making it suitable for UAVs, surveillance systems, and monitoring applications.
Due to its lightweight design, it ensures fast inference and low resource usage during deployment.

---
