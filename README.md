# Transfer-Learning-for-Predicting-Germination-Rates-in-Botrytis-cinerea-Grey-Mold-Disease-

This repository provides code and pretrained models for predicting germination rates of *Botrytis cinerea* using deep learning techniques, including transfer learning and object detection with YOLOv11.

## 📂 Repository Structure
├── Train/ # Scripts and configurations for training
│ └── YOLO.ipynb
├── Test/ # Scripts and configurations for training
│ │── Germinación/ # Jupyter Notebooks for inference and detection
│ │	├── Inferencia.ipynb # Inference pipeline on test samples
│ │	└── Detection.ipynb # Visualization and object detection
│ └── Models/ # Pretrained models
│       └── YOLOv11.pt # Trained YOLOv11 mode


---

## 🔍 YOLOv11 Architecture

The following figure shows the high-level architecture of YOLOv11 used in this study:

![YOLOv11 Architecture](Images/YOLOv11_2000.png)

YOLOv11 combines high-resolution feature extraction with efficient prediction heads, making it ideal for detecting small fungal structures like conidia.

---

## 🧪 Inference Workflow

To run the detection over test images, use the notebooks provided in the `Germinación/` folder:

1. **Detection.ipynb** – runs YOLOv11 on input images and outputs bounding boxes.
2. **Inferencia.ipynb** – visualizes detection results and computes statistics.

Example of a detection result:

![Detection Example](Images/Test_detection.png)

---

## 🧪 Requirements

- Python ≥ 3.8
- PyTorch ≥ 2.0
- OpenCV
- Jupyter Notebook
- Other dependencies listed in `requirements.txt` (if available)



