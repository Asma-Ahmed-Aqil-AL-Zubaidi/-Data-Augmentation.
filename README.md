#  Image Augmentation Pipeline (Brightness – Rotation – Resolution)

This repository contains a clean, modular, and reusable **image augmentation pipeline** designed to expand and diversify grayscale or RGB datasets using core computer vision techniques.  
It is **task-agnostic**, making it suitable for *any* image-based machine learning or deep learning project.

---

##  Features

-  **Brightness Adjustment** using Keras `ImageDataGenerator`
-  **Random Rotation** (up to ±40°) to simulate viewpoint variance
-  **Resolution Upscaling** via OpenCV’s `INTER_CUBIC` interpolation
-  **Automatic Directory Cleanup** before each run
-  **Google Colab + Google Drive compatibility**
-  **Lightweight and easily extensible** (e.g., add flipping, cropping...)

---

##  Libraries Used

- `OpenCV (cv2)`
- `Keras (ImageDataGenerator)`
- `NumPy`
- `os`, `shutil`, `glob`
- Google Drive interface for Colab

---

##  How It Works

1. Upload your image folder to Google Drive
2. Mount the drive in Colab
3. Run the notebook to:
   - Clean the destination directory (optional)
   - Generate new samples with brightness & rotation
   - Double the image resolution using cubic interpolation
4. Save all outputs to a new organized directory

---

##  Use Cases

- Data expansion for small image datasets  
- Improving model generalization  
- Training robust CNNs  
- Image preprocessing for research, hackathons, or deployment

---

##  Why This Matters

In computer vision, quality **augmentation** is often the key to overcoming limited data.  
This pipeline provides an elegant, easy-to-adapt solution to multiply your dataset while preserving semantic content.

---

##  Author

Developed by [Asma Al-Zubaidi](https://www.linkedin.com)
