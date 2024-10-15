# SOTA Segmentation Using BASNet

## 🔍 Project Overview

This project focuses on improving **state-of-the-art (SOTA)** segmentation models for **dichotomous image annotation** using **BASNet** (Boundary-Aware Salient Object Detection Network). The main objective is to enhance segmentation accuracy, particularly for objects with complex boundaries.

### 📝 Problem Statement

Existing segmentation models often focus on specific object characteristics (e.g., salient, camouflaged, or meticulous), and they are typically dataset-dependent. This project aims to create a **category-agnostic dichotomous image segmentation (DIS)** task for accurately segmenting objects of various complexities.

### Key Features:
- **Model**: BASNet (Boundary-Aware Salient Object Detection Network)
- **Objective**: Improve segmentation accuracy for binary image segmentation tasks.
- **Dataset**: 🖼️ DUTS Saliency Detection Dataset (DUTS-TR) with 10,553 images.
- **Key Enhancements**:
  - ⚙️ Adaptive learning rate scheduling.
  - 📈 Advanced loss functions (Dice, Focal loss).
  - 🔍 Multi-scale attention mechanisms.
  - ✂️ Integration of contour maps using edge detection techniques (e.g., Canny/Sobel).
  - 🌀 Atrous Spatial Pyramid Pooling (ASPP) for multi-scale context capture.

---

## 🛠️ Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.ecodesamsung.com/22i363/BASNET-MODEL-FOR-SOTA-SEGMENTATION.git

2. **Navigate to the project directory:**

  ```bash
  cd BASNET-MODEL-FOR-SOTA-SEGMENTATION

3. **Navigate to the project directory:**
    ```bash
    pip install -r requirements.txt

##🗂️ Dataset
##📊 DUTS-TR Dataset:
The dataset used is from the DUTS Saliency Detection benchmark, containing 10,553 training images with binary masks. You can download the dataset from Kaggle or use the pre-processed dataset available in the GitHub repository.

##🔄 Preprocessing Steps:
- Resizing and normalizing images.
- Applying histogram equalization for contrast enhancement.
Contour maps generated using Canny/Sobel edge detection.

##🧠 Model Architecture
##🖼️ BASNet Overview:
- *Encoder:* Deep residual networks (ResNet) for feature extraction.
- *Decoder:* U-Net style decoder to reconstruct segmentation masks.
-**Attention Mechanisms:** Multi-scale attention modules for enhanced feature extraction.
-**ASPP (Atrous Spatial Pyramid Pooling):** Captures multi-scale context to improve segmentation performance.
  - 🔧 Improvements Implemented:
  - ⚙️ Adaptive learning rate scheduling.
  - 🔍 Multi-scale attention modules.
- 📈 Custom loss functions (Dice, Focal loss).
- ✂️ Contour integration using edge detection.

##🏅 Results
- Accuracy: The BASNet model achieved an accuracy of 94.76% on the DUTS-TR dataset.
Observations:
✂️ Improved boundary detection using contour maps.
🔍 Multi-scale attention mechanisms significantly improved segmentation in complex regions.
🚀 Usage
1. Training the Model:
Use the following command to train the model:

bash
Copy code
python train.py --dataset ./data/DUTS --epochs 50 --batch_size 16
2. Testing the Model:
To test the model on the DUTS-TE test set:

bash
Copy code
python test.py --dataset ./data/DUTS --checkpoint ./checkpoints/basnet_model.pth
👥 Authors
Sengathir Soorian E T
Kavin T.
Vishal K.
Professor: Dr. R. Rekha (rra.it@psgtech.ac.in)
📄 License
This project is licensed under the MIT License - see the LICENSE file for details
