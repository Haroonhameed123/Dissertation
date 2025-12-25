# 🐶 Dog Breed Classification Using Deep Learning

##  Project Overview

This project focuses on developing a deep learning–based system for automatic dog breed classification from images. Dog breed recognition is a challenging computer vision task due to high visual similarity between breeds, variations in pose, lighting conditions, and background complexity.

To address these challenges, three different modelling approaches were implemented and compared:

A Convolutional Neural Network (CNN) trained from scratch (baseline model)

A transfer learning approach using EfficientNet-B3

A hybrid deep learning model combining ResNet50 and ResNeXt101

The models were evaluated on a dataset containing 120 dog breeds to analyse the impact of transfer learning and hybrid architectures on fine-grained image classification performance.

##  Models Implemented

###  CNN From Scratch

Custom CNN architecture

Trained on the 20 most frequent dog breeds

Used as a baseline for performance comparison

### EfficientNet-B3 (Transfer Learning)

Pretrained on ImageNet

Fine-tuned on all 120 dog breeds

Includes data augmentation and class balancing

###  Hybrid ResNet Model (Best Performing)

Combines ResNet50 and ResNeXt101 as parallel feature extractors

Features are concatenated and passed to a classification head

Achieved the highest classification accuracy

## 🛠️ Technologies Used

Programming Language: Python 3.11

Deep Learning Frameworks: PyTorch, TorchVision

Libraries: NumPy, Pandas, Scikit-learn, Matplotlib, Pillow

Platforms: Google Colab Pro (GPU), Visual Studio Code

Version Control: GitHub

## 📂 Dataset

Custom-labelled dog breed image dataset

120 dog breed classes

Thousands of RGB images

Large variation in lighting, pose, background, and image quality

Moderate class imbalance

A stratified data split was used to ensure balanced representation across training and validation sets.

## How to Run the Code
1. Clone the Repository
git clone <your-repository-link>
cd dog-breed-classification

2. Install Required Packages
pip install -r requirements.txt


Example requirements.txt:

torch
torchvision
numpy
pandas
scikit-learn
matplotlib
pillow
tqdm

3. Run the Models

cnn_from_scratch.py — CNN baseline model

efficientnet_b3.py — EfficientNet-B3 transfer learning model

hybrid_resnet.py — Hybrid ResNet50 + ResNeXt101 model

Run using:

python filename.py

## 📈 Evaluation Metrics

The models were evaluated using:

Classification accuracy

Training and validation loss

Confusion matrices

Learning curves

Performance Summary
Model	Number of Breeds	Accuracy
CNN From Scratch	20	77.78%
EfficientNet-B3	120	91.01%
Hybrid ResNet Model	120	92.62%

## Applications

Automated dog breed identification

Pet adoption and animal welfare platforms

Veterinary support systems

Educational tools for learning dog breeds

Image-based animal classification research

## Conclusion

This project demonstrates that transfer learning and hybrid deep learning architectures significantly improve performance in fine-grained dog breed classification tasks. While a CNN trained from scratch provides a useful baseline, pretrained and hybrid models achieve superior accuracy and generalisation. The hybrid ResNet model achieved the best results and offers a robust solution for large-scale dog breed recognition.

Contact

For questions, feedback, or collaboration, feel free to reach out via GitHub.

