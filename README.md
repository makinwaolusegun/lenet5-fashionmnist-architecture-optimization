# lenet5-fashionmnist-architecture-optimization
This project implements a LeNet-5 convolutional neural network trained on the FashionMNIST dataset using PyTorch.
Multiple experiments were conducted by varying convolution layers, pooling types, activation functions, and filter counts to optimize performance.
The best configuration achieved a validation accuracy of 90.37%.

📊 Conclusion

Model 5, with 4 convolution layers, ReLU activation, average pooling, and [8, 18] filters, produced the highest validation accuracy (90.37%), outperforming other tested configurations.

🚀 How to Run

Clone the repository:

git clone https://github.com/your-username/lenet5-fashionmnist-experiments.git
cd lenet5-fashionmnist-experiments


Install dependencies:

pip install torch torchvision matplotlib pandas


Open the notebook and run all cells:

jupyter notebook lenet5_fashionmnist_experiments.ipynb


