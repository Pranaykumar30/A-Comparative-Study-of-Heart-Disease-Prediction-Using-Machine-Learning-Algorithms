# Heart Disease Prediction: A Comparative Study of Machine Learning Models

## Project Overview

This project aims to predict the likelihood of heart disease using various machine learning algorithms. We compare different models to identify the most accurate one and deploy it in a user-friendly web application. Users can enter personal health metrics and receive a risk assessment for heart disease.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Model Performance](#model-performance)
- [Contributing](#contributing)
- [License](#license)

## Features
- Predicts the likelihood of heart disease based on user inputs.
- Compares multiple machine learning algorithms (Random Forest, Decision Tree, Logistic Regression, K-Nearest Neighbors).
- Real-time risk prediction with user-friendly web interface using Flask.
- Interactive visualizations for prediction results (e.g., pie chart showing risk distribution).

## Installation

### Prerequisites
Ensure you have the following installed:
- Python 3.x
- pip (Python package manager)
- Git

### Setup
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/heart-disease-prediction.git
   cd heart-disease-prediction
   ```

2. **Create a Virtual Environment** (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate    # On macOS/Linux
   venv\Scripts\activate       # On Windows
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Load the Model**:
   Make sure to have the trained model file `best_model.pkl` in the project directory. This file contains the pre-trained machine learning model used for predictions.

5. **Run the Application**:
   ```bash
   python app.py
   ```
   The application should now be running at `http://127.0.0.1:5000`.

## Usage

1. **Navigate to the Web Application**:
   Open a web browser and go to `http://127.0.0.1:5000`.

2. **Enter Health Metrics**:
   On the prediction page, fill out the form with health metrics like age, cholesterol, blood pressure, etc.

3. **Submit for Prediction**:
   Click "Predict" to see the risk assessment, including a risk percentage and a high/low-risk message.

4. **Interpret Results**:
   The result page shows the predicted risk percentage along with a detailed message. A pie chart visualization displays the risk vs. no-risk distribution for easy interpretation.

## Project Structure

```plaintext
heart-disease-prediction/
├── app.py                 # Main application file
├── best_model.pkl         # Trained machine learning model
├── templates/
│   ├── index.html         # Homepage template
│   ├── predict.html       # Prediction input form template
│   └── result.html        # Result display template
├── static/
│   └── style.css          # CSS styling for the web app

```

## Technologies Used
- **Programming Language**: Python 3.x
- **Machine Learning**: sci-kit-learn
- **Web Framework**: Flask
- **Frontend**: HTML, CSS, JavaScript (with Chart.js for visualizations)
- **Data Processing**: Pandas, NumPy

## Model Performance
The project includes a comparative analysis of different machine-learning models. Below are the metrics for each model:

| Model                | Accuracy | Precision | Recall | F1 Score | AUC  |
|----------------------|----------|-----------|--------|----------|------|
| Random Forest        | 100%     | 100%      | 100%   | 100%     | 1.0  |
| Decision Tree        | 97.66%   | 100%      | 95.2%  | 97.5%    | 0.976|
| Logistic Regression  | 80.54%   | 76.6%     | 86.4%  | 81.2%    | 0.883|
| K-Nearest Neighbors  | 71.98%   | 71.2%     | 71.2%  | 71.2%    | 0.841|

## Contributing
Contributions are welcome! If you'd like to improve this project, please fork the repository and create a pull request. For major changes, please open an issue first to discuss your ideas.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/NewFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/NewFeature`)
5. Open a pull request

## License
This project is licensed under the MIT License.
