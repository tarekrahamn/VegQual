# 🥦 VegQual: A Quality-Based Vegetable Image Dataset for Defect Detection Using YOLO Models  

[![Paper](https://img.shields.io/badge/Paper-Link-blue?style=flat-square)](#)
[![Dataset](https://img.shields.io/badge/Dataset-Download-green?style=flat-square)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 🌱 Overview  
**VegQual** is a specialized dataset designed to support defect detection and quality classification of vegetables using state-of-the-art **YOLO models (v9 & v11)**.  
It includes *fresh* and *defected* samples across 7 vegetable types, collected under controlled conditions to ensure data consistency and realism.

---

## 📊 Dataset Summary  

| Vegetable Name | Defected Images | Fresh Images |
|----------------|----------------:|--------------:|
| Tomato | 190 | 167 |
| Potato | 105 | 442 |
| Bitter Gourd | 629 | 413 |
| Pointed Gourd | 256 | 175 |
| Onion | 518 | 245 |
| Capsicum | 295 | 569 |
| Brinjal | 393 | 339 |
| **Total** | **2,386** | **2,350** |

> **Total Images:** 4,736  
> **Number of Classes:** 7  
> **Annotations:** YOLO format (bounding boxes)

---

## ⚙️ Model Performance  

| Model | Precision (%) | Recall (%) | PR (%) | F1-score (%) | mAP@50 (%) |
|:------|---------------:|------------:|--------:|--------------:|------------:|
| YOLOv9  | 89.4 | 92.6 | 94.3 | 90.8 | 94.3 |
| YOLOv11 | 89.8 | 89.2 | 93.9 | 89.4 | 93.9 |

---

## 🧠 Methodology  

1. **Image Acquisition:** Captured using various smartphone cameras under daylight and indoor light.  
2. **Annotation:** Bounding boxes labeled manually following the YOLO format.  
3. **Model Training:** YOLOv9 and YOLOv11 trained on the dataset for comparative analysis.  
4. **Evaluation:** Assessed using Precision, Recall, F1-score, and mAP@50 metrics.

---

## 🧩 Contribution  


---

## 💻 How to Use  

```bash
# Clone this repository
git clone https://github.com/yourusername/VegQual.git

# Navigate into the directory
cd VegQual

# Install dependencies
pip install -r requirements.txt

# Train YOLO model
python train.py --data vegqual.yaml --weights yolov9.pt

# Evaluate the model
python test.py --weights runs/train/weights/best.pt --data vegqual.yaml
