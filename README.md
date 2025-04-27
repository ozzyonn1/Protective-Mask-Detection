# Protective Mask Detection

[![Python](https://img.shields.io/badge/Python-3.11-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Detecting the presence of protective face masks on people's faces based on images.  

---

## 📝 Project Description

The aim of this project is to build a computer vision system that can automatically classify images into three categories:
- **With mask**
- **Without mask**
- **Mask worn incorrectly**

We use deep learning techniques based on convolutional neural networks (CNNs).  
The model was trained and evaluated using a publicly available dataset from Kaggle.

---

## 📂 Dataset

The dataset used for training and validation can be found here:  
🔗 [Face Mask Detection Dataset on Kaggle](https://www.kaggle.com/datasets/andrewmvd/face-mask-detection)

> **Important:**  
> The dataset files are **NOT** included in this repository due to their large size.  
> Please download the dataset manually and extract the archive directly into the project folder.

After extraction, your project folder should look like this:

```
protective-mask-detection/
├── annotations/
├── images/
├── archive.zip
├── test1.jpg
├── test2.jpg
├── test3.jpg
├── test4.jpg
├── test5.jpg
└── Coding.ipynb
```

## 📁 Project Structure

```
protective-mask-detection/
├── annotations/         # Annotations for the images
├── images/              # Original dataset images
├── archive.zip          # Original dataset archive
├── test1.jpg - test5.jpg # Test images
├── Coding.ipynb         # Jupyter notebook with code
├── LICENSE
└── README.md
```

---
## 📊 Example Usage

After training, the model can classify input images into three categories with high accuracy:
- Wearing Mask
- No Mask
- Mask Worn Incorrectly


---

## 🚀 Future Improvements

- Add a validation set for better performance monitoring
- Implement real-time mask detection using webcam input
- Optimize the model for deployment on mobile/embedded devices

---

## 📄 License

This project is licensed under the MIT License.  
See the [LICENSE](LICENSE) file for more information.
