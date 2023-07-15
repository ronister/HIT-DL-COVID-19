# HIT-DL-COVID-19
HIT Deep Learning Project - Detecting COVID-19 and Other Respiratory Conditions Using Deep Learning Image Classification on Chest X-Ray Scans
using PyTorch.

**Project Description:**
**The research problem and objective** of this project is, whether we can identify COVID-19 positive cases, Lung Opacity cases, Viral Pneumonia cases or Normal cases using deep learning image classification model on Chest X-Ray (CXR) scans with a reasonably high accuracy.

**The dataset: "COVID-19 Radiography Database"** taken from Kaggle - https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database

In the 2nd update of this dataset, we have 21,165 total cases, which are categorized in four classes:
 - 3616 COVID-19 positive cases
 - 10,192 Normal cases
 - 6012 Lung Opacity (Non-COVID lung infection) cases
 - 1345 Viral Pneumonia cases

In addition, there are corresponding lung masks.
(This dataset will continue to be updated as soon as they have new x-ray images for COVID-19 pneumonia patients).

**Note:** This dataset, and the model that we train in the project, can not be used to diagnose COVID-19 or Viral Pneumonia. We are only using this data for **educational purpose.**
Researchers can use this database to produce useful and impactful scholarly work on COVID-19, which can help in tackling this pandemic.

**Image Formats:**
All the images are in Portable Network Graphics (PNG) file format and the resolution are 256*256 pixels.

**Architecture:** We will use **ResNet-18 model** and compare it to **ResNet-50**, **VGG19** and **DenseNet-121**. The ResNet-18 model is a Convolutional Neural Network (CNN) with 18 layers, and has been pre-trained on a large dataset (such as **ImageNet**) with *millions of images*, allowing it to learn general representations of various visual concepts. By leveraging **transfer learning**, this project takes advantage of the ResNet-18 model's pre-trained weights and fine-tunes it specifically for the problem at hand.

One of the key benefits of this model is **Computational Efficiency:** ResNet-18 strikes a good balance between model complexity and computational efficiency. It offers a relatively compact architecture compared to deeper models like **ResNet-50**, making it easier to train and deploy, especially for projects with limited computational resources.
