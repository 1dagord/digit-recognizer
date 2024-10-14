Digit Recognizer

Inputs: 60000 28x28-pixel images of handwritten digit
Outputs: One-hot encoded digit 0-9

Data Validation:
Training/validation sets assigned using 10-Fold Cross-Validation


Model Architecture:
- Convolution Layer	5x5 kernel
- Max Pooling Layer	2x2 pool size
- Dropout Layer 1 	25% chance of drop
- Hidden Layer 1 	initialized with Glorot Normal values, activated with ReLU
- Dropout Layer 2	50% chance of drop
- Hidden Layer 2	initialized with Glorot Normal values, activated with Softmax


Model Evaluation:
Model evaluated using Categorical Cross Entropy Loss function


Results:
Average Validation Accuracy:	88.24%
Test Accuracy:			98.46%