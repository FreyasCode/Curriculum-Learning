# 🧠 Curriculum Learning in Neural Networks: A Neurobiological Perspective

This repository contains the code and experimental results for our project exploring **curriculum learning** in neural networks through a biologically inspired lens. Our work was conducted as part of the **Computational Neuroscience** course at the University of Waterloo.

We examine how **training data ordering** (easy-to-hard vs. random) and **biologically plausible activation functions** (Sigmoid vs. ReLU/Softmax) influence learning dynamics, generalization, and convergence in neural models like perceptrons and multilayer perceptrons (MLPs).

---

## 📜 Project Overview

**Title:** Curriculum Learning in Neural Networks: A Neurobiological Perspective on Model Performance  
**Authors:** [Freya Zhang](mailto:freya.zhang@uwaterloo.ca), [Toshani Nath](mailto:t2nath@uwaterloo.ca)  
**Institution:** University of Waterloo, Cheriton School of Computer Science

**Paper:** [Read the full report (PDF)](https://drive.google.com/file/d/11a0c3DmdiNyFx8tfXJHoyOZBqEqzap1F/view?usp=sharing)  
**Conference Format:** NeurIPS 2020 style

---

## 🧪 Research Questions

- Does training from easier to harder data (curriculum learning) improve model performance compared to random ordering?
- Do more biologically plausible models (e.g., sigmoid activations) benefit more from curriculum learning?
- How does curriculum learning affect convergence speed and test accuracy across different architectures?

---

## 🧰 Methods

We used:

- **Models:** Single-layer Perceptron, 3-layer MLP  
- **Activation Functions:** ReLU, Sigmoid (biologically plausible), Softmax  
- **Dataset:** MNIST, with added Gaussian noise to create five difficulty levels  
- **Training Regimes:** Random vs. Forward Curriculum (easy → hard)  
- **Metrics:** Accuracy, loss, convergence rate, stability across epochs

---

## 📊 Key Findings

- **Sigmoid MLP + Curriculum Learning** achieved highest test accuracy (88.3%) and best convergence behavior.
- **ReLU and Softmax models** suffered from overfitting under curriculum learning unless learning rates were lowered.
- **Perceptron** model showed **no benefit** from curriculum learning—simpler models may lack capacity to benefit from structured training.
- Lowering learning rate (e.g., 0.001) helped convergence for ReLU/Softmax, but **did not improve generalization**.

---
