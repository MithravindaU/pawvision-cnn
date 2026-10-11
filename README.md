# PawVision CNN
### Image Classification Using Convolutional Neural Networks

PawVision CNN is a deep learning project built with TensorFlow and Keras to classify images into 10 categories using a Convolutional Neural Network (CNN). It uses the CIFAR-10 dataset to explore image preprocessing, feature extraction, model training, and classification performance.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Deep Learning](https://img.shields.io/badge/Deep-Learning-red?style=for-the-badge)


## Overview

The project implements a CNN that learns visual patterns from small colour images and predicts which of the 10 CIFAR-10 categories an image belongs to.

**Supported classes:**
- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

## Technologies Used

- **Python**
- **TensorFlow**
- **Keras**
- **Convolutional Neural Networks (CNN)**
- **Matplotlib**
- **CIFAR-10 Dataset**
- **Google Colab / Jupyter Notebook**

## Model Architecture

The model uses a sequential CNN architecture:

1. **Convolutional Layer:** 32 filters with a 3 × 3 kernel and ReLU activation.
2. **Max Pooling:** Reduces spatial dimensions.
3. **Convolutional Layer:** 64 filters with a 3 × 3 kernel and ReLU activation.
4. **Max Pooling:** Further reduces spatial dimensions.
5. **Flatten Layer:** Converts feature maps into a one-dimensional vector.
6. **Dense Layer:** 64 neurons with ReLU activation.
7. **Output Layer:** 10 outputs, one for each CIFAR-10 class.

The model is compiled using the Adam optimizer and Sparse Categorical Crossentropy loss.

## Workflow

1. Load the CIFAR-10 dataset.
2. Normalize image pixel values to the range 0 to 1.
3. Build the CNN architecture.
4. Compile the model using Adam and Sparse Categorical Crossentropy.
5. Train the model for 5 epochs.
6. Evaluate performance on the test dataset.

## Dataset

The project uses **CIFAR-10**, a dataset containing 60,000 colour images of size 32 × 32 pixels across 10 classes.

- Training images: 50,000
- Test images: 10,000
- Image channels: 3 (RGB)
- Number of classes: 10

The dataset is loaded directly using TensorFlow Keras.

## Model Performance

The model was trained for 5 epochs.

| Metric | Result |
|---|---:|
| Training Accuracy | 69.43% |
| Validation Accuracy | 67.22% |
| Test Accuracy | 67.22% |
| Test Loss | 0.9551 |
| Training Epochs | 5 |

The model achieved a **test accuracy of 67.22%**. These results provide a baseline for further experimentation with CNN architecture, training duration, and image augmentation.

## Project Structure

```text
pawvision-cnn/
├── Cat_Dog_Classifier.ipynb
├── README.md
└── accuracy.png
```

## How to Run

1. Open the notebook in Google Colab or Jupyter Notebook.
2. Run the notebook cells in order.
3. TensorFlow downloads the CIFAR-10 dataset when it is first loaded.
4. Train the CNN for 5 epochs.
5. Review the training history and test evaluation results.

## Future Improvements

- Train for more epochs and monitor overfitting.
- Add data augmentation to improve generalization.
- Experiment with additional convolutional layers and different filter sizes.
- Plot training and validation accuracy and loss curves.
- Display sample predictions with their predicted class labels.
- Compare the CNN with other image classification architectures.
- Explore deployment through a simple image-classification interface.

## Author

**Mithravinda U**

GitHub: [MithravindaU](https://github.com/MithravindaU)

---

*Exploring computer vision through deep learning, one image at a time.*
