# 🧠 Brain Tumor Segmentation (U-Net)

This repository contains a **U-Net based semantic segmentation system** designed to identify and segment brain tumors from **MRI (Magnetic Resonance Imaging)** scans.
The model leverages the U-Net architecture to produce precise pixel-wise masks, distinguishing between healthy brain tissue and tumor regions.

> **⚠️ Important:**
> This repository focuses on the deep learning model and training pipeline. The medical dataset is expected to be mounted or downloaded separately during runtime.

## 📌 Features

- **Medical Image Analysis**: Specialized preprocessing for MRI scans (normalization, resizing).
- **High-Precision Segmentation**: U-Net architecture optimized for biomedical image segmentation.
- **Tumor Localization**: accurately identifies tumor boundaries for clinical support.
- **Visualizations**: Displays side-by-side comparisons of Input MRI, Ground Truth Mask, and Model Prediction.
- **Framework**: Built using **TensorFlow/Keras**.

## 🧠 Model Architecture

### **U-Net**
The model follows the standard U-Net Encoder-Decoder design:
- **Contracting Path (Encoder)**: Extracts deep features and context from the MRI images.
- **Expanding Path (Decoder)**: Upsamples features to generate a high-resolution segmentation mask.
- **Skip Connections**: Bridge the encoder and decoder to retain fine-grained spatial details essential for accurate tumor boundaries.

## 📂 Repository Structure

```
.
├── UNet_Training.ipynb   # Main notebook for training the U-Net on MRI data
└── README.md             # Project documentation
```

## 📊 Dataset

**Target Dataset**: Brain Tumor MRI Dataset (e.g., Brats or similar public datasets).
- **Inputs**: 2D or 3D MRI scans (FLAIR, T1, T2 modalities).
- **Annotations**: Binary or Multi-class masks indicating tumor sub-regions (Edema, Core, Enhancing Tumor).

## ⚙️ Installation & Usage

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/Azmy36/UNet_Tumor.git
    cd UNet_Tumor
    ```

2.  **Install dependencies**:
    ```bash
    pip install tensorflow numpy matplotlib opencv-python
    ```

3.  **Run the Notebook**:
    Open `UNet_Training.ipynb` in **Jupyter Notebook** or **Google Colab**.
    *   Ensure your dataset is correctly linked (e.g., from Google Drive).
    *   Run the training cells to optimize the model.
    *   Use the inference cells to visualize tumor segmentations.

## 👨‍💻 Author

**Youssef Mohamed Moussa**
- 📧 Email: [youssefazmy36@gmail.com](mailto:youssefazmy36@gmail.com)
