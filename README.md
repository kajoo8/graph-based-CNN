# julia-graph-based-cnn
An implementation and performance comparison of an automatic differentiation algorithm in Julia against PyTorch in a Convolutional Neural Network.

## Project Overview

This project demonstrates an automatic differentiation algorithm implemented from scratch in Julia, applied to a convolutional neural network (CNN). The backward propagation process leverages a computation graph to compute gradients necessary for training the network. The same CNN architecture was then built using the PyTorch library to perform comparative tests evaluating speed and efficiency.

The goal is to explore the effectiveness of Julia's automatic differentiation in neural network training and benchmark it against the well-established PyTorch framework.

## Repository Contents

- **Julia implementation:** Source code implementing the CNN and automatic differentiation algorithm built from the ground up.
- **PyTorch implementation:** The same CNN architecture recreated in PyTorch for benchmarking. The PyTorch one is available in the directory ```Previous_versions```.
- **Performance analysis:** Comparative results on speed and computational efficiency between Julia and PyTorch implementations, located in the ```report_eng.pdf``` file.

## Key Insights

- The Julia automatic differentiation model successfully computes gradients via a computation graph enabling training from scratch.
- PyTorch implementation serves as a reliable baseline for performance comparison.
- Initial benchmarking shows differences in speed and efficiency, providing valuable insights into deploying custom autodiff in Julia versus using PyTorch's optimized libraries. It also shows differences between fast-fourier transform and standard convolution computation.
- This project demonstrates the feasibility and challenges of building deep learning components in Julia without relying on existing automatic differentiation libraries.
- Time needed to train one epochs is 68 seconds for Julia's implementation, and 160 seconds for PyTorch one.
- Each forward and backward pass in Julia's implementation was also measured before and after improving the implementation. The results are presented in the table below.
<p align="center">
<img width="535" height="272" alt="image" src="https://github.com/user-attachments/assets/779a53be-01d7-4a08-b060-d771578cffdb" />
</p>

---
