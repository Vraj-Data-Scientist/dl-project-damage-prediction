# DL Project Damage Prediction

This project implements a **Deep Learning Damage Prediction Model** that predicts the extent of damage (e.g., car damage) using convolutional neural networks (CNNs) and transfer learning techniques. The project explores multiple model architectures—from a baseline CNN to advanced transfer learning approaches—culminating in a fine-tuned ResNet model that achieved an accuracy of **80.87%**.

## 1. Project Overview

The model development process followed these steps:

- **Data Loading & Preprocessing:**  
  The dataset is loaded and preprocessed for model training.

- **Baseline CNN:**  
  A simple CNN model was implemented, achieving an accuracy of **57.74%**.

- **CNN with Regularization:**  
  Applying regularization techniques resulted in an accuracy of **50.43%**.

- **Transfer Learning with EfficientNet:**  
  Leveraging EfficientNet improved the accuracy to **65.74%**.

- **ResNet Fine-Tuning:**  
  A pre-trained ResNet model was fine-tuned, reaching an accuracy of **76.70%**.

- **Hyperparameter Tuning:**  
  Using a separate notebook for hyperparameter tuning, the best parameters for the ResNet model were identified:  
  - **Dropout Rate:** 0.2  
  - **Learning Rate:** 0.005  
  This tuning led to the final model accuracy of **80.87%**.

## 2. Project Structure

dl-project-damage-prediction/ ├── streamlit-app/ │ ├── app.py # Main Streamlit application file │ ├── model_helper.py # Helper functions for model loading and prediction │ ├── requirements.txt # Python dependencies for the project │ └── model/ │ └── saved_model.pth # Pre-trained model weights for ResNet ├── notebooks/ │ └── hyperparameter_tuning.ipynb # Notebook with hyperparameter tuning experiments └── README.md # Project documentation
