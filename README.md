#  MNIST Deep Learning Project (CNN)

##  Overview
This project implements a Convolutional Neural Network (CNN) to classify handwritten digits using the MNIST dataset.

The goal is to compare two optimizers:
- Adam
- SGD

---

##  Dataset
- MNIST (from torchvision)
- 60,000 training images
- 10,000 testing images
- Image size: 28×28 grayscale

---

##  Model Architecture
Simple CNN:
- Conv Layer (32 filters)
- ReLU
- MaxPooling
- Conv Layer (64 filters)
- ReLU
- MaxPooling
- Fully Connected Layer (128 neurons)
- Output Layer (10 classes)

---

## Training Setup
- Loss Function: CrossEntropyLoss
- Epochs: 5
- Batch Size: 64

---

##  Optimizers
### Adam
- Learning Rate: 0.001

### SGD
- Learning Rate: 0.01

---

##  Results

### Adam
- Test Accuracy: 99.15%

### SGD
- Test Accuracy: 96.99%

---

##  Comparison Table

| Optimizer | Accuracy |
|------------|----------|
| Adam       | 99.15%   |
| SGD        | 96.99%   |

---

##  Conclusion
- Adam performs better and converges faster.
- SGD is slower but still gives good results.

---

##  How to Run
```bash
pip install torch torchvision
python main.py
