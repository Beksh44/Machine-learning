# Neural Network Image Classifier

This project is focused on building and experimenting with neural network models for multi-class classification of grayscale images. The data is based on modified 32×32 pixel versions of the [Fashion MNIST dataset](https://www.kaggle.com/datasets/zalando-research/fashionmnist).

## About the Project

The goal was to classify images into multiple categories using both fully connected (dense) and convolutional neural networks. I worked through several stages: exploring the data, building various models, tuning hyperparameters, and finally generating predictions on an unseen test set.

## Dataset

- `train.csv`: contains labeled training images.
- Each image is represented as a row of pixel values, with the label column in `train.csv`.

## Approach

1. **Data Preparation & Exploration**  
   I loaded the data, visualized sample images, and explored class distributions. I also split the dataset into training and validation sets.

2. **Dense Neural Networks**  
   I tested several dense models with different architectures, using techniques like:
   - Normalization / standardization
   - Dropout regularization
   - Optimizer variations (Adam, SGD, etc.)

3. **Convolutional Neural Networks (CNNs)**  
   I built and trained CNN models, which significantly improved performance. I tried different combinations of:
   - Convolutional and pooling layers
   - Activation functions
   - Batch normalization and dropout

4. **Model Selection**  
   Based on validation accuracy and generalization performance, I selected the best-performing model.


## Tools & Libraries

- Python
- Pytorch
- NumPy, Pandas
- Matplotlib for visualizations

## Results

The final model achieved high classification accuracy and generalizes well. The CNN outperformed all dense models, confirming the advantage of spatial feature extraction for image data.

