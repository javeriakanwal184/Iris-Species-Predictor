**Assignment No. 2: Iris Species Predictor**

**Objective**

Train a Multi-Layer Perceptron (MLP) to classify Iris species and deploy it as an Android app.

**Files Included**

train_model.py: Python script for training the model.

iris_model.tflite: The trained model converted to TensorFlow Lite format.

screenshot.png: Screenshot of the working application.

**Sequence of Steps**

**1. Model Training**

Loaded the Iris dataset (150 samples, 4 features).

Preprocessed data using StandardScaler.

Built a Dense Neural Network with architecture: Input(4) -> Dense(8, ReLU) -> Dense(16, ReLU) -> Dense(3, Softmax).

Trained the model for 50 epochs using Adam optimizer.

Achieved high accuracy on the test set.

**2. TFLite Conversion**

Saved the trained Keras model.

Converted the model to .tflite format using TFLiteConverter.

Downloaded iris_model.tflite.

**3. Android Frontend Integration**

Developed a React Native (Expo) application.

Created a UI with 4 input fields for flower measurements.

Integrated the model weights and scaler parameters directly into the JavaScript logic for inference.

The app predicts the species (Setosa, Versicolor, Virginica) based on user input.

**Final Output**

See attached screenshot for the working application prediction
