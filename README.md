## Deep Learning with TensorFlow
The goal was to build a neural network in TensorFlow and tune it to get the best results on a binary classification problem.

  ### What the project does

  An employee attrition dataset was used to predict whether an employee will leave
  the company (Attrition: yes or no). Started with a very simple model and kept
  improving it by changing one thing at a time, like the number of epochs, layers,
  neurons, learning rate, and the activation function.

  ### Best model

  After testing a bunch of options, the model with a sigmoid output layer worked the best.

  | Setting | Value |
  | --- | --- |
  | Hidden layer | 1 Dense layer, 3 neurons |
  | Output layer | Dense(1), sigmoid |
  | Loss | Binary Crossentropy |
  | Optimizer | SGD, learning rate 0.01 |
  | Epochs | 100 |
  | Batch size | 32 |
  | Training accuracy | 0.894 |
  | Test accuracy | 0.896 |

  The biggest improvement came from adding the sigmoid activation. It dropped the loss from about 2.0 down to 0.28.

  ### Files in this repo

  - `employee_attrition.csv` - the dataset
  - `deep-learning-with-tensorflow.ipynb` - the main notebook with all works
  - `best-model-hyperparameters-and-loss-accuracy-plot.pdf` - a short conclusion to list the best model hyper parameters achieved in a table with its loss and accuracy plot

#### Featured by: Ngan Nguyen
