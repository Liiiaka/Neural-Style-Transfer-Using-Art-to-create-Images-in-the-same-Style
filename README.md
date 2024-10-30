# Neural Style Transfer: Artistic Style Recreation with Convolutional Neural Networks

Welcome to our implementation of neural style transfer, a technique for blending the content of one image with the artistic style of another. Our project builds on the groundbreaking work of [Gatys et al. (2016)](https://doi.org/10.1109/cvpr.2016.265) and explores further variations in style transfer realism and experimental image synthesis using both pre-trained and custom-trained VGG networks.

## 📝 Abstract

This paper implements an artistic style transfer approach based on ”A Neural Algorithm of Artistic Style” by Gatys et al. (2016). We begin with a brief explanation of
how artistic style transfer functions, followed by an overview of various approaches to this challenge. We continue with a more detailed explanation of the pre-trained VGG network and loss functions used in the original paper and in our implementation. Subsequently, we describe our own network implementation of a similar network
and present the results obtained with it. Furthermore, we present and compare results obtained from using pre-trained networks and evaluate how different parameters in-
fluence the outcome. Additionally, we explore the inverse application of making art more realistic and use our results to highlight the limitations of our approach. Finally, we summarize our findings and outline for future research

## 🗂️ Repository Structure

The primary files for executing the model are:

- **Training the Custom Network**: `VGG13/VGG13_Training.py` - Trains a VGG13 model from scratch.
- **Performing Style Transfer**:
  - `VGG13/VGG13_Style_Transfer.py` - Transfers artistic style using the custom-trained VGG13 model. *Ensure to update the path to exported weights in line 139.*
  - `Pretrained_VGG/Style_Transfer.py` - Uses pre-trained VGG models for high-resolution style transfer.

Supporting files:
- `VGG13/VGG13_Utils.py` and `Pretrained_VGG/General_Utils.py`: Essential functions for training and style transfer operations. Minor differences exist to optimize functionality across custom and pre-trained models.

**Output**: Both `VGG13_Style_Transfer.py` and `Style_Transfer.py` export results as `.jpg` files.

## 🔧 Setup and Requirements

- **Python Version**: 3.6.5

## 🧠 Contributors
- Annika Richter
- Cornelius Wolff
- Juri Moriße
