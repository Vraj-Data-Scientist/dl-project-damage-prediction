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

```plaintext
dl-project-damage-prediction/
├── streamlit-app/
│   ├── app.py                # Main Streamlit application file
│   ├── model_helper.py       # Helper functions for model loading and prediction
│   ├── requirements.txt      # Python dependencies for the project
│   └── model/
│       └── saved_model.pth   # Pre-trained model weights for ResNet
├── notebooks/
│   └── damage_prediction.ipynb
│   └── hyperparameter_tuning.ipynb  # Notebook with hyperparameter tuning experiments
└── README.md                 # Project documentation
```

## 3. Features

- **Deep Learning-Based Damage Prediction:**  
  Utilizes CNNs and transfer learning for accurate damage prediction.

- **Model Experimentation:**  
  Compares different approaches (baseline CNN, regularized CNN, EfficientNet, ResNet) with detailed performance metrics.

- **Hyperparameter Tuning:**  
  Optimizes the ResNet model with the best parameters (Dropout Rate: 0.2, Learning Rate: 0.005) for enhanced accuracy.

- **Interactive Web Interface:**  
  A Streamlit web app allows users to upload images and get real-time damage predictions.



## 4. Installation Instructions

```bash

git clone https://github.com/Vraj-Data-Scientist/dl-project-damage-prediction.git
cd dl-project-damage-prediction/streamlit-app

python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

pip install -r requirements.txt

streamlit run app.py

```

## 5. Contributions

We welcome contributions from the community! If you'd like to improve the model or add new features, feel free to fork this repository and submit a pull request.


## Dataset Citation

This project uses a dataset provided by Codebasics as part of the Codebasics Data Science Bootcamp. The dataset is not included in this repository due to usage restrictions.

### Citation

If you would like to use the dataset, please reference it as follows:

```markdown
Codebasics. (n.d.). Dataset from the Codebasics Data Science Bootcamp. Retrieved from [Codebasics](https://codebasics.io/)

