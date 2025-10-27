# Medical Appointment No-Show Prediction

## Project Overview

This project aims to predict patient no-shows for medical appointments using machine learning. No-shows cause inefficiencies and lost resources in healthcare; predicting these helps optimize scheduling and patient outreach.

We explore several machine learning models, including Logistic Regression, Decision Trees, Random Forest, XGBoost, and Artificial Neural Networks (ANN). We perform data cleaning, feature engineering, model training, hyperparameter tuning, and evaluation.

## Dataset

We use a public dataset containing patient appointment information, including:
- Patient demographics (age, scholarship status, health conditions like hypertension, diabetes, alcoholism)
- Appointment information (scheduled day, appointment day, days difference)
- SMS reminders received
- No-show labels (0 = showed up, 1 = no-show)

## Key Challenges

- Imbalanced dataset with fewer no-shows than shows
- Time features needing careful processing (handling time components in dates)
- Feature selection and encoding to improve model learning

## Methods

1. Data Cleaning and Feature Engineering  
2. Exploratory Data Analysis with visualization (histograms, bar plots, correlation heatmaps)  
3. Baseline model comparisons (Logistic Regression, Decision Tree, Random Forest, SVM)  
4. Hyperparameter tuning using GridSearchCV with custom scoring (F1)  
5. Evaluation with classification metrics focusing on F1 score and recall  
6. Introduction to advanced models like XGBoost and ANNs  

## Results

- Baseline models achieved up to ~77% accuracy but poor recall on no-shows.
- Hyperparameter tuning improved F1 score significantly (~0.44), emphasizing recall.
- XGBoost and ANN models explored for further improvements.
- Final tuned models balanced recall and precision for effective no-show detection.

## How to Use

1. Install dependencies: `pip install -r requirements.txt`  
2. Run `data_preprocessing.ipynb` to clean and prepare data  
3. Train models in `model_training.ipynb` with provided parameters  
4. Evaluate and interpret results using included visualization notebooks  
5. Modify and extend for your datasets or clinical scenarios

## Contributing

Contributions, suggestions, and feedback welcome! Please open issues or pull requests.

## License

MIT License

---

