#  Car Price Prediction using TensorFlow

This project builds and trains a **Neural Network** using **TensorFlow** to predict used car prices based on various features such as year, mileage, rating, horsepower, and more. It includes data preprocessing, normalization, model design, training, evaluation, and testing.
##  Project Structure

###  1. Task Understanding
- Understand the goal: Predict car prices using historical and categorical features.
- Explore the data and define the machine learning task clearly.

###  2. Data Preparation 
- Load and clean the dataset.
- Handle missing values and normalize features using TensorFlow preprocessing layers.

###  3. 5 Layer Neural Network Architecture
- 3 hidden with 128 nodes and relu activation function , 8 nodes in input layer and 1 node at output layer
- 
###  4. Error Sanctioning 
- Implement error metrics such as **Mean Absolute Error** (MAE) and **Root Mean Squared Error** (RMSE).
- Visualize the error trends during training.

###  5. Training and Optimization
- Build a **deep neural network** using `tf.keras.Sequential`.
- Use **Adam optimizer** and custom learning rates for training.

### 6. Performance Measurement
- Evaluate model performance using validation metrics.
- Display predictions vs actual values using plots.

###  7. Validation and Testing 
- Split data into training, validation, and test sets.
- Use early stopping and model checkpoints if necessary.

###  8. Corrective Measures 
- Tune hyperparameters.
- Add more layers, regularization, or modify learning rate for better results.

---
##  Model Summary

```python
model = tf.keras.Sequential([
    tf.keras.layers.InputLayer(input_shape=(8,)),
    tf.keras.layers.Normalization(),
    tf.keras.layers.Dense(128, activation="relu"),
    tf.keras.layers.Dense(128, activation="relu"),
    tf.keras.layers.Dense(128, activation="relu"),
    tf.keras.layers.Dense(1)
])

