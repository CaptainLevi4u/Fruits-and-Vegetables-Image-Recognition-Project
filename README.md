🥕🍎 Fruit & Vegetable Image Classification using CNN
📌 Project Overview

This project implements a Multi-Class Image Classification Model using a custom-built Convolutional Neural Network (CNN) to classify fruits and vegetables into 36 different categories.

The model was trained from scratch using TensorFlow & Keras, evaluated on a separate test set, and optimized using EarlyStopping to prevent overfitting.

📂 Dataset

Dataset source (Kaggle):
🔗 https://www.kaggle.com/datasets/kritikseth/fruit-and-vegetable-image-recognition

Dataset Structure:
train/
validation/
test/

36 classes

RGB images

Resized to 224×224 during preprocessing

🧠 Model Architecture

The CNN architecture consists of:

5 Convolutional Blocks

Conv2D

Batch Normalization

ReLU Activation

MaxPooling

Flatten Layer

Dense Layer (256 units)

Dropout (0.3)

Output Layer (Softmax – 36 classes)

This architecture was designed to progressively extract hierarchical image features while maintaining generalization.

⚙️ Training Configuration
Parameter	Value
Optimizer	Adam
Loss Function	Sparse Categorical Crossentropy
Batch Size	32
Epochs	30
EarlyStopping	Patience = 5

🚀 Future Improvements

Apply Data Augmentation
Use Transfer Learning (VGG16 / ResNet50 / EfficientNet)
Add Learning Rate Scheduler

📊 Results
✔ Strong accuracy on the test dataset
✔ Good generalization between training & validation
✔ Stable convergence with minimal overfitting
✔ Clean and reusable pipeline for future Computer Vision tasks

📸 Performance curves and test results are attached below.
<img width="891" height="93" alt="Screenshot 2026-03-03 183136" src="https://github.com/user-attachments/assets/86e22506-c9e2-4338-958c-2bc27f7d066c" />
<img width="569" height="455" alt="Model loss" src="https://github.com/user-attachments/assets/9c8aa9da-c0bf-4c8d-91ff-677ba0167a3a" />
<img width="569" height="455" alt="Model Accuracy" src="https://github.com/user-attachments/assets/35810b29-4097-4423-82a0-39e4c8abf9e4" />
<img width="1919" height="861" alt="Screenshot 2026-02-27 202919" src="https://github.com/user-attachments/assets/f6819def-e9ea-4d91-873e-8d701700419c" />
<img width="1919" height="886" alt="Screenshot 2026-02-27 202856" src="https://github.com/user-attachments/assets/6549e801-4329-45f0-9967-617e3aeecfd9" />

