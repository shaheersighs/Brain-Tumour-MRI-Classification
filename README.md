# Brain Tumour MRI Classification
### Fundamentals of Medical Image Processing (on Brain Tumour MRI Dataset)

This project presents an end-to-end deep learning solution for the classification of brain MRI images into four clinically relevant categories: glioma, meningioma, pituitary tumor, and no tumor. The workflow is grounded in the Kaggle “Brain Tumor MRI Dataset” by Masoud Nickparvar and implements a series of professional image processing, augmentation, and explainability techniques. The objective is to demonstrate a reproducible, robust, and interpretable computer vision pipeline suitable for medical image analysis.

![image](https://github.com/user-attachments/assets/7e0d3ec4-ddc8-471b-98c0-d4d85b05ad89)  ![image](https://github.com/user-attachments/assets/949c90d5-02c4-4927-bb42-9985779247ef)



### Dataset Exploration
The dataset consists of 7,313 grayscale MRI images, structured in separate folders for training and testing, and further organized by class.
Training set: 5,712 images
Glioma: 1,321  | Meningioma: 1,339  | Pituitary: 1,457 | No tumor: 1,595
Testing set: 1,311 images
Glioma: 300  | Meningioma: 306  | Pituitary: 300 | No tumor: 405

![image](https://github.com/user-attachments/assets/46230eb5-8a67-4ec5-83a3-939ce8bb3a7b)


### Model Architecture
A custom Convolutional Neural Network (CNN) was constructed using TensorFlow/Keras. The architecture consisted of several convolutional blocks, each followed by batch normalization and ReLU activation, with max pooling and dropout for regularization. The final dense layers mapped the feature representations to four output classes. The model was compiled with the Adam optimizer and categorical cross-entropy loss, with computed class weights used to address label imbalance.

### Evaluation and Results
The trained model was evaluated on the held-out test set. Key performance metrics included:
Test accuracy: Approximately 90.5%
Test loss: Approximately 0.28

![image](https://github.com/user-attachments/assets/3c1dbfad-7787-4c89-a0e7-ff0fd3735bd0)







