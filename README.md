# IPL Score Prediction using Deep Learning 🏏

This project leverages a deep learning approach to predict the total score of an IPL team during a cricket match. By using match-related data and encoding techniques, the model accurately forecasts the total score for given inputs.

## 🚀 Project Overview

This project involves:
- **Data Preprocessing**: Cleaning and encoding IPL match data for deep learning compatibility.
- **Deep Learning Model**: A neural network built with Keras and TensorFlow to predict match scores.
- **Interactive UI**: A user-friendly widget-based interface for selecting match details and generating predictions.

## 📊 Dataset

The project uses a dataset of IPL matches containing features like:
- Venue
- Batting Team
- Bowling Team
- Striker
- Bowler
- Total Score

### Example Data:
| Venue                  | Batting Team           | Bowling Team         | Striker       | Bowler       | Total |
|------------------------|------------------------|----------------------|---------------|--------------|-------|
| M Chinnaswamy Stadium | Kolkata Knight Riders | Royal Challengers   | SC Ganguly    | P Kumar      | 222   |

## 🧠 Model Architecture

- **Input Layer**: Accepts preprocessed match data.
- **Hidden Layers**: Two dense layers with 512 and 216 neurons, ReLU activation.
- **Output Layer**: A single neuron with linear activation for regression.

The model uses the **Huber loss function** for better handling of outliers and the Adam optimizer.

### Training Details:
- **Epochs**: 50
- **Batch Size**: 64
- **Validation Loss**: ~19.05 (after training)

## 🛠️ Features

1. **Match Data Preprocessing**:
   - Label Encoding for categorical variables.
   - Min-Max Scaling for numerical features.

2. **Interactive Prediction System**:
   - Dropdown widgets for user input.
   - Generates predictions instantly.

3. **Performance Metrics**:
   - Mean Absolute Error (MAE): ~19.54

## 🔧 How to Use

### Prerequisites:
- Python 3.7+
- TensorFlow 2.0+
- Jupyter Notebook

### Steps:
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/ipl-score-prediction.git
   cd ipl-score-prediction
