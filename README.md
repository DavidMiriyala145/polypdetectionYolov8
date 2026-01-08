# 🩺 YOLOv8 Polyp Detection

![Model](https://img.shields.io/badge/Model-YOLOv8-blue)
![Framework](https://img.shields.io/badge/Framework-Ultralytics-black)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)
![Dataset](https://img.shields.io/badge/Dataset-Roboflow-orange)
![Notebook](https://img.shields.io/badge/Environment-Jupyter-informational)
![License](https://img.shields.io/badge/License-Ultralytics-green)

Automatic **polyp detection from endoscopic images** using **YOLOv8**, trained on a **Roboflow Polyp Detection dataset**.
The complete pipeline—dataset loading, training, evaluation, and inference—is implemented in a Jupyter Notebook.

---

## 📌 Overview

Polyp detection plays a vital role in early colorectal cancer prevention.
This project applies **YOLOv8**, a fast and accurate object detection model by **Ultralytics**, to identify polyps in medical images.

### ✨ Highlights

* YOLOv8 object detection
* Transfer learning with pretrained weights
* Roboflow-hosted annotated dataset
* End-to-end notebook-based workflow

---

## 🧠 Model Details

* **Architecture:** YOLOv8
* **Framework:** Ultralytics (PyTorch-based)
* **Task:** Object Detection
* **Classes:** Polyp (single class)

---

## 📦 Dataset

**Polyp Detection Dataset – Roboflow**

🔗 **Dataset & Model Link**
[https://app.roboflow.com/polyp-e78ji/polyp_detection-k9te7/models](https://app.roboflow.com/polyp-e78ji/polyp_detection-k9te7/models)

### Dataset Features

* Annotated colonoscopy images
* Bounding-box labels
* Exported in YOLOv8 format
* Train / Validation / Test splits

### Dataset Structure

```
dataset/
├── train/
│   ├── images/
│   └── labels/
├── valid/
│   ├── images/
│   └── labels/
└── test/
    ├── images/
    └── labels/
```

---

## 📂 Project Structure

```
.
├── Copy_of_polypdetectionYolov8.ipynb   # Main YOLOv8 notebook
├── dataset/                             # Roboflow dataset
├── runs/                                # Training & inference outputs
├── weights/                             # Saved model weights
└── README.md                            # Documentation
```

---

## ⚙️ Requirements

* Python 3.8+
* PyTorch
* Ultralytics YOLOv8
* OpenCV
* NumPy
* Matplotlib
* Jupyter Notebook

### Install Dependencies

```bash
pip install ultralytics opencv-python numpy matplotlib
```

---

## 🚀 Usage

1. Launch the notebook:

   ```bash
   jupyter notebook Copy_of_polypdetectionYolov8.ipynb
   ```
2. Download the dataset from Roboflow in **YOLOv8 format**.
3. Update dataset paths if required.
4. Run cells sequentially to:

   * Train the YOLOv8 model
   * Evaluate performance
   * Run inference and visualize predictions

---

## 📊 Training & Evaluation

YOLOv8 automatically generates:

* Loss curves
* Precision, Recall, mAP metrics
* Best model checkpoints

Saved under:

```
runs/train/
```

---

## 🔍 Inference

* Bounding boxes around detected polyps
* Confidence scores per detection
* Outputs saved to:

```
runs/detect/
```

---

## 🧪 Applications

* Medical image analysis
* Colonoscopy screening assistance
* Healthcare AI research
* Performance comparison with YOLOv5 / Faster R-CNN

---

## ⚠️ Disclaimer

🚨 **For research and educational use only**
This project is **not approved for clinical or diagnostic use**.

---

## 📜 License

* **YOLOv8:** Ultralytics License
* **Dataset:** Roboflow Dataset License

Please review respective platforms for licensing details.

---

## 🙌 Acknowledgements

* **Roboflow Polyp Detection Dataset**
* **Ultralytics YOLOv8**
* Open-source medical imaging community

---

## ⭐ Support

If this project helped you, please consider **starring the repository** ⭐
Contributions and suggestions are welcome!
