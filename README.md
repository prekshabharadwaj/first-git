# Construction Site Safety PPE Detection System

## 🏗️ Overview
Real-time computer vision system for detecting Personal Protective Equipment (PPE) compliance on construction sites using YOLOv8.

## 🎯 Problem Statement
Construction sites face 60,000+ fatal accidents annually, with 30-40% linked to PPE non-compliance. This system automatically detects workers without helmets or safety vests in real-time.

## 📊 Dataset
- **Source**: Roboflow Construction Safety Dataset
- **Classes**: helmet, no-helmet, vest, no-vest, person
- **Images**: 1,116 total (997 train, 119 val)

## 🚀 Model Architecture
- **Framework**: YOLOv8 (You Only Look Once)
- **Backbone**: CSPDarknet53
- **Input Size**: 640×640
- **Loss**: CIoU + BCE + DFL

## 📈 Results
| Metric | Value |
|--------|-------|
| mAP50 | 87.3% |
| mAP50-95 | 62.1% |
| Precision | 85.6% |
| Recall | 83.2% |
| FPS (T4 GPU) | 30+ |

## 🔧 Setup & Usage

### Run in Colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/YOUR_NOTEBOOK_ID)

### Local Setup
```bash
git clone https://github.com/YOUR_USERNAME/Construction-Safety-PPE-Detection.git
cd Construction-Safety-PPE-Detection
pip install -r requirements.txt
jupyter notebook construction_safety_ppe.ipynb
