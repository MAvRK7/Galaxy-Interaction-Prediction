# 🌌 Explainable Galaxy Interaction Prediction with Novel Hybrid Attention Mechanisms

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)]()
[![Framework](https://img.shields.io/badge/Framework-PyTorch%20%7C%20TensorFlow-orange)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)]()

---

## 📌 Overview
This repository presents a **novel attentive neural ensemble** for predicting galaxy interactions using the **Galaxy Zoo DESI** dataset from the **DESI Legacy Imaging Surveys**.

The model integrates **three complementary architectures**:
- **Attention‑Guided Explainable Capsules (AG‑XCaps)**
- **Hybrid Self‑Attention Neural Network (H‑SNN)**
- **ResNet with GRU layers**

The ensemble is designed for **high accuracy**, **interpretability**, and **scalability** in large‑scale astronomical surveys.

---

## 🛰 Dataset
- **Source**: [Galaxy Zoo DESI](https://www.zooniverse.org/projects/zookeeper/galaxy-zoo/) from the DESI Legacy Imaging Surveys  
- **Content**: Morphological classifications of galaxies, including interaction labels  
- **Preprocessing**:
  - Image resizing and normalization
  - Data augmentation (rotation, flipping, scaling) to improve generalization
  - Stratified train/validation/test split to preserve class balance

---

## 🧪 Methodology

### **1. Attention‑Guided Explainable Capsules (AG‑XCaps)**
- Capsule network backbone with **attention gates** to focus on salient morphological regions
- Integrated with **LIME** for local interpretability of predictions

### **2. Hybrid Self‑Attention Neural Network (H‑SNN)**
- Combines convolutional feature extraction with **multi‑head self‑attention**
- Captures both local texture and global structural dependencies

### **3. ResNet + GRU**
- **ResNet** backbone for deep spatial feature extraction
- **GRU layers** to model sequential dependencies in multi‑view or multi‑band data

**Ensemble Strategy**:
- Soft‑voting across model outputs
- Confidence‑weighted aggregation to reduce false positives

---

## 📊 Key Results

| Metric        | Ensemble Model | Random Forest Baseline |
|---------------|---------------:|-----------------------:|
| **Accuracy**  | **96%**        | 88%                    |
| **Precision** | **0.95**       | 0.87                   |
| **Recall**    | **1.00**       | 0.92                   |
| **F1‑Score**  | **0.97**       | 0.89                   |
| **False Positives** | **23**  | 70                     |

**Highlights**:
- **Perfect recall** ensures no interacting galaxies are missed
- **~67% reduction** in false positives compared to baseline
- Model size: **0.45 MB** — lightweight for deployment in large surveys

---

## 🔍 Explainability
- **LIME** applied to individual predictions to highlight morphological regions influencing classification
- Attention maps from AG‑XCaps and H‑SNN provide **visual interpretability**
- Enables astronomers to **validate model reasoning** against domain knowledge

---

## 🚀 Key Takeaways
- Hybrid attention mechanisms + capsule networks yield **state‑of‑the‑art performance** in galaxy interaction prediction
- Lightweight architecture enables **scalable inference** for upcoming surveys like **Euclid** and **LSST**
- Explainability tools ensure **trust and transparency** in scientific AI applications

---

## 📂 Repository Structure
- `Galaxy_Morphology_main.ipynb` — Full training & evaluation pipeline  
- `data/` — Preprocessing scripts for Galaxy Zoo DESI dataset  
- `figures/` — Attention maps, LIME explanations, and performance plots

---

## 💡 Skills Demonstrated
- Advanced deep learning architectures (Capsule Networks, Self‑Attention, ResNet, GRU)
- Explainable AI (LIME, attention visualization)
- Ensemble learning for robust classification
- Astronomical image preprocessing & augmentation
- Performance benchmarking against classical ML baselines

---

## 📈 Potential Applications
- Automated morphological classification in large‑scale surveys
- Early detection of interacting galaxies for follow‑up studies
- Transferable to other astrophysical image classification tasks

---

## 🛠 Installation

**Prerequisites**:
- Python 3.9+
- PyTorch, TensorFlow

--- 

## 🤝 Contributing
Contributions are welcome! Please open an issue or submit a pull request.

---

## 🙏 Acknowledgments
Galaxy Zoo

DESI Legacy Imaging Surveys

LIME for explainable AI

---
## 📐 Model Architecture Diagrams

- 1️⃣ Attention‑Guided Explainable Capsules (AG‑XCaps)

<img width="338" height="504" alt="image" src="https://github.com/user-attachments/assets/6f68eec1-8380-4c55-9353-3f6f9ff7800e" />


- 2️⃣ Hybrid Self‑Attention Neural Network (H‑SNN)

  <img width="338" height="504" alt="image" src="https://github.com/user-attachments/assets/9740609a-513a-4097-a977-435dec0e1f7b" />


-3️⃣ ResNet + GRU

<img width="338" height="504" alt="image" src="https://github.com/user-attachments/assets/7e311038-5cc0-4ddf-a0ae-11c7fbeea7f7" />


- 4️⃣ Ensemble Integration

<img width="796" height="379" alt="image" src="https://github.com/user-attachments/assets/1b5a1800-874f-402a-a891-d3f8913db7c8" />


---

**Required Libraries**:
```bash
pip install numpy pandas scikit-learn lime matplotlib
