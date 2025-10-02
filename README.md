# NVIDIA DLI: "Building a Brain in 10 Minutes"

I completed NVIDIA’s  hands-on tutorial **"Building a Brain in 10 Minutes"**, a beginner-friendly introduction to artificial neural networks using **TensorFlow** and **Google Colab**.

🔗 **Official Resource**: [NVIDIA Deep Learning Institute – Getting Started with Deep Learning](https://www.nvidia.com/en-us/training/)

---

## 🎯 What This Notebook Does
- Loads the **Fashion MNIST dataset** (70,000 grayscale images of clothing items)
- Builds a simple **neural network with just 10 neurons**
- Trains the model on a **free GPU via Google Colab**
- Achieves ~80% accuracy in classifying items like T-shirts, sneakers, and ankle boots

---

## 💡 Key Concepts I Learned

### 🧠 Biological Inspiration
- Artificial neurons are inspired by biological ones: inputs → weights → activation → output
- Unlike real brains, current models ignore **timing** and **spiking behavior** — they use simplified math (like `y = w·x + b`)

### ⚙️ Technical Workflow
- **Flatten layer**: Converts 28×28 pixel images into a 784-length vector
- **Dense layer**: 10 output neurons (one per clothing class)
- **SparseCategoricalCrossentropy**: Loss function ideal for integer-labeled classification
- **Adam optimizer**: Automatically adjusts learning for faster convergence

### 📊 Training vs. Validation
- **Training data**: Used to "study" (like flashcards)
- **Validation data**: Used to "quiz" the model and prevent memorization (overfitting)

### 🚀 Why GPUs?
- Neural networks rely on **massive matrix multiplications**
- GPUs (originally for graphics) excel at parallel math → perfect for deep learning!

---

## 🤔 Reflections & Next Steps

This tiny model proves that **even simple neural networks can learn patterns** — but it’s far from perfect!  
- It confuses **shirts vs. T-shirts** (both label 0 and 6 look similar)
- Real-world models use **convolutional layers (CNNs)**, **more data**, and **regularization**

I’m excited to explore:
- Building deeper networks with hidden layers
- Using **callbacks** and **learning rate scheduling**
- Applying transfer learning with pre-trained models

---

## 🙏 Credit
All code and content are from **NVIDIA’s Deep Learning Institute (DLI)**.  
This repository is for **personal learning documentation only** — not for redistribution of NVIDIA’s materials.

> “The best way to learn AI is to build it.” – NVIDIA DLI
