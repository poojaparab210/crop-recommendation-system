# 🌱 Crop Recommendation System

A Machine Learning project that recommends suitable crops based on soil nutrient levels and climatic conditions. Built using Python, Scikit-learn, and Django, the project combines data preprocessing, exploratory data analysis (EDA), classification, and web development to demonstrate an end-to-end machine learning application for agriculture.

The system analyses agricultural input features and predicts a suitable crop category, demonstrating how machine learning can support data-driven crop selection.

## Project Overview

Selecting a suitable crop depends on soil composition and environmental conditions. This project uses a supervised machine learning classification approach to predict crop recommendations from agricultural data.

The project includes two main components:

- **Machine Learning Pipeline:** Data cleaning, exploratory data analysis, feature preparation, model training, and evaluation using Scikit-learn.
- **Crop Recommendation Web Application:** A Django-based interface that accepts agricultural input values and displays the model's crop prediction.

The project was developed to explore how machine learning can be applied to agricultural decision-support systems.

## Key Features

### Data Analysis and Machine Learning

- Data cleaning and preprocessing using Pandas and NumPy.
- Exploratory data analysis to examine agricultural data distributions and patterns.
- Analysis of relationships between soil nutrients and climatic variables.
- Data visualization using Matplotlib and Seaborn.
- Supervised classification using Scikit-learn.
- Model evaluation using accuracy.
- Crop prediction from soil and climate input features.

### Crop Recommendation Application

- Django-based web application.
- Input-driven crop prediction.
- Integration of a trained machine learning model.
- Display of predicted crop recommendations through a web interface.
- HTML and CSS for the application interface.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data manipulation and preprocessing |
| NumPy | Numerical operations |
| Scikit-learn | Model training and prediction |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Django | Web application development |
| HTML and CSS | Frontend interface |
| Google Colab | Model development and experimentation |
| VS Code | Application development |
| Git and GitHub | Version control and project hosting |

## Dataset and Input Features

The project uses agricultural data containing soil nutrient measurements and climatic conditions.

The standard Crop Recommendation dataset contains 2,200 records across 22 crop categories. Verify that your repository uses this exact dataset version before treating these figures as your project's final dataset statistics.

The model uses seven input features:

| Feature | Description |
|---|---|
| Nitrogen (N) | Nitrogen content in the soil |
| Phosphorus (P) | Phosphorus content in the soil |
| Potassium (K) | Potassium content in the soil |
| Temperature | Environmental temperature |
| Humidity | Environmental humidity |
| pH | Soil acidity or alkalinity |
| Rainfall | Rainfall measurement |

**Target variable:** Crop label.

**Output:** A predicted crop category based on the supplied input values.

## Machine Learning Workflow

1. **Data Loading:** Load the agricultural dataset for analysis and model development.
2. **Data Cleaning:** Inspect the dataset and handle missing values or outliers where necessary.
3. **Exploratory Data Analysis:** Examine feature distributions and relationships between soil and climate variables.
4. **Data Visualization:** Create charts using Matplotlib and Seaborn to explore patterns in the data.
5. **Feature Preparation:** Separate input variables from the target crop label and prepare the data for training.
6. **Model Training:** Train a Scikit-learn classification model on the prepared dataset.
7. **Model Evaluation:** Evaluate the trained model using accuracy.
8. **Web Integration:** Connect the trained model to the Django application.
9. **Crop Prediction:** Accept agricultural input values and display the predicted crop.

## Model Performance

The project evaluates its classification model using accuracy.

| Metric | Result |
|---|---|
| Model type | Scikit-learn classification model |
| Evaluation metric | Accuracy |
| Final test accuracy | To be verified from the model evaluation output |

The final test accuracy has not been included because the verified evaluation result is not available in the current project description.

The model's performance should be reported using results from the held-out test dataset, rather than training accuracy alone.

Additional evaluation metrics that could strengthen the project include:

- Precision
- Recall
- F1-score
- Confusion matrix
- Per-class classification performance

## Application Workflow

1. The user enters soil nutrient values and climatic conditions through the web interface.
2. The application collects the supplied input values.
3. The inputs are prepared in the format expected by the trained model.
4. The trained Scikit-learn model generates a crop prediction.
5. The Django application displays the predicted crop category to the user.

The recommendation is a model prediction based on the data used for training. It should not be treated as a guarantee of crop yield or agricultural success.

## Project Structure

The following is an illustrative structure based on the technologies and files described for this project. Adjust it to match the actual folders and filenames in your repository.

```text
crop-recommendation-system/
├── crop_site/
├── recommender/
├── manage.py
├── requirements.txt
├── README.md
├── .gitignore
└── model and data files
```

The `crop_site` directory contains the Django project configuration, while `recommender` is the application directory. Confirm the exact model, dataset, templates, static files, and training notebook locations in the repository before documenting their filenames.

## Getting Started

### Prerequisites

- Python 3.13 or another Python version compatible with the project's dependencies.
- Git.
- pip.
- A terminal such as PowerShell.
- VS Code or another Python development environment.

### 1. Clone the repository

```bash
git clone https://github.com/poojaparab210/crop-recommendation-system.git
cd crop-recommendation-system
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

Make sure the repository includes a valid `requirements.txt` file listing the packages required by the application.

### 4. Run database migrations

```bash
python manage.py migrate
```

### 5. Start the Django development server

```bash
python manage.py runserver
```

### 6. Open the application

Visit:

`http://127.0.0.1:8000/`

Enter the required agricultural input values and test the crop recommendation functionality.

*Note: The application requires its trained model and supporting files to be available at the locations expected by the project code. Follow the actual repository structure if any setup steps differ.*

## Evaluation and Limitations

The project explores the use of machine learning for agricultural crop recommendation.

Current scope:

- Agricultural data cleaning and preprocessing.
- Exploratory data analysis and visualization.
- Classification-based crop prediction.
- Integration of model predictions into a Django application.

Limitations:

- The verified final test accuracy has not yet been documented here.
- Recommendations depend on the quality and coverage of the training dataset.
- The application does not independently validate real-world soil measurements.
- Model predictions do not guarantee crop yield, profitability, or suitability under all local farming conditions.
- The project's actual agricultural or business impact has not been measured.

Further evaluation using independent test data and domain-expert feedback would help assess the system's practical usefulness.

## What I Learned

- Cleaning and preparing agricultural data with Pandas and NumPy.
- Performing exploratory data analysis and interpreting visualizations.
- Understanding relationships between soil nutrients and climatic variables.
- Training and evaluating classification models with Scikit-learn.
- Integrating machine learning predictions into a Django web application.
- Connecting backend prediction logic with a user-facing interface.
- Organizing and documenting a Python project using Git and GitHub.

## Future Improvements

- Compare multiple classification algorithms and select the best-performing model.
- Document test accuracy and additional evaluation metrics.
- Improve input validation and error handling.
- Enhance the user interface and display prediction explanations.
- Evaluate model performance on independent agricultural datasets.
- Deploy the application to a suitable hosting platform.
- Incorporate additional agricultural variables where reliable data is available.
- Seek agricultural expert feedback to evaluate recommendation quality.

## Author

**Pooja Parab**

B.Sc. Computer Science  
Aspiring Data Science and Machine Learning Professional

- **GitHub:** [poojaparab210](https://github.com/poojaparab210)
- **LinkedIn:** [pooja-datascience](https://www.linkedin.com/in/pooja-datascience/)

---

*This project was developed for educational and portfolio purposes. Crop recommendations should be considered alongside local agricultural knowledge, soil testing, weather information, and professional guidance.*
