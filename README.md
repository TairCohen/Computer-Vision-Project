# Skin lesions Classification Project

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

## Model Architecture #TODO 

A deep convolutional neural network (CNN) was designed for lesion classification. 
The architecture consists of:

* Pretrained CNN Backbone () for feature extraction
* Fully Connected Layers with dropout and batch normalization
* Softmax Activation for multi-class classification

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

## Conclusion

This project demonstrates that deep learning can effectively differentiate between Psoriasis + Lichen Planus, Eczema, and Atopic Dermatitis, despite their clinical similarities. 
