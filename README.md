# Audiobook Customer Purchase Prediction

## Project Overview

This project aims to predict whether a customer will make another purchase based on audiobook data. The model is built using a dataset of customer information and audiobook interactions. It leverages machine learning techniques to classify whether a customer will "buy again" or "not buy again." Key features are extracted and preprocessed before feeding them into the model, and the model's performance is evaluated based on accuracy.

## Table of Contents

- [Project Overview](#project-overview)
- [Data Preprocessing](#data-preprocessing)
- [Modeling](#modeling)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [Contributing](#contributing)
- [Contact](#contact)

## Data Preprocessing

1. **Dataset**: The dataset contains multiple customer records with features like previous interactions, completion rates, and other relevant audiobook-related data.
   
2. **Balanced Dataset**: To avoid bias in predictions, the dataset was balanced by removing extra samples where the customer did not make a repeat purchase.

3. **Scaling**: The features were scaled using `preprocessing.scale()` to standardize the data before feeding it into the model.

4. **Data Split**: The data was split into training, validation, and testing sets with an 80-10-10 ratio.

## Modeling

The model is a neural network implemented using TensorFlow/Keras with the following architecture:
- Input Layer: 10 input features.
- Hidden Layers: Three hidden layers with `ReLU` and `tanh` activations.
- Output Layer: A softmax layer for binary classification ("Buy" or "Not Buy").

### Model Training:
The model was compiled using the `Adam` optimizer and `sparse_categorical_crossentropy` loss function. Early stopping was employed to prevent overfitting.

## Results

The final model achieved:
- **Test Accuracy**: 92.24%

### Prediction Example:
After training, the model can predict whether a customer will make another purchase or not based on customer data.

## Technologies Used

- **Python**: For data processing and model building.
- **NumPy**: For numerical operations.
- **TensorFlow/Keras**: For building and training the neural network.
- **Scikit-learn**: For preprocessing and performance metrics.
- **Jupyter Notebook**: For developing and visualizing the process.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/AmaanP314/audiobook-prediction.git
   cd audiobook-prediction

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt

3. Run the Jupyter notebook to train the model and make predictions:
   ```bash
   jupyter notebook audiobook_prediction.ipynb

## Contributing
Contributions are welcome! Feel free to fork the repository and submit a pull request with any suggestions or improvements.

## Contact
Amaan Poonawala - [GitHub](https://github.com/AmaanP314) | [LinkedIn](https://www.linkedin.com/in/amaan-poonawala/)
