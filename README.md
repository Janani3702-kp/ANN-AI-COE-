# Artificial Neural Network (ANN) for Binary Classification

## Project Overview

This project implements an Artificial Neural Network (ANN) using Python, TensorFlow, and Keras to perform binary classification on the Make Moons dataset. The model learns nonlinear patterns in the data and classifies observations into two different classes.

## Objectives

- Generate a synthetic dataset using `make_moons`.
- Visualize the distribution of the two classes.
- Preprocess and standardize input features.
- Build and train an ANN model.
- Evaluate the model using classification metrics.
- Visualize training accuracy, loss, and the decision boundary.

## Technologies Used

- Python
- NumPy
- Matplotlib
- Scikit-learn
- TensorFlow
- Keras
- Seaborn

## Dataset

The project uses the Make Moons dataset provided by Scikit-learn.

The dataset contains two interleaving half-moon-shaped classes, making it suitable for demonstrating nonlinear classification.

**Dataset Configuration**

- Number of Samples: 1,000
- Number of Classes: 2
- Number of Features: 2
- Noise Level: 0.2
- Training Data: 80%
- Testing Data: 20%

The dataset is generated directly in the notebook, so no external dataset download is required.

## Model Architecture

1. **Input Layer:** Accepts two numerical features.
2. **Hidden Layer 1:** Contains 16 neurons with ReLU activation.
3. **Hidden Layer 2:** Contains 8 neurons with ReLU activation.
4. **Output Layer:** Contains one neuron with sigmoid activation to predict the probability of the positive class.

## Training Configuration

- Optimizer: Adam
- Loss Function: Binary Cross-Entropy
- Evaluation Metric: Accuracy
- Number of Epochs: 100
- Batch Size: 32
- Validation Split: 20% of the training data
- Classification Threshold: 0.5

## Project Workflow

1. Import the required libraries.
2. Generate the Make Moons dataset.
3. Visualize the dataset using a scatter plot.
4. Split the dataset into training and testing sets.
5. Standardize the input features using `StandardScaler`.
6. Build the ANN model.
7. Compile the model with the Adam optimizer and binary cross-entropy loss.
8. Train the model using the training dataset.
9. Evaluate the model using the testing dataset.
10. Display the confusion matrix and classification report.
11. Plot training and validation accuracy and loss.
12. Visualize the learned decision boundary.

## Installation

Install the required dependencies:

```bash
pip install numpy matplotlib scikit-learn seaborn tensorflow
```

## How to Run

1. Open the notebook in Google Colab or Jupyter Notebook.
2. Run the notebook cells from top to bottom.
3. Review the generated dataset visualization.
4. Observe the model training progress.
5. Check the test accuracy and loss.
6. Review the confusion matrix and classification report.
7. Examine the accuracy, loss, and decision-boundary plots.

## Output

The notebook produces the following outputs:

- Visualization of the Make Moons dataset
- ANN model summary
- Training and validation accuracy graph
- Training and validation loss graph
- Test loss and accuracy
- Confusion matrix
- Precision, recall, and F1-score
- Decision-boundary visualization

The actual evaluation scores depend on the training run and environment.

## Limitations

- The project uses a synthetic dataset rather than real-world data.
- The model is designed for a simple binary classification problem.
- Performance depends on the network architecture and training configuration.
- The results may vary slightly across training runs.

## Future Enhancements

- Experiment with different numbers of hidden layers and neurons.
- Tune the learning rate and batch size.
- Compare ANN performance with logistic regression and other classifiers.
- Add early stopping to reduce unnecessary training.
- Save the trained model for future predictions.
- Create an interface for classifying new data points.

## Author

**Your Name**

*An educational project demonstrating ANN-based binary classification using TensorFlow and Keras.*
