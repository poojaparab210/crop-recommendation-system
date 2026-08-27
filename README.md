Crop Recommendation System

A machine learning web application that recommends the optimal crop to cultivate based on soil composition and climate conditions. Built to help simulate data-driven decision-making for farmers, replacing guesswork with a model trained on real agricultural data.

Overview

The system takes soil and climate inputs (e.g., nitrogen, phosphorus, potassium levels, temperature, humidity, rainfall) through a simple web form and returns a predicted crop recommendation in real time.

Features
Data cleaning and preprocessing of a large agricultural dataset (handling missing values and outliers)
Exploratory data analysis to identify relationships between soil, climate, and yield
Feature engineering to improve model input quality
Supervised classification model (built with Scikit-learn) trained to recommend optimal crops
Model evaluation using accuracy as the core performance metric, with iterative tuning to reduce prediction error
Data visualizations (Matplotlib/Seaborn) to surface trends in soil, climate, and yield data
Django-based web interface allowing users to input data via a form and receive instant predictions
Tech Stack
Language: Python
Data Processing & Model Development: Google Colab (Pandas, NumPy)
Machine Learning: Scikit-learn
Visualization: Matplotlib, Seaborn
Web Framework: Django (local development)
Frontend: HTML, CSS
How It Works
Data cleaning, exploratory analysis, feature engineering, and model training were done in Google Colab
The trained model was exported and integrated into a local Django application
User enters soil and climate parameters through a web form
Input is passed to the trained classification model
Model predicts the most suitable crop based on the given conditions
Result is displayed back to the user through the Django interface
Project Structure
crop-recommendation-system/
├── colab_notebook/      # Data cleaning, EDA, and model training (Google Colab)
│   └── crop_model_training.ipynb
├── model/               # Exported trained model file
├── crop_app/            # Django application (views, forms, templates)
├── data/                # Dataset used for training
├── requirements.txt     # Python dependencies
└── README.md
Setup & Installation

1. Model Training (Google Colab) Open colab_notebook/crop_model_training.ipynb in Google Colab to view the full data cleaning, EDA, and model training process.

2. Web Application (Django, local)

bash
# Clone the repository
git clone <your-repo-url>
cd crop-recommendation-system

# Install dependencies
pip install -r requirements.txt

# Run the Django development server
python manage.py runserver

Then visit http://127.0.0.1:8000/ in your browser.

What I Learned

This project gave me hands-on experience with the full data science pipeline — from raw, messy data to a deployed, usable application. It also taught me how to bridge machine learning with a functional web interface, going beyond a notebook-only model to something a real user could actually interact with.

Future Improvements
Add more evaluation metrics (precision, recall, confusion matrix) for deeper model insight
Expand the dataset to cover more regions and crop varieties
Deploy the application to a live hosting platform
Author

Pooja Parab poojaparab4752@gmail.com
