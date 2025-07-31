# CNN Image Classification - CIFAR-10

This project implements a Convolutional Neural Network (CNN) using TensorFlow/Keras to classify images from the CIFAR-10 dataset. The model is trained to distinguish between 10 classes of 32×32 color images such as airplanes, cats, trucks, and ships.

## Dataset
- **Name:** CIFAR-10
- **Size:** 60,000 images (50,000 train / 10,000 test)
- **Classes:** airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck
- **Image Size:** 32×32 RGB

## Model Architecture
- **3 Convolutional Layers** with ReLU activation and MaxPooling
- **Dropout** layers for regularization
- **2 Fully Connected (Dense) Layers**
- **Softmax** output for multi-class classification

## Training Details
- **Optimizer:** Adam (adaptive learning rate)
- **Loss Function:** Sparse Categorical Crossentropy
- **Batch Size:** 64
- **Epochs:** 30
- **Callbacks:**
  - EarlyStopping (patience = 5)
  - ReduceLROnPlateau (factor = 0.5, patience = 3)
- **Validation Split:** 20%

## Evaluation
- Achieved ~77% test accuracy
- Evaluated using:
  - Accuracy
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1-score)

## Visualizations
- Training vs Validation Accuracy and Loss plots
- Confusion Matrix Heatmap
