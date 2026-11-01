# Chest-X-Ray-Pneumonia-Classification-Using-CNN
A deep learning project that uses a Convolutional Neural Network (CNN) to classify chest X-ray images into Normal and Pneumonia classes. 
The project aims to demonstrate how deep learning can support medical image analysis by providing fast and consistent pneumonia detection.

# Project Overview
The model was developed using the Labeled Chest X-Ray Images dataset from Kaggle. The dataset contains chest X-ray images categorized into Normal and Pneumonia classes.
The project covers the complete machine learning pipeline, including data exploration, preprocessing, image augmentation, model development, training, and evaluation.

# Methodology
Explored image dimensions, pixel distributions, and image quality.
Resized images to provide consistent inputs to the CNN.
Created a stratified validation set using an 80/20 split from the original training data.
Applied image augmentation to training images, while validation and test images were only rescaled.
Developed a Custom CNN model from scratch.
Used Binary Cross-Entropy as the loss function and the Adam optimizer.
Trained the model for 10 epochs and used callbacks such as Early Stopping and ReduceLROnPlateau to help control overfitting and adjust the learning rate.

# Results
The model achieved approximately:

- 95% Validation Accuracy
- 86% Test Accuracy
- 98% Recall for Pneumonia
- 64% Recall for Normal cases
On the test set of 624 images, the model correctly classified 534 images. It detected 384 out of 390 Pneumonia cases, resulting in a low number of missed pneumonia cases.

# Conclusion
The results demonstrate that a custom CNN can effectively learn visual patterns from chest X-ray images and detect pneumonia, particularly achieving high recall for pneumonia cases.

The project also highlights the importance of improving the classification of Normal X-rays to reduce false positives. Overall, the project demonstrates the potential of deep learning to support radiologists and reduce diagnostic delays.

# Technologies
Python
TensorFlow / Keras
Convolutional Neural Networks (CNN)
Deep Learning
ImageDataGenerator
Data Augmentation
Matplotlib
Seaborn
Scikit-learn
