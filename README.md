# Skin Lesions Classification Project

A deep learning-based computer vision model for classifying three clinically similar skin conditions: Psoriasis + Lichen Planus, Eczema, and Atopic Dermatitis.

## Background

Psoriasis, Atopic Dermatitis, and Eczema are distinct inflammatory skin diseases that often share overlapping clinical features, making diagnosis challenging. 
Deep learning-based automated classification can assist in differentiating these conditions and supporting diagnosis.

## Dataset

The images used in this project were obtained from Kaggle [Skin diseases image dataset](https://www.kaggle.com/datasets/ismailpromus/skin-diseases-image-dataset) dataset. 
The dataset consists images of skin lesions labeled into three classes:

* Psoriasis + Lichen Planus
* Eczema
* Atopic Dermatitis
  

## Environment & Python Packages

The project was developed and executed using a Jupyter Notebook on the Kaggle website. 
I used pyTorch, Torchvision, and PyTorch Lightning python packages to implement the model.

## Model Architecture  

A deep convolutional neural network (CNN) was designed for lesion classification. It uses EfficientNet-B3 as the backbone, pre-trained on ImageNet (IMAGENET1K_V1), with a modified classifier head consisting of a dropout layer (0.2) and a fully connected layer matching the number of output classes

## Training Process

* Data Split: Training (80%) and Validation (20%)
* Loss Function: Cross-Entropy Loss
* Optimizer: Adam
* Learning Rate Scheduling: Reduce LR on Plateau
* Early Stopping: Stop training when validation loss no longer improves

## Evaluation

Model performance was evaluated on an unseen test set using:

* Accuracy, Precision, Recall, F1-score
* Confusion Matrix to visualize misclassifications

## Results 

Training Process:

![Screenshot 2025-05-28 at 8 34 18](https://github.com/user-attachments/assets/8d4954f3-9b08-4800-9d63-abbf115671cd)


The classification model achieved an overall accuracy of 75%.

![Screenshot 2025-05-28 at 8 23 02](https://github.com/user-attachments/assets/50161f88-73d2-4d20-a833-c101b0be5876)


## Conclusion

This project demonstrates that deep learning can effectively differentiate between Psoriasis + Lichen Planus, Eczema, and Atopic Dermatitis, despite their clinical similarities. Increasing the number of images in future studies could further enhance model performance and classification accuracy.

