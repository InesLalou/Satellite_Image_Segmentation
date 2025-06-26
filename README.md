# 🌍 **Satellite Image Segmentation with DynamicEarthNet**  

## **Project Overview**  
The goal of this project is to **reproduce semantic segmentation** on satellite images from the **DynamicEarthNet** dataset. Our approach includes:  

- **Building and exploring** the multi-spectral dataset.  
- **Applying advanced preprocessing** techniques.  
- **Designing a U-Net model** from scratch.  
- **Using a pre-trained U-Net model** for segmentation.  
- **Applying Data Augmentation** techniques to enhance training.  

Due to storage and computational constraints, we used only a small portion of the available data.

---

## **Dataset Overview**  

### **DynamicEarthNet: A Multi-Spectral Satellite Dataset**  
**DynamicEarthNet** is a collection of satellite images covering a **two-year period (January 2018 – December 2019)**. It provides:  

✔ **Daily coverage** of observed areas.  
✔ **Monthly annotations**, updated when changes are detected.  
✔ **4 spectral bands**: **Red (R), Green (G), Blue (B), and Near-Infrared (NIR)**.  
✔ **Advanced preprocessing** to remove artifacts (e.g., clouds).  

---

### 🌍 **Class Distribution & Annotations**  
The dataset includes **75 Areas of Interest (AOI)** across **six continents**. Each image is annotated into **seven land cover categories**:  

| **Class**                 | **Percentage** |
|---------------------------|--------------|
| **Impervious surfaces** | 7.1%        |
| **Agriculture**         | 10.3%       |
| **Forest / Vegetation** | 44.9%       |
| **Wetlands**           | 0.7%        |
| **Bare soil**          | 28.0%       |
| **Water**              | 8.0%        |
| **Snow and ice**       | 1.0%        |

📌 **The first annotated image** for each region serves as a **reference**, with annotations updated **monthly** based on detected changes.  

---

### 📊 **Labeled vs. Unlabeled Data**  
The dataset contains **54,750 satellite images**, of which **1,800 are labeled** with segmentation masks.  

A project by Lily Daganaud and Ines Lalou
