# Rainfall Prediction Project

A machine learning web application that predicts rainfall occurrence based on various meteorological features using MLflow for model management and Flask for deployment.

## 📷 Screenshots

![Prediction Result](https://github.com/Manish-Kumar24/Rainfall-Prediction/blob/main/assets/Main%20Prediction%20Interface.png)
*Main prediction interface*

![Web Interface](https://github.com/Manish-Kumar24/Rainfall-Prediction/blob/main/assets/prediction%20result.png)
*Example of a prediction result*

## 📋 Overview

This project implements a rainfall prediction system using machine learning techniques. It uses MLflow for experiment tracking and model management, and provides a web interface built with Flask for making predictions.

## 🚀 Features

- Real-time rainfall prediction based on meteorological data
- Web-based user interface for easy interaction
- MLflow integration for model versioning and management
- Production-ready model deployment
- Error handling and user feedback

## 🛠️ Technologies Used

- Python
- Flask
- MLflow
- Pandas
- Scikit-learn
- HTML/CSS

## 📁 Project Structure

```
rainfall-prediction/
│
├── assets/
│   ├── prediction result.png
│   └── Main Prediction Interface.png
│
├── mlruns/
│   ├── .trash/
│   ├── 0/
│   └── models/
│       ├── rainfall-prediction-production/
│       └── Random Forest Model Data/
│
├── templates/
│   └── index.html
│
├── app.py
├── Rainfall Prediction Using Python & MLFLOW.ipynb
├── Rainfall.csv
└── requirements.txt
```

## 🔧 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Manish-Kumar24/Rainfall-Prediction.git
   cd Rainfall-Prediction
   ```

2. Create a virtual environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

## 💻 Usage

1. Start the MLflow tracking server:
   ```bash
   mlflow server --host 127.0.0.1 --port 5000
   ```

2. In a new terminal, run the Flask application:
   ```bash
   python app.py
   ```

3. Open your web browser and navigate to:
   ```
   http://localhost:8080
   ```

## 📊 Input Features

The model accepts the following meteorological features:
- Pressure (hPa)
- Dewpoint (°C)
- Humidity (%)
- Cloud Cover (oktas)
- Sunshine (hours)
- Wind Direction (degrees)
- Wind Speed (km/h)

## 🔄 Model Information

The project uses a Random Forest classifier trained on historical weather data. The model is registered in MLflow with the name "rainfall-prediction-production" and is versioned for production use.

## 🚦 Model Deployment

The application automatically loads the production model marked as "champion" from MLflow. The model version can be updated through MLflow without changing the application code.

## 🛟 Error Handling

The application includes comprehensive error handling for:
- Invalid input values
- Model loading issues
- Prediction errors

## 📝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Authors

- Manish Kumar - *Initial work*

## 🙏 Acknowledgments

- Any third-party resources or inspirations
