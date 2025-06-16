# 🧠 Dynamic Neural Network (Python From Scratch)

This project implements a fully customizable **Feedforward Neural Network** from scratch in Python — no external libraries like TensorFlow or PyTorch required. It allows you to define the number of layers, nodes, learning rate, and test it with new inputs.

---

## 📌 Features

- ✅ Automatically detects input/output layer size from training data
- ✅ User-configurable or random hidden layers
- ✅ Sigmoid activation function + derivative
- ✅ Forward pass & backpropagation
- ✅ Tracks best weights & biases based on lowest SSE (Sum of Squared Errors)
- ✅ Accepts new inputs after training for prediction

---

# ⚙️ How It Works
# 🔧 Model Setup
Input & Output nodes are detected automatically

3 modes for hidden layers:

Manual: User defines exact number of layers and nodes

Random: User specifies max limits; structure is randomized

Default: 5 hidden layers, 3 nodes each

# 🔁 Training Phase
Forward pass using sigmoid activation

Backpropagation using gradient descent

Weights & biases are updated per epoch

Model saves best parameters with minimum SSE

# 🔮 Prediction Phase
Predicts outputs for all training inputs

Accepts new inputs interactively and outputs predictions

---

 # 🔢 Example Input Format
 training_data = [
    {"inputs": [0.2, 0.5, 0.9], "target": [1]},
    {"inputs": [0.1, 0.3, 0.6], "target": [0]},
    {"inputs": [0.7, 0.8, 0.2], "target": [1]},
]

----

# 🧪 Sample Console Output
Choose one of the following options for hidden layers:
1. Predefined hidden layer count
2. Randomized layers and nodes
3. Default: 5 hidden layers, 3 nodes each

Enter your choice (1, 2, or 3): 3
Enter the Learning Rate: 0.1
Enter number of epochs: 1000

Training completed!
Least SSE: 0.002194

Predicted outputs for trained inputs:
Input: [0.2, 0.5, 0.9] -> Predicted Output: [0.9712]


