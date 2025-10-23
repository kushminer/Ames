# Ames Housing Price Prediction

A comprehensive machine learning project analyzing and predicting house prices in Ames, Iowa using advanced regression techniques and extensive feature engineering.

## Overview

This project performs in-depth analysis of the Ames Housing Dataset, containing approximately 2,580 house sale records from 2006-2010 with 81 features describing various aspects of residential properties. The goal is to build both descriptive and predictive models to understand the local housing market dynamics and accurately forecast house prices.

## Key Features

- **Comprehensive Data Analysis**: Detailed exploratory data analysis revealing housing market insights
- **Advanced Feature Engineering**: Custom feature creation based on domain knowledge and data-driven insights
- **Multiple Modeling Approaches**: Implementation of various regression algorithms including:
  - Linear Regression with regularization (Ridge, Lasso)
  - Gradient Boosting (XGBoost, LightGBM, CatBoost)
  - Statistical modeling with StatsModels
- **Robust Preprocessing**: Handling missing values, outliers, and encoding categorical variables
- **Model Evaluation**: Cross-validation and performance metrics (R², MAE, RMSE)

## Project Structure

```
Ames/
│
├── data/
│   ├── Ames_Housing_Price_Data.csv      # Main dataset (81 features)
│   └── Ames_Real_Estate_Data.csv        # Additional property data
│
├── pic/
│   ├── Ames.jpg                         # City images
│   ├── AmesHouses.jpg
│   └── ISU.jpg
│
├── Ames_1_import_basic_data_eval.ipynb  # Data import and initial evaluation
├── Ames_2_exploratory_data_analysis.ipynb  # Comprehensive EDA
├── Ames_3_preprocessing.ipynb           # Data cleaning and preprocessing
├── Ames_4_feature_engineering.ipynb     # Feature creation and selection
├── Ames_5_regression.ipynb              # Model training and evaluation
├── Ames_6_future_work.ipynb             # Future improvements and extensions
├── Machine Learning Project Proposal.ipynb  # Project overview and methodology
│
└── README.md
```

## Dataset Description

The Ames Housing Dataset includes detailed information about:

- **Property Characteristics**: Lot size, building type, dwelling style, year built
- **Quality Metrics**: Overall quality, exterior quality, kitchen quality, basement finish
- **Size Features**: Living area, basement area, garage size, porch area
- **Amenities**: Fireplaces, pools, garages, central air conditioning
- **Location**: Neighborhood, proximity to conditions, lot configuration
- **Sale Information**: Sale price, sale type, sale condition, month/year sold

## Methodology

### 1. Data Import & Evaluation
- Load raw data and perform initial quality checks
- Understand data types (43 categorical, 39 numerical features)
- Identify high dimensionality challenges

### 2. Exploratory Data Analysis
- Analyze price distributions and relationships
- Investigate price per square foot variations
- Study neighborhood characteristics and trends
- Examine temporal patterns (seasonality, market trends)
- Discover log-log relationships between area and price

### 3. Data Preprocessing
- Handle missing values with appropriate imputation strategies
- Detect and treat outliers
- Encode categorical variables (Label Encoding, One-Hot Encoding)
- Scale and normalize features

### 4. Feature Engineering
- Create interaction features
- Generate polynomial features
- Engineer domain-specific features (e.g., total bathrooms, house age)
- Apply feature selection techniques

### 5. Model Training & Evaluation
- Train multiple regression models
- Perform hyperparameter tuning with GridSearchCV
- Cross-validation for robust performance estimation
- Compare models using multiple metrics

### 6. Future Work
- Ensemble methods
- Advanced feature engineering
- Model interpretation and explainability

## Key Insights

- **Price/Area Relationship**: Log-log transformation reveals that price per square foot decreases for larger homes, suggesting market pressure on high-end properties
- **Top Features**: Ground living area, overall quality, total basement area, and garage area are strongest predictors
- **Neighborhood Impact**: Significant price variations across neighborhoods reflecting school quality, commute times, and amenities
- **Quality Premium**: Overall quality ratings show strong positive correlation with sale prices

## Technologies Used

- **Python 3.x**
- **Data Analysis**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Machine Learning**: Scikit-learn
- **Advanced Models**: XGBoost, LightGBM, CatBoost
- **Statistical Analysis**: StatsModels
- **Geospatial**: Geopy (for location-based analysis)

## Installation & Setup

1. Clone the repository:
```bash
git clone https://github.com/yourusername/Ames.git
cd Ames
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

4. Launch Jupyter Notebook:
```bash
jupyter notebook
```

5. Run notebooks in sequential order (1 through 6)

## Usage

The project is organized as a series of Jupyter notebooks that should be executed in order:

1. Start with `Machine Learning Project Proposal.ipynb` to understand the project scope
2. Follow the numbered notebooks (1-6) for the complete analysis pipeline
3. Each notebook builds upon the previous, creating a comprehensive workflow

## Model Performance

The project explores multiple regression algorithms with performance metrics tracked throughout the modeling process. Best results achieved using ensemble methods combining gradient boosting algorithms.

*(Specific metrics would be added here after reviewing the regression notebook)*

## Future Enhancements

- Implement stacking and blending ensemble methods
- Add geospatial analysis using property coordinates
- Develop interactive visualizations and dashboards
- Deploy model as a web application for real-time predictions
- Incorporate external data (economic indicators, school ratings)

## Dataset Source

This project uses the Ames Housing Dataset, a well-known dataset for regression analysis in machine learning. A subset is available on [Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data) as an entry-level competition.

## Author

Created as a comprehensive machine learning portfolio project demonstrating end-to-end data science workflow from exploratory analysis to model deployment preparation.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Iowa State University for the Ames Housing Dataset
- The data science community for inspiration and best practices
- Contributors to the open-source libraries used in this project

## Contact

For questions, feedback, or collaboration opportunities, please open an issue or reach out via [your contact method].

---

**Note**: This project demonstrates proficiency in data analysis, feature engineering, machine learning model development, and professional documentation practices.
