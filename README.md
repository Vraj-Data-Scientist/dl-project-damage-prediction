Car Damage Prediction
# DL Project Damage Prediction

This repository demonstrates a deep learning approach for damage prediction using various convolutional neural network (CNN) architectures and transfer learning techniques. The experiments in this project explore different models and techniques, culminating in a fine-tuned ResNet model with improved accuracy.

## Project Overview

The project follows these steps:

1. **Load the Dataset**  
   The dataset is loaded and preprocessed to serve as input for training.

2. **Baseline CNN**  
   - A simple CNN model was implemented.  
   - **Accuracy Achieved:** 57.74%

3. **CNN with Regularization**  
   - Regularization techniques were applied to the baseline CNN to address overfitting.  
   - **Accuracy Achieved:** 50.43%

4. **Transfer Learning with EfficientNet**  
   - EfficientNet was used for transfer learning to leverage pre-trained features.  
   - **Accuracy Achieved:** 65.74%

5. **ResNet Fine-Tuning**  
   - A pre-trained ResNet model was fine-tuned for the task.  
   - **Accuracy Before Hyperparameter Tuning:** 76.70%

6. **Hyperparameter Tuning**  
   - Hyperparameter tuning was performed in a separate notebook.  
   - **Best Parameters Identified:**  
     - Dropout Rate: **0.2**  
     - Learning Rate: **0.005**

7. **Final Model**  
   - The final tuned ResNet model achieved an overall accuracy of **80.87%**.

## Repository Structure


## Getting Started

### Prerequisites

- Python 3.8 or later
- pip

### Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/Vraj-Data-Scientist/dl-project-damage-prediction.git
   cd dl-project-damage-prediction/streamlit-app

```bash
pip install -r requirements.txt


