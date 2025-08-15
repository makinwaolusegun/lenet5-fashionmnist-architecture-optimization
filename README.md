# lenet5-fashionmnist-architecture-optimization
Implementation of a LeNet-5 CNN trained on the FashionMNIST dataset. Includes experiments with convolution layers, pooling types, activation functions, and filter counts to optimize performance, achieving validation accuracy above 80%.
LeNet-5 FashionMNIST Experiments
📌 Overview

This project implements a LeNet-5 convolutional neural network trained on the FashionMNIST dataset using PyTorch.
Multiple experiments were conducted by varying convolution layers, pooling types, activation functions, and filter counts to optimize performance.
The best configuration achieved a validation accuracy of 90.37%.

📂 Project Structure

lenet5_fashionmnist_experiments.ipynb – Main Jupyter notebook with all model configurations, training loops, and results.

README.md – Project documentation.

🧠 Model Architecture

LeNet-5 was adapted for FashionMNIST with:

Convolutional layers (variable count in experiments)

ReLU or Tanh activations

Max or Average pooling

Fully connected layers for classification

⚙️ Experiments & Results
Model	Configuration	Final Validation Accuracy
Model 1	num_conv_layers=1, activation=ReLU, pooling=Max, filter_size=5, num_filters=[6, 16]	0.8868
Model 2	num_conv_layers=2, activation=ReLU, pooling=Max, filter_size=5, num_filters=[6, 16]	0.8620
Model 3	num_conv_layers=2, activation=ReLU, pooling=Average, filter_size=5, num_filters=[6, 16]	0.8670
Model 4	num_conv_layers=4, activation=ReLU, pooling=Average, filter_size=5, num_filters=[6, 16]	0.8720
Model 5	num_conv_layers=4, activation=ReLU, pooling=Average, filter_size=5, num_filters=[8, 18]	0.9037
Model 6	num_conv_layers=4, activation=Tanh, pooling=Average, filter_size=5, num_filters=[8, 18]	0.8750
Model 7	num_conv_layers=4, activation=Tanh, pooling=Max, filter_size=5, num_filters=[6, 16]	0.8850
🚀 How to Run

Clone the repository:

git clone https://github.com/your-username/lenet5-fashionmnist-experiments.git
cd lenet5-fashionmnist-experiments


Install dependencies:

pip install torch torchvision matplotlib pandas


Open the notebook and run all cells:

jupyter notebook lenet5_fashionmnist_experiments.ipynb

📊 Conclusion

Model 5, with 4 convolution layers, ReLU activation, average pooling, and [8, 18] filters, produced the highest validation accuracy (90.37%), outperforming other tested configurations.
