# 🥦 VegQual: A Quality-Based Vegetable Image Dataset for Defect Detection Using YOLO Models  

[![Paper](https://img.shields.io/badge/Paper-Link-blue?style=flat-square)](#)
[![Dataset](https://img.shields.io/badge/Dataset-Download-green?style=flat-square)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 🌱 Overview  

**VegQual** is a specialized multiclass image dataset designed for **real-time classification and defect detection of vegetables**.  
The dataset contains images of both **fresh** and **defective** vegetables across **seven classes**, collected under diverse environmental and lighting conditions to ensure robustness and generalization.

This dataset supports computer vision research focused on:
- Quality assessment of agricultural produce  
- Real-time defect detection systems  
- Training and evaluation of **YOLO-based object detection models**  

Each image in VegQual is annotated using the **YOLO format**, with bounding boxes that clearly identify the fresh or defected portions of vegetables.  
The dataset aims to assist researchers, students, and practitioners in developing AI-driven solutions for improving agricultural quality inspection and reducing food waste.

---

### 🧩 Key Highlights
- **7 vegetable and 14 classes:** Tomato, Potato, Bitter Gourd, Pointed Gourd, Onion, Capsicum, and Brinjal  
- **4,736 annotated images** (2,386 defected + 2,350 fresh samples)  
- **High-quality annotations** in YOLO format  
- **Benchmark results** available for **YOLOv9** and **YOLOv11**  
- Ideal for **machine learning, agriculture automation, and quality inspection systems**


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
> **Number of Classes:** 14
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
**Authors:**  
Tarek Rahman¹, Md Rahadul Islam Jishan¹, Robiul Islam¹, Md Rakibul Islam¹, and Jannatul Tajrian¹  

**Supervisor:**  
Ohidujjaman¹*  

¹ Department of Computer Science and Engineering  
*Corresponding author and project supervisor*


---

## 💻 How to Use 


---

## 📬 Contact  

For any questions, collaborations, or dataset-related inquiries, please reach out to:  

**Tarek Rahman**  
📧 Email: [tarekrahamn01@gmail.com](mailto:tarekrahamn01@gmail.com)  
🔗 LinkedIn: [linkedin.com/in/tarekrahamn01](https:www.linkedin.com/in/tarek-rahmantr)  
🎓 Google Scholar: [scholar.google.com/citations?user=YOUR-SCHOLAR-ID](https://scholar.google.com/citations?user=n_PyeXwAAAAJ&hl=en)



---


## 📜 Citation  

If you use this dataset or code in your research, please cite:

```bibtex
@misc{rahman2025vegqual,
  author       = {Rahman, T. and Jishan, Md Rahadul Islam and Islam, Robiul and Islam, Md Rakibul and Tajrian, Jannatul},
  title        = {A Multiclass Dataset for Real-Time Fresh and Defective Vegetables},
  year         = {2025},
  month        = nov,
  publisher    = {Figshare},
  url          = {https://figshare.com/articles/dataset/_/30596084/0}
}



