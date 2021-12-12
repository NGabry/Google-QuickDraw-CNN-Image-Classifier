# Classifying Google Quickdraw Images with PyTorch

Contains the template for building and testing a convolutional neural network for identify five classes of images from "Google Quick, Draw!"

https://quickdraw.withgoogle.com

From GQD, there are drawings of airplanes, bicycles, coffee cups, shoes and spoons, each saved in its own numpy bitmap file. Each bitmap contains 10,000 28x28 images condensed into a single array: 
![alt text]()https://github.com/NGabry/Google-QuickDraw-CNN-Image-Classifier/blob/main/images/airplane_bitmap_subset.png?raw=true)

This repo contains jupyter notebooks which walk through the steps of exporting individual pngs from each bitmap file and presorting into testing and training folders seperated by image class.

Then, following a tutorial by Akash N S from Jovian.ai (https://jovian.ai/aakashns/05-cifar10-cnn), a convolutional neural network is trained, applied, and assesed. 

The goal here is to create the neural network seen below, and see how well it is able to accurately classify novel images.

![alt text]()https://github.com/NGabry/Google-QuickDraw-CNN-Image-Classifier/blob/main/images/CNN.png?raw=true)

To do this, images are shuffled and prepped for batch loading:

![alt text]()https://github.com/NGabry/Google-QuickDraw-CNN-Image-Classifier/blob/main/images/batch_load.png?raw=true)

After our dataloaders are initialized, the neural network is defined and validated prior to training on our train set.

Once trained, we are then able to asses the accuracy of our classifier across training epochs based on its ability to classifty the validation set:

![alt text]()https://github.com/NGabry/Google-QuickDraw-CNN-Image-Classifier/blob/main/images/Accuracy_Across_Epochs.png?raw=true)

as well as visualize loss across epochs. This allows us to see that we may be overfitting our data! 

![alt text]()https://github.com/NGabry/Google-QuickDraw-CNN-Image-Classifier/blob/main/images/Loss_Across_Epochs.png?raw=true)
