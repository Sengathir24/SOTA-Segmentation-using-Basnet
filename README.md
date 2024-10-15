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

