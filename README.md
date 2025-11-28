# Image_Colorization_using_VGG

## Project Overview
This project explores and implements a VGG-based deep learning model to convert grayscale images into visually realistic color images. 
The ultimate aim of this project is to implement and evaluate deep learning colorization approaches (VGG-based) to find its strengths and limitations in achieving contextually accurate and visually realistic colorization.

## Approach & Methodology

* Use a pre-trained VGG backbone (or similar) to leverage learned features for image semantics and structure — this helps the model understand contents of grayscale images beyond simple pixel intensities.

* Build a colorization network that takes grayscale input (often L channel in LAB or a single-channel grayscale) and predicts color components (e.g. ab channels in LAB, or RGB color output). This approach reduces the difficulty compared to predicting full RGB from scratch. This kind of approach is common in colorization literature. 

* Use deep learning frameworks (e.g. TensorFlow / Keras or PyTorch) to define, train and test the network.

* Evaluate qualitatively — generate colorized images from grayscale inputs and visually inspect the colorization output.

Method:
1) Loading and preprocessing of input (grayscale or L-channel) images.

2) Conversion between color spaces (e.g. L*a*b ↔ RGB) as needed for colorization tasks.

3) A convolutional neural network based on a VGG-inspired architecture, trained to predict color channels (e.g. a*, b*) from grayscale input.

4) Training loops, loss definitions, and utilities for model evaluation & output visualization.

Examples showing before (grayscale) vs after (colorized) results — helping to gauge the performance and output quality.
<img width="701" height="744" alt="image" src="https://github.com/user-attachments/assets/c5c02887-a48d-4018-a0a1-a9c133205884" />


