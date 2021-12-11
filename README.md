# Classifying Google Quickdraw Images with PyTorch

Contains the template for building and testing a convolutional neural network for identify five classes of images from "Google Quick, Draw!"

https://quickdraw.withgoogle.com

From GQD, there are drawings of airplanes, bicycles, coffee cups, shoes and spoons, each saved in its own numpy bitmap file.

This repo contains jupyter notebooks which walk through the steps of exporting individual pngs from each bitmap file and presorting into testing and training folders seperated by image class.

Then, following a tutorial by Akash N S from Jovian.ai (https://jovian.ai/aakashns/05-cifar10-cnn), a convolutional neural network is trained, applied, and assesed. 
