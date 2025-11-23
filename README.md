# Fake News Detection System

A web-based machine learning system that detects whether news articles are fake or real using Natural Language Processing and classification algorithms.

## 🔹 Features

- **Text Preprocessing**: Advanced cleaning, stopword removal, and stemming
- **TF-IDF Vectorization**: Converts text into numerical features
- **Dual Classifiers**: Logistic Regression and Naive Bayes models
- **Web Interface**: Beautiful Flask-based UI for real-time predictions
- **Model Persistence**: Saves trained models using pickle
- **Responsive Design**: Modern, mobile-friendly interface

## 🔹 Quick Start

### Option 1: Automated Installation (Windows)
1. Double-click `install.bat` to install dependencies and setup
2. Double-click `run.bat` to start the web application

### Option 2: Manual Installation
1. Install Python 3.7 or higher
2. Install required packages:
```bash
pip install -r requirements.txt
```
3. Run setup:
```bash
python setup.py
```

## 🔹 Usage

1. **Train the model** (first time only):
```bash
python train_model.py
```

2. **Run the Flask application**:
```bash
python app.py
```

3. **Open your browser** and go to `http://localhost:5000`

## 🔹 Project Structure

```
fake-news-detection/
├── app.py                 # Flask web application
├── train_model.py         # Model training script
├── preprocessing.py       # Text preprocessing utilities
├── setup.py              # Setup and installation script
├── test_system.py        # System testing script
├── install.bat           # Windows installation script
├── run.bat               # Windows run script
├── models/               # Saved models directory
├── templates/            # HTML templates
│   ├── index.html        # Main page
│   ├── about.html        # About page
│   ├── 404.html          # Error page
│   └── 500.html          # Server error page
├── static/               # CSS and static files
│   └── style.css         # Main stylesheet
├── data/                 # Dataset directory
│   └── sample_dataset.csv # Sample news dataset
└── requirements.txt      # Python dependencies
```

## 🔹 Dataset

The system includes a sample dataset with 20 news articles. Each entry contains:
- `title`: News article title
- `text`: News article content  
- `label`: "FAKE" or "REAL"

You can replace `data/sample_dataset.csv` with your own dataset following the same format.

## 🔹 API Endpoints

- `GET /`: Main page with input form
- `POST /predict`: Predict if news is fake or real
- `GET /about`: About page with system information
- `GET /health`: Health check endpoint

## 🔹 Testing

Run the test suite to verify everything works:
```bash
python test_system.py
```

## 🔹 Technology Stack

- **Backend**: Python 3, Flask
- **Machine Learning**: scikit-learn, pandas, numpy
- **NLP**: NLTK for text processing
- **Frontend**: HTML5, CSS3, JavaScript
- **Styling**: Modern CSS with gradients and animations

## 🔹 Model Performance

The system trains two models and automatically selects the best performing one:
- **Logistic Regression**: High accuracy with good interpretability
- **Naive Bayes**: Fast predictions with reliable performance

## 🔹 Important Notes

- This system is for **educational and demonstration purposes**
- Always verify news through multiple reliable sources
- The model accuracy depends on the training data quality
- For production use, consider using larger, more diverse datasets

## 🔹 Troubleshooting

1. **ModuleNotFoundError**: Run `pip install -r requirements.txt`
2. **NLTK data missing**: Run `python setup.py`
3. **Model not found**: Run `python train_model.py` first
4. **Port already in use**: Change port in `app.py` or stop other Flask apps

## 🔹 Contributing

Feel free to submit issues, feature requests, or pull requests to improve the system!
