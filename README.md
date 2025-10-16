# US-Loss: Integrating Uncertainty Estimation in the Loss Function of Image Segmentation

## 📌 Abstract
_Paste abstract here._

---

## ✨ Overview
US-Loss is a novel **uncertainty-aware segmentation loss function** designed to improve both:
- **Segmentation accuracy**
- **Epistemic uncertainty estimation**

Unlike traditional uncertainty methods (e.g., MC Dropout, Deep Ensembles), US-Loss:
✅ Does **not** require multiple forward passes  
✅ Does **not** modify model architecture  
✅ Provides uncertainty in a **single pass**  
✅ Improves interpretability and robustness  

---

## 🧠 Key Idea: What is US-Loss?
The core of US-Loss combines:
1. **Segmentation loss** (BCEWithLogits)
2. **Uncertainty loss** using:
   - Predictive entropy
   - Updated entropy (weighted by prediction error)

A **dynamic weighting schedule (λ)** balances accuracy and uncertainty during training, allowing the model to first learn segmentation and then focus on uncertainty calibration.

---

## ✅ Main Contributions
- ✅ Introduce **US-Loss**, a plug-and-play loss function  
- ✅ Integrates uncertainty estimation **directly into training**  
- ✅ Produces sharper, boundary-focused uncertainty maps  
- ✅ Outperforms Monte Carlo Dropout and Deep Ensembles  
- ✅ Requires only **one forward pass** (fast and efficient)  
- ✅ Robust to out-of-distribution (OOD) data  

---

## 🗂 Datasets Used

We evaluate US-Loss on two medical image segmentation datasets:

### 1️⃣ ISIC 2018 Skin Lesion Dataset
- **Task:** Melanoma skin lesion segmentation  
- **Dataset:** https://challenge.isic-archive.com/data/  
- **Reference Paper:** https://arxiv.org/abs/1902.03368

### 2️⃣ BUS Breast Ultrasound Dataset
- **Task:** Breast tumor segmentation  
- **Dataset:** https://www.kaggle.com/datasets/aryashah2k/breast-ultrasound-images-dataset  
- **Reference Paper:** https://doi.org/10.1016/j.dib.2019.104863


## 📦 Repository Structure (to be added)
