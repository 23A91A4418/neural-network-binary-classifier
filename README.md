# Deep Learning Binary Classification using TensorFlow & Keras

## Project Overview
This project demonstrates an end-to-end deep learning workflow for solving a binary classification problem using TensorFlow and the Keras API.

The objective is to design, train, and evaluate a neural network while applying proper preprocessing, validation strategies, and performance evaluation techniques.

---

## Objectives

- Perform Exploratory Data Analysis (EDA)
- Implement a robust preprocessing pipeline
- Build a Sequential Neural Network using Keras
- Apply EarlyStopping and ModelCheckpoint callbacks
- Evaluate the final model using multiple performance metrics

---

## Dataset

The Breast Cancer dataset from Scikit-learn is used.

- Total Samples: 569
- Features: 30 numerical features
- Target Classes:
  - 0 → Malignant
  - 1 → Benign

---

## Data Preprocessing

The following preprocessing steps were applied:

1. Checked for missing values
2. Scaled numerical features using StandardScaler
3. Split dataset into:
   - 60% Training set
   - 20% Validation set
   - 20% Test set
4. Stratified sampling used to maintain class balance

---

## Neural Network Architecture

The model was built using the Sequential API.

Architecture:

- Input Layer → 30 features
- Dense Layer (ReLU)
- Dense Layer (ReLU)
- Dense Layer (ReLU)
- Output Layer → 1 neuron (Sigmoid activation)

### Activation Functions

- ReLU used for hidden layers to introduce non-linearity
- Sigmoid used for output layer to produce probability values for binary classification

---

## Model Training

The model was compiled with:

- Loss Function: Binary Crossentropy
- Optimizer: Adam
- Metric: Accuracy

### Callbacks Used

- EarlyStopping  
  Stops training when validation loss stops improving and prevents overfitting.

- ModelCheckpoint  
  Saves the best performing model automatically.

---

## Model Evaluation

The trained model was evaluated on the unseen test dataset using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score

Additional visualizations:

- Training vs Validation Loss Curve
- Training vs Validation Accuracy Curve
- Confusion Matrix
- ROC Curve

---

## Results

The neural network achieved strong classification performance exceeding the required threshold.

Typical results:

- Accuracy: ~0.96+
- F1-Score: ~0.95+
- ROC-AUC: ~0.98+

---

## Technologies Used

- Python
- TensorFlow / Keras
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## Conclusion

This project successfully demonstrates the complete deep learning workflow for binary classification.  
The use of proper preprocessing, validation strategies, and performance metrics ensures a reliable and well-generalized model.

---

## Future Improvements

- Hyperparameter tuning
- Adding Dropout layers
- Trying different optimizers
- Applying cross-validation
- Testing on larger datasets
