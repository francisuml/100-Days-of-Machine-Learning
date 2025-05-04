# 🧠 Autoencoder for Anomaly Detection
This project demonstrates how autoencoders, a type of unsupervised deep learning model, can be used for anomaly detection and dimensionality reduction. The workflow includes data preprocessing, training an autoencoder on normal data, detecting anomalies based on reconstruction error, and visualizing the latent space using deep learning representations.

📌 Objectives
Understand how autoencoders work for unsupervised learning

Implement an autoencoder model using TensorFlow/Keras

Use the model for anomaly detection by learning normal patterns

Perform dimensionality reduction with the encoder's bottleneck layer

Visualize model architecture and learned features using Plotly

## 🧬 Key Concepts
### 🔍 What is an Autoencoder?
An autoencoder is a neural network trained to reconstruct its input. It consists of:

Encoder: Compresses the input data into a lower-dimensional latent representation.

Bottleneck: The latent space (compressed features).

Decoder: Reconstructs the original data from the compressed representation.

During training, the network learns the most important features needed to represent the input data accurately. For anomaly detection, it is trained only on "normal" data.

### 🚨 Anomaly Detection
Once trained, the autoencoder will:

Reconstruct normal data with low error

Reconstruct anomalous data poorly (high reconstruction error)
By setting a threshold on the reconstruction loss, we classify whether a sample is anomalous.

## 🛠️ Model Architecture
Input layer: 20 neurons

Encoder:

Dense(14) → ReLU

Dense(7) → ReLU (Bottleneck)

Decoder:

Dense(14) → ReLU

Dense(20) → Sigmoid

Total Parameters: 811
The model was visualized using Plotly to display the layered neural architecture.

## 📊 Results & Visualizations
The model was trained for 20 epochs.

Loss steadily decreased, indicating effective learning.

Latent space extracted from the bottleneck layer was visualized using 3D scatter plots.

Abnormal instances were separated effectively using reconstruction loss.

## 📈 Insights
Autoencoders are powerful tools for anomaly detection when only normal samples are available.

The bottleneck layer effectively reduces dimensions while retaining essential data characteristics.

Plotly visualizations provide intuitive insights into latent representations and network structure.

## ✅ Conclusion
Autoencoders are highly effective for learning data structure in an unsupervised setting. This project demonstrated their application in anomaly detection, dimensionality reduction, and latent space analysis, supported by intuitive visualizations and metrics.

