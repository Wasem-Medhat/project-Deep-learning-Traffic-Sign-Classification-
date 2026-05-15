🚦 Traffic Sign Classification Using CNN


📌 Project Overview


This project presents a Deep Learning-based Traffic Sign Classification System using Convolutional Neural Networks (CNNs) and the German Traffic Sign Recognition Benchmark (GTSRB) dataset.

The main objective of the project is to classify traffic signs into 43 different categories using advanced Computer Vision and Deep Learning techniques.

Additionally, the project compares the performance of two optimization algorithms:



✨ Adam Optimizer

✨ SGD (Stochastic Gradient Descent) Optimizer


The entire model was implemented using PyTorch, and its performance was evaluated through:

Training Accuracy

Validation Accuracy

Training & Validation Loss Curves

Performance Visualization Graphs

🎯 Project Objectives

The main goals of this project are to:

✅ Build an efficient CNN model for traffic sign recognition

✅ Improve classification accuracy using preprocessing and augmentation

✅ Compare different optimization techniques

✅ Analyze model performance visually using graphs

✅ Test the trained model on unseen traffic sign images


📂 Dataset Used

🚥 German Traffic Sign Recognition Benchmark (GTSRB)

Dataset Link:

GTSRB Dataset on Kaggle

📊 Dataset Features

43 traffic sign classes

Thousands of labeled training images

Separate training and testing datasets

🛑 Examples of Traffic Signs
Speed Limit Signs

Stop Signs

No Entry Signs

Warning Signs

Direction Signs

⚙️ Project Workflow

The project pipeline consists of the following stages:

Step	Description
1️⃣	Dataset Loading

2️⃣	Data Preprocessing

3️⃣	Data Augmentation

4️⃣	Dataset Splitting

5️⃣	CNN Model Building

6️⃣	Model Training

7️⃣	Optimizer Comparison

8️⃣	Model Evaluation

9️⃣	Testing on New Images

📥 Step 1: Dataset Loading

The dataset was loaded from Google Drive after extracting the ZIP file.

🔹 Main Operations

Mounting Google Drive

Extracting dataset files

Verifying dataset paths

Reading training and testing folders

📁 Dataset Structure

Train Folder

Test Folder

🧹 Step 2: Data Preprocessing

Before feeding images into the CNN model, several preprocessing operations were applied.

🔧 Preprocessing Operations

📏 Image Resizing

All images were resized to:

32×32

This ensures consistent image dimensions across the dataset.

🔄 Tensor Conversion

Images were converted into tensors to make them compatible with PyTorch.

📉 Normalization

Normalization improves:

Training stability

Model convergence

Learning efficiency

🎨 Step 3: Data Augmentation

Data augmentation techniques were applied to improve model generalization and reduce overfitting.

✨ Techniques Used
Random Rotation

Random Horizontal Flip

🎯 Benefits

✅ Increases dataset diversity

✅ Helps the model learn robust features

✅ Improves performance on unseen data

📊 Step 4: Dataset Splitting

The dataset was divided into training and validation sets.

Dataset	Percentage

Training Set	80%

Validation Set	20%

🎯 Purpose of Validation Set

Monitor model performance

Detect overfitting

Evaluate generalization ability

🧠 Step 5: CNN Model Architecture

A custom Convolutional Neural Network (CNN) architecture was designed for this project.

🏗️ CNN Layers Used

🔹 Convolution Layers (Conv2D)

Used for extracting important image features.

🔹 Batch Normalization

Improves training speed and model stability.

🔹 ReLU Activation Function

Introduces non-linearity into the model.

🔹 Max Pooling

Reduces image dimensions and computational complexity.

🔹 Fully Connected Layers

Used for final classification.

🔹 Dropout Layer

Helps reduce overfitting by randomly disabling neurons during training.

🧾 CNN Architecture Summary

Layer Type	Purpose

Conv2D	Feature Extraction

BatchNorm2D	Training Stability

ReLU	Activation Function

MaxPool2D	Dimensionality Reduction

Dropout	Overfitting Reduction

Linear Layer	Final Classification

🏋️ Step 6: Training Process

The CNN model was trained using:

Cross Entropy Loss Function

Backpropagation

Gradient Descent Optimization

⚙️ Training Hyperparameters

Hyperparameter	Value

Batch Size	64

Learning Rate	0.001

Epochs	10

Number of Classes	43

🚀 Hardware Support

The project automatically detects whether CUDA (GPU) is available for faster training.

🔍 Step 7: Optimizers Comparison

Two experiments were performed to compare optimization performance.

🟢 Experiment 1: CNN + Adam Optimizer

Adam combines:

Momentum

Adaptive Learning Rate

✅ Advantages of Adam

Faster convergence

More stable training

Excellent performance in deep learning tasks

🔵 Experiment 2: CNN + SGD Optimizer

SGD updates model weights gradually using gradient descent.

✅ Advantages of SGD

Simpler optimization technique

Lower memory usage

Can generalize effectively in some cases

📈 Step 8: Model Evaluation

The model performance was evaluated using several metrics.

📊 Evaluation Metrics

✅ Training Accuracy

Measures performance on training data.

✅ Validation Accuracy

Measures generalization ability.

✅ Training Loss

Indicates how effectively the model is learning.

✅ Validation Loss

Helps identify overfitting problems.

📉 Visualization of Results

The project visualizes:

📌 Adam Accuracy Curve

📌 Adam Loss Curve

📌 SGD Accuracy Curve

📌 SGD Loss Curve

These visualizations help analyze:

Model learning behavior

Convergence speed

Overfitting and underfitting

🧪 Step 9: Testing on New Images

After training, the model was tested on unseen traffic sign images.

🔄 Testing Procedure

1️⃣ Read the input image

2️⃣ Apply preprocessing operations

3️⃣ Pass the image through the trained CNN

4️⃣ Predict the traffic sign class

5️⃣ Display the predicted label

This demonstrates the practical real-world usability of the system.

🎯 Expected Results

The expected outputs include:

✅ Successful traffic sign classification

✅ High training and validation accuracy

✅ Accuracy and loss visualization graphs

✅ Performance comparison between Adam and SGD

✅ Predicted labels for unseen images

🌟 Advantages of the Project

✨ Applies real-world computer vision techniques

✨ Demonstrates CNN implementation from scratch

✨ Uses advanced image augmentation techniques

✨ Compares optimization algorithms

✨ Provides visual analysis through graphs

✨ Can be extended for autonomous driving systems

⚠️ Challenges Faced

Some challenges encountered during development include:

Overfitting

Long training time

Dataset imbalance

GPU memory limitations

Hyperparameter tuning difficulties

🌍 Real-World Applications

Traffic sign classification systems are widely used in:

🚗 Autonomous Vehicles

🚦 Driver Assistance Systems

🛣️ Smart Transportation Systems

🚨 Road Safety Monitoring

🚘 Intelligent Traffic Management

🏁 Conclusion

This project successfully demonstrates how Convolutional Neural Networks (CNNs) can be applied to traffic sign recognition tasks.

The project covers the complete deep learning pipeline, including:

✅ Data Preprocessing

✅ Data Augmentation

✅ CNN Architecture Design

✅ Model Training

✅ Evaluation & Visualization

✅ Testing on New Images

The comparison between Adam and SGD optimizers also provides valuable insights into how optimization techniques impact deep learning model performance.

Overall, this project represents a strong practical application of:

🧠 Deep Learning

👁️ Computer Vision

🔥 PyTorch Frameworks

for intelligent traffic sign recognition systems.

📚 References
PyTorch Documentation

Torchvision Documentation

GTSRB Dataset

Deep Learning Research Papers
