# NN_Model_with_TANH_Activation_on_IMDB_Dataset
Neural Network with TANH Activation – IMDB Sentiment Classification
- Overview
- This project implements a feedforward neural network for binary sentiment classification on the IMDB
dataset. The model and experiments explore the effects of activation functions, hidden layers, loss
functions, and regularization techniques.

- Dataset and Preprocessing
• Dataset: Keras IMDB (25,000 train / 25,000 test samples)
• Input Representation: Multi-hot encoded vectors (10,000 features)
• Output Labels: 0 = negative, 1 = positive
• Validation Split: 10,000 samples

- Model Configuration
• Hidden Layers: 2
• Units per Layer: 16
• Activation: Tanh
• Output Layer: Sigmoid
• Optimizer: RMSprop
• Loss Function: Binary Crossentropy
• Metric: Accuracy

- Key Insights
• Tanh activation provided consistent and smooth convergence.• Using two layers with 32 units achieved the best overall performance.
• MSE loss degraded performance compared to binary Crossentropy.
• Dropout and L2 regularization slightly improved validation stability.
• Early stopping around epoch 3 prevents overfitting and maximizes test accuracy.

- Final Performance
Test Accuracy: 0.8859
Best Epoch: 3
The model demonstrates that Tanh-based architectures can perform competitively on binary sentiment
classification when combined with regularization and careful tuning.
