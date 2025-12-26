# 🖼️ U-Net: Semantic Image Segmentation from Scratch

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Framework](https://img.shields.io/badge/Framework-TensorFlow%20%7C%20Keras-orange)
![Task](https://img.shields.io/badge/Task-Semantic%20Segmentation-green)
![Architecture](https://img.shields.io/badge/Model-Encoder--Decoder-purple)

## 📌 Project Overview
This project implements the **U-Net architecture** from scratch for semantic image segmentation tasks. Originally designed for biomedical image segmentation, U-Net has become the gold standard for pixel-level classification problems.

The model is built to take an input image and output a precise segmentation mask, classifying every pixel into a specific category.

## ⚙️ Technical Architecture
The U-Net consists of a symmetric **Encoder-Decoder** structure with **Skip Connections**:

### 1. 📉 Encoder (Contracting Path)
* Captures context using a series of convolutional blocks followed by max-pooling.
* Reduces spatial dimensions while increasing feature depth.

### 2. 🌉 Bottleneck
* The bridge connecting the encoder and decoder, processing the most abstract features.

### 3. 📈 Decoder (Expansive Path)
* Enables precise localization using **Transposed Convolutions** (Upsampling).
* Concatenates feature maps from the Encoder via **Skip Connections** to recover lost spatial information during downsampling.

## 🛠️ Key Features
* **Custom Implementation:** Full model architecture built layer-by-layer without pre-trained backbones.
* **Skip Connections:** Implemented to solve the vanishing gradient problem and preserve fine-grained details.
* **Data Preprocessing:** Image normalization and mask handling for supervised learning.

## 🚀 How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/mariamashraf731/UNet-Semantic-Segmentor.git](https://github.com/mariamashraf731/UNet-Semantic-Segmentor.git)
    ```
2.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Train the Model:**
    Open `notebooks/UNet_Implementation.ipynb` and run the cells to train on your dataset.

## 👨‍💻 Tech Stack
* **Language:** Python
* **Deep Learning:** TensorFlow / Keras
* **Concepts:** CNNs, Transposed Convolution, Max Pooling, Semantic Segmentation.