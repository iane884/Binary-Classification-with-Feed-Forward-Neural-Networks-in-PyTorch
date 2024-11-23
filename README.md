# CBinary-Classification-with-Feed-Forward-Neural-Networks-in-PyTorch

## Project Overview
In this project, we implemented a Feed-Forward Neural Network (FFNN) for binary classification tasks on datasets like XOR, center_surround, two_gaussians, and spiral. We used PyTorch to train the model with two different loss functions: Multi-Class Cross Entropy (MCE) and Mean Squared Error (MSE). The goal was to tune the model, visualize the decision boundaries, and explore the effects of regularization.

## Steps Completed

### 1. **FFNN with MCE Loss**
- Built a simple FFNN with one hidden layer.
- Experimented with different numbers of hidden nodes (k = 2, 3, 5, 7, 9).
- Used MCE loss for training.
- Plotted the learning curves and decision boundaries.
- Evaluated accuracy on the test set.

### 2. **FFNN with MSE Loss**
- Used MSE loss instead of MCE.
- Applied a sigmoid function for the output layer and thresholded predictions at 0.5.
- Plotted results like the learning curves and decision boundaries.

### 3. **Manual Gradients and Updates**
- Manually calculated gradients and updated weights without using automatic differentiation from PyTorch.
- Verified results by comparing with PyTorch's built-in gradients.

### 4. **Regularization**
- Added two regularizers:
  1. Minimize the norm of the input layer's weight matrix.
  2. Encourage orthogonality in the hidden layer’s weight matrix.
- Compared regularized and unregularized models using the XOR dataset.

## Hyperparameters Used:
- **Learning Rate:** 0.01
- **Epochs:** 100
- **Batch Size:** 32
- **Optimizer:** Adam
- **Hidden Layer Nodes:** 3
- **Activation Function:** LeakyReLU
- **Loss Function:** Cross-Entropy Loss (for MCE)

## Results:
- **Accuracy:** Calculated the accuracy on the test set.
- **Learning Curves:** Plotted the loss for training and validation over epochs.
- **Decision Boundaries:** Visualized how the model classifies the data.

## Conclusion:
We successfully built and trained FFNN models for binary classification. By experimenting with different loss functions, the number of hidden nodes, and regularization techniques, we learned how each factor affects the model’s performance. This helped us understand how to optimize and regularize neural networks for classification tasks.

