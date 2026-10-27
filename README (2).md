# Artificial Neural Network (ANN) for Binary Classification

An Artificial Neural Network (ANN) built with TensorFlow/Keras to classify the two interleaving half-moon classes in the synthetic **make_moons** dataset. The project demonstrates data visualization, preprocessing, model training, evaluation, and decision-boundary visualization.

## Project Overview

This project uses a feed-forward neural network to learn a nonlinear decision boundary for a binary classification problem.

### Objectives
- Generate and visualize a two-class dataset using `make_moons`.
- Split the dataset into training and testing sets.
- Standardize input features using `StandardScaler`.
- Build and train an ANN using TensorFlow/Keras.
- Evaluate predictions using accuracy, a confusion matrix, and a classification report.
- Plot training/validation accuracy and loss.
- Visualize the model's decision boundary.

## Technologies Used

- Python
- NumPy
- Matplotlib
- scikit-learn
- TensorFlow / Keras
- Seaborn

## Dataset

The dataset is generated locally with scikit-learn:

```python
X, y = make_moons(n_samples=1000, noise=0.2, random_state=42)
```

- **Samples:** 1,000
- **Classes:** 2
- **Features:** 2 numerical features
- **Noise:** 0.2
- **Train/test split:** 80% training, 20% testing

The dataset is synthetic, so no external dataset download is required.

## Neural Network Architecture

| Layer | Configuration |
|---|---|
| Input | 2 features |
| Hidden layer 1 | 16 neurons, ReLU activation |
| Hidden layer 2 | 8 neurons, ReLU activation |
| Output layer | 1 neuron, Sigmoid activation |

### Training Configuration

- **Optimizer:** Adam
- **Loss function:** Binary cross-entropy
- **Metric:** Accuracy
- **Epochs:** 100
- **Batch size:** 32
- **Validation split:** 20% of the training data
- **Classification threshold:** 0.5

## Project Workflow

1. Import the required libraries.
2. Generate and plot the `make_moons` dataset.
3. Split the data into training and testing sets.
4. Standardize the features.
5. Define and compile the ANN model.
6. Train the model and record its learning history.
7. Evaluate the model on the test set.
8. Print the confusion matrix and classification report.
9. Plot accuracy and loss curves.
10. Display the learned decision boundary.

## Installation

Install the dependencies:

```bash
pip install numpy matplotlib scikit-learn seaborn tensorflow
```

## How to Run

1. Download or clone this project.
2. Open `Untitled21.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.
3. Run the notebook cells from top to bottom.
4. Review the printed evaluation metrics and generated plots.

## Evaluation

The notebook reports:
- Test loss
- Test accuracy
- Confusion matrix
- Precision, recall, F1-score, and support for each class

The actual scores can vary slightly depending on the TensorFlow version and training environment. Use the results printed by your own run rather than assuming a fixed accuracy.

## Visualizations

The notebook produces:
- A scatter plot of the two moon-shaped classes
- Training and validation accuracy curves
- Training and validation loss curves
- The ANN's learned decision boundary

## Repository Structure

```text
AICOE-main/
├── README.md
└── Untitled21.ipynb
```

## Learning Outcomes

By completing this project, you can understand how to:
- Prepare and scale data for neural networks
- Build a simple feed-forward ANN
- Train a binary classifier with Keras
- Interpret classification metrics
- Identify learning trends using accuracy and loss plots
- Visualize nonlinear decision boundaries

## Future Improvements

- Add early stopping to reduce unnecessary training.
- Tune the number of layers, neurons, learning rate, and batch size.
- Compare the ANN with logistic regression and other classifiers.
- Add a saved-model export and a prediction example for new data.
- Set random seeds for more reproducible training.

## Author

**Your Name**

*Educational project demonstrating ANN-based binary classification.*
