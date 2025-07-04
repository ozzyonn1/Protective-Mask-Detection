# Protective Mask Detection

[![Python](https://img.shields.io/badge/Python-3.11-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Detecting the presence of protective face masks on people's faces using computer vision and deep learning.

---

## Project Description

This project aims to build a deep learning-based computer vision system that classifies images into three categories:
- **With Mask**
- **Without Mask**
- **Mask Worn Incorrectly**

The model is based on **Convolutional Neural Networks (CNN)** and uses **transfer learning** via **MobileNetV2** — a lightweight model suitable for real-time applications.  
Training and evaluation were conducted using a labeled dataset from Kaggle containing images and bounding box annotations.

---

## Dataset

The dataset used is publicly available on Kaggle:  
[Face Mask Detection Dataset – by andrewmvd](https://www.kaggle.com/datasets/andrewmvd/face-mask-detection)

> **Note:** The dataset is not included in this repository due to size restrictions.  
> Please download it manually and extract it into the project directory.

Expected folder structure:

```
protective-mask-detection/
├── annotations/ # XML annotations (Pascal VOC format)
├── images/ # Raw image files
├── archive.zip # Original dataset archive
├── test1.jpg - test5.jpg # Sample test images
├── Coding.ipynb # Jupyter notebook with full training pipeline
```

---

## Project Structure

| File/Folder       | Description |
|-------------------|-------------|
| `Coding.ipynb`    | Main notebook with preprocessing, model training, evaluation, and inference |
| `images/`         | Input images used for training/testing |
| `annotations/`    | XML annotations with class labels and bounding boxes |
| `test*.jpg`       | Custom images used for final testing |
| `README.md`       | Project description |
| `LICENSE`         | MIT license |

---

## Model & Techniques Used

- **MobileNetV2** (pretrained on ImageNet, used for transfer learning)
- **Fine-tuning** of the last CNN layers
   **Image preprocessing** using OpenCV and TensorFlow
- **Multi-class classification** using softmax activation
- **Evaluation** using accuracy score and confusion matrix

---

## Libraries & Tools

- `TensorFlow`, `Keras`
- `OpenCV`
- `NumPy`, `matplotlib`, `os`, `xml.etree.ElementTree`
-  Jupyter environment

---

## Example Usage

After training, the model can classify any input image into:
- **Wearing Mask**
- **No Mask**
- **Mask Worn Incorrectly**

Example output:

Input Image → Predicted: Mask Worn Incorrectly

---

## License

This project is licensed under the **MIT License**.  
See the [LICENSE](LICENSE) file for details.

---

## Author

**Oleh Zemlianyi**  
[LinkedIn](https://www.linkedin.com/in/oleh-zemlianyi) • [GitHub](https://github.com/ozzyonn1)
