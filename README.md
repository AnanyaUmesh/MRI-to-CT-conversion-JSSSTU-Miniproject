# MRI to CT Conversion using DCNN and TensorFlow

This project aims to develop a Deep Convolutional Neural Network (DCNN) model using TensorFlow for converting Magnetic Resonance Imaging (MRI) images to Computed Tomography (CT) images. The conversion process involves training a model to learn the mapping between MRI and CT images, enabling the generation of CT-like images from MRI inputs.

## Overview

Medical imaging often involves different modalities, each with its unique characteristics and advantages. While MRI provides detailed anatomical information, CT imaging offers high-resolution density information. Converting MRI images to CT-like representations can be valuable in scenarios where CT imaging is not available or to complement MRI data with density information.

## Dataset

The dataset used for training and evaluation consists of paired MRI and CT images. Each MRI image is associated with its corresponding CT image, forming a paired dataset. The dataset should be preprocessed and organized into training, validation, and test sets before training the model.

## Model Architecture

The DCNN model architecture is designed to learn the complex mapping between MRI and CT images. It typically consists of multiple convolutional layers followed by pooling layers for feature extraction, followed by fully connected layers for regression or classification. The exact architecture can be customized based on the complexity of the mapping task and available computational resources.

## Training

The model is trained using the paired MRI and CT images. During training, the model learns to minimize the discrepancy between the predicted CT images and the ground truth CT images. Training involves optimizing a loss function, such as Mean Squared Error (MSE) or Structural Similarity Index (SSI), using an optimization algorithm like Stochastic Gradient Descent (SGD) or Adam.

## Evaluation

The trained model is evaluated using separate validation and test datasets. Evaluation metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and Structural Similarity Index (SSI) are computed to assess the model's performance. Qualitative evaluation through visual inspection of generated CT-like images can also provide insights into the model's effectiveness.

### Results

- **Quantitative Results**:
  - **Mean Absolute Error (MAE)**
  - **Mean Squared Error (MSE)**
  - **Structural Similarity Index (SSI)**

- **Qualitative Results**:
  - Visual inspection of generated CT-like images shows a high degree of similarity to ground truth CT images.
  - Example images demonstrating successful conversion from MRI to CT are included in the `sample` directory.

## Conclusion

The DCNN model trained in this project demonstrates promising results in converting MRI images to CT-like representations. The quantitative evaluation metrics indicate good performance, and qualitative assessment confirms the visual similarity between generated CT images and ground truth CT images. Further research could explore enhancements to the model architecture, optimization techniques, and dataset augmentation methods to improve performance and generalization.
