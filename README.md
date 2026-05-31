# CNN-Based Waste Image Classification for Recycling 

## Project Overview
This project focuses on the automation of waste sorting using Deep Learning. By utilizing Convolutional Neural Networks (CNN), the project aims to classify images of waste materials into distinct categories to facilitate recycling processes.

## Dataset Information
The dataset(Garbage Classification ) consists of labeled images of various waste categories(12 Class). The images were preprocessed to ensure consistency, and data augmentation techniques were applied to improve model robustness and generalization during training.

## Key Features & Methodology
- **Deep Learning Architectures:** Implementation and comparison of a custom CNN, MobileNetV2, and ResNet50.
- **Data Analysis:** Visualizing accuracy and loss curves to monitor training progress and prevent overfitting.
- **Performance Metrics:** Detailed evaluation using confusion matrices and Grad-CAM for model explainability.

## Project Structure
- `/Notebook`: Contains the Jupyter notebook with the full implementation and training pipeline.
- `/Results`: Contains documented figures, including confusion matrices and performance curves.
- `/Models`: Pre-trained weights for the custom and MobileNetV2 models.

## How to Access
1. **View the Notebook:** View the code directly here: [View Notebook](https://nbviewer.org/github/farzaneh3745/CNN-Based-Waste-Image-Classification-for-Recycling/blob/main/Notebook/notebook-wasterecycling-codes.ipynb)
2. **Download Models:** The ResNet50 model weights (93MB) are available for download in the **[Releases](https://github.com/farzaneh3745/CNN-Based-Waste-Image-Classification-for-Recycling/releases)** section.

## Technologies Used
- **Python**
- **TensorFlow / Keras**
- **Matplotlib & Seaborn**
- **Scikit-learn**
