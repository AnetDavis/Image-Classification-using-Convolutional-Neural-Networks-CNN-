# Image Classification using Convolutional Neural Networks (CNN)

**Author:** Anet Davis

**Registration Number:** 23BHI10146

**Application Number:** IN26011852

**Batch Number:** 1A

**Email ID:** anet.23bhi10146@vitbhopal.ac.in

---

## Objective

The objective of this project is to develop a Convolutional Neural Network (CNN) that can accurately classify images of cats and dogs. By learning visual features directly from images, the model performs binary image classification and predicts the correct category for unseen data.

---

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Pillow

---

## Methodology

### 1. Data Preparation

- Loaded the image dataset for binary classification.
- Removed invalid or corrupted image files.
- Resized all images to **128 × 128** pixels.
- Normalized pixel values to improve model performance.
- Split the dataset into training and testing sets.
- Generated image batches using **ImageDataGenerator**.

### 2. CNN Model Development

The CNN model consists of multiple convolutional layers for feature extraction followed by fully connected layers for classification.

- Conv2D layer with **32 filters** and ReLU activation.
- MaxPooling2D layer.
- Conv2D layer with **64 filters** and ReLU activation.
- MaxPooling2D layer.
- Conv2D layer with **128 filters** and ReLU activation.
- MaxPooling2D layer.
- Flatten layer.
- Dense layer with **128 neurons** and ReLU activation.
- Output layer with **1 neuron** and Sigmoid activation.

### 3. Model Training

The model was compiled using:

- **Optimizer:** Adam
- **Loss Function:** Binary Crossentropy
- **Epochs:** 10

Training and validation accuracy were monitored throughout the learning process.

### 4. Model Evaluation

The trained model was evaluated using:

- Accuracy
- Loss
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Accuracy and Loss Curves

---

## CNN Architecture

| Layer | Configuration |
|--------|---------------|
| Conv2D | 32 Filters (3×3), ReLU |
| MaxPooling2D | Pool Size (2×2) |
| Conv2D | 64 Filters (3×3), ReLU |
| MaxPooling2D | Pool Size (2×2) |
| Conv2D | 128 Filters (3×3), ReLU |
| MaxPooling2D | Pool Size (2×2) |
| Flatten | Converts feature maps into a vector |
| Dense | 128 Neurons, ReLU |
| Output | 1 Neuron, Sigmoid |

---

## Results

- Test Accuracy: **85.20%**
- Test Loss: **0.7194**
- Precision: **84.43%**
- Recall: **86.32%**
- F1-Score: **85.36%**

The CNN model achieved good performance in distinguishing between cat and dog images. The evaluation metrics indicate balanced predictions and effective feature extraction, making the model suitable for binary image classification tasks.

---

## Conclusion

This project demonstrates how Convolutional Neural Networks can effectively perform image classification by automatically learning meaningful visual features from data. The model achieved strong classification performance and successfully distinguished between cat and dog images.

Future enhancements may include applying data augmentation, dropout layers, batch normalization, and transfer learning models such as ResNet, MobileNet, or EfficientNet to further improve accuracy and generalization.
