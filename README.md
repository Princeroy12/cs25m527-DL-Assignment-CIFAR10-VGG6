# cs25m527-DL-Assignment-CIFAR10-VGG6
Deep Learning Assignment - VGG6 on CIFAR-10

Roll Number: CS25M527
 Course: Deep Learning
 Assignment: VGG6 Model Training and Evaluation on CIFAR-10 Dataset

Contents

DL_Assignment_Report.pdf - Complete assignment report
results_summary.png - Results summary visualization
training_curves.png - Training curves for all configurations
best_model.pth - Trained model weights (best configuration)

Google Colab Notebook

Full training code and experiments:
 https://colab.research.google.com/drive/1mKrtJVVcuMmyEkljlhjE5X6wFk6qUcYd?usp=sharing

W&B Project

Training logs and metrics:
 https://wandb.ai/royprincejmp-iit-madras/uncategorized

Best Configuration

Activation: GELU
Optimizer: Adam
Learning Rate: 0.001
Batch Size: 128
Best Validation Accuracy: 90.98%
* on retrain to get best model accuracy was 88.52%


Setup and Reproducibility

Environment

Platform: Google Colab (GPU: Tesla T4)
Python: 3.10
PyTorch: 2.0+
CUDA: Enabled

Dependencies

bash pip install torch torchvision wandb matplotlib

Running the Code

1. Open the Colab notebook (link above)
2. Runtime → Change runtime type → GPU
3. Run all cells in order
4. Training takes ~2 hours for 8 configurations (25 epochs each)

Reproducibility

Random seed: 42 (set for PyTorch, NumPy, Python)
CIFAR-10 data downloaded automatically via torchvision
All hyperparameters logged to W&B

File Structure

├── vgg6_cifar10_training.ipynb # Main training notebook ├── DL_Assignment_Report.pdf # Assignment report ├── results_summary.png # Configuration comparison ├── training_curves.png # Loss/accuracy plots └── W&B visualization images # 6 plots from Weights & Biases

Trained Configurations

8 configurations tested with combinations of:

Activations: ReLU, GELU, Tanh
Optimizers: Adam, SGD, RMSprop
Learning rates: 0.001, 0.0001
Batch sizes: 64, 128

