## ResNet-Based Image Classification

## Overview
This project implements a deep learning model based on the **ResNet (Residual Network) architecture** for image classification. The model leverages residual blocks to improve gradient flow, making it more efficient in training deep neural networks.

## Architecture
The implemented architecture follows a ResNet-style design with the following key components:
- **Conv2D (64) + BatchNorm2D + ReLU** as the initial feature extractor.
- **Residual Blocks** with increasing channel sizes to capture hierarchical features.
- **Adaptive Average Pooling (1x1)** to reduce dimensionality.
- **Fully Connected Layer (256 → 10)** for final classification.

## Installation
To run this project, install the required dependencies:
```bash
pip install torch torchvision numpy matplotlib
```

## Usage
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <project_folder>
   ```
2. Run the training script:
   ```bash
   python train.py
   ```
3. Evaluate the model:
   ```bash
   python evaluate.py
   ```

## Dataset
The model is trained on a standard image dataset such as CIFAR-10. Modify `dataset.py` to use a different dataset.

## Model Summary
The implemented architecture is inspired by ResNet and supports residual learning. The skip connections help mitigate vanishing gradients, improving deep network performance.

## Contributing
Feel free to submit pull requests for improvements or additional features.

## License
This project is licensed under the MIT License.
