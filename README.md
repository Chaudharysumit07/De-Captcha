# DeCaptcha: CAPTCHA Recognition System
**DeCaptcha** is a lightweight, high-performance machine learning solution designed to recognize CAPTCHA characters with exceptional speed and accuracy. By combining robust image pre-processing with optimized classification algorithms, this project delivers a highly efficient solver suitable for real-time applications.
## 🚀 Project Overview
The primary goal of DeCaptcha is to automate the recognition of text within CAPTCHA images, which are typically designed to feature complex backgrounds and distorted text to thwart automated systems. This project tackles the challenge through a two-stage pipeline: **Extraction** and **Recognition**.

## 🛠️ Methodology
* 1. Image Pre-processing & Segmentation
     Before feeding data into the model, raw CAPTCHA images undergo a rigorous pre-processing pipeline to maximize character clarity:
     - **Background Removal**: Applied advanced filtering techniques to separate text from noisy, complex backgrounds.
     - **Character Segmentation**: Employed segmentation algorithms to isolate individual characters from the CAPTCHA string, treating each character as a distinct classification task.
* 2. Model Exploration
     We explored three distinct machine learning architectures to find the optimal balance between accuracy and computational cost:
     - **Support Vector Machines (SVM)**: Tested for their effectiveness in high-dimensional spaces.
     - **Convolutional Neural Networks (CNN)**: Evaluated for their ability to learn spatial hierarchies in image data.
     - **Logistic Regression**: Analyzed for simplicity and speed.
     - 
## 🏆 Performance & Results
After a comprehensive evaluation of all three approaches, **Logistic Regression** emerged as the optimal choice, outperforming more complex models in terms of efficiency while maintaining high accuracy.
|Metric|Result|
|:---|:---|
|Accuracy|98.5%|
|Prediction Time|4 ms|
|Model Size|174 KB|

**Key Takeaways** 
- **High Precision**: The final model achieves a 98.5% accuracy rate on the recognition task.
- **Ultra-Lightweight**: At just 174KB, the model is incredibly resource-efficient compared to typical deep learning weights.
- **Real-Time Speed**: With a prediction latency of only 4 milliseconds, the system is suitable for high-throughput environments.
- 
##🔮 Future Improvements
- Handling overlapping characters with advanced segmentation.
- Expanding the dataset to include variable-length CAPTCHAs.
- Testing on adversarial CAPTCHA examples.
