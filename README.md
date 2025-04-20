# Determining the Optimal Ensemble Learning Model for House Price Prediction: CatBoost

## Overview

Our project aims to accurately **predict** **housing** **prices** by leveraging advanced ensemble learning models, using the **Ames** **Housing** **dataset** as the foundation. We wish to set a foundation for models that may be valuable for stakeholders in real estate valuation, investment decisions, and urban development planning.

By applying and evaluating the four powerful ensemble techniques — **Random Forest**, **XGBoost**, **LightGBM**, and **CatBoost** — we strive to identify the more effective approach for handling complex, high-dimensional housing data. This research also explores the impact of **feature engineering**, **hyperparameter** **optimization** (**GridSearchCV** vs. **Optuna**), and **model** **interpretability** to ensure that the predictive framework is both robust and practically useful.

## Directory Structure

```         
|-- DS340W                              <- Project root level that is checked into GitHub
      |-- project                       <- Project folder
            |-- data
                  |-- interim           <- Intermediate data that has been transformed
                  |-- processed         <- Final model-ready data
                  |-- raw               <- Original data
            |-- required
                  |-- requirements.txt  <- Libraries for reproducing the Python environment
            |-- src
                  |-- features          <- Scripts for turning raw data into model-ready data
                  |-- models            <- Scripts for training models
      |-- .gitignore                    <- List of files not to sync with GitHub
      |-- README.md                     <- Top-level README for developers
```

### Data File

**AmesHousing.csv**

-   Link to original dataset: <https://www.kaggle.com/datasets/shashanknecrothapa/ames-housing-dataset>

-   We also have this dataset here: **DS340W/project/data/raw**

### Scripts

#### **Scripts for data process**, they are here: **DS340W/project/src/features**

-   **Features_1.ipynb** includes

    -   Initial data exploration

    -   Data cleaning

    -   Feature correlation

    -   Feature engineering

    -   Distribution analysis

    -   Price-related visualizations

-   **Features_2.ipynb** includes

    -   Skewness detection & transformation

    -   Updated correlation analysis

    -   Encoding categorical variables

#### **Scripts for model**, they are here: **DS340W/project/src/models**

(Note here that GitHub will be arranged in alphabetical order, the following list is in the order we ran)

-   **Linear_Regression_Model.ipynb** includes

    -   Initial data inspection

    -   Build the linear regression model

    -   Model evaluation (initial)

    -   Hyperparameter tuning (GridSearchCV)

    -   Model evaluation (tuned with GridSearchCV)

-   **Random_Forest_Model.ipynb** includes

    -   Build the random forest model

    -   Model evaluation (initial)

    -   Hyperparameter tuning (GridSearchCV)

    -   Model evaluation (tuned with GridSearchCV)

    -   Hyperparameter tuning (Optuna, same parameter space)

    -   Model evaluation (tuned with Optuna, same parameter space)

    -   Hyperparameter tuning (Optuna, larger parameter space)

    -   Model evaluation (tuned with Optuna, larger parameter space)

-   **Support_Vector_Regression_Model.ipynb** includes

    -   Build the support vector regression model

    -   Model evaluation (initial)

    -   Hyperparameter tuning (GridSearchCV)

    -   Model evaluation (tuned with GridSearchCV)

-   **Multilayer_Perceptron_Model.ipynb** includes

    -   Build the multi-layer perceptron model

    -   Model evaluation (initial)

    -   Hyperparameter tuning (GridSearchCV)

    -   Model evaluation (tuned with GridSearchCV)

-   **XGBoost_Model.ipynb** includes

    -   Build the extreme gradient boosting (XGBoost) model

    -   Model evaluation (initial)

    -   Hyperparameter tuning (GridSearchCV)

    -   Model evaluation (tuned with GridSearchCV)

    -   Hyperparameter tuning (Optuna, same parameter space)

    -   Model evaluation (tuned with Optuna, same parameter space)

    -   Hyperparameter tuning (Optuna, larger parameter space)

    -   Model evaluation (tuned with Optuna, larger parameter space)

-   **Catboost_Model.ipynb** includes

    -   Build the categorical boosting (CatBoost) model

    -   Model evaluation (initial)

    -   Hyperparameter tuning (Optuna)

    -   Model evaluation (tuned with Optuna)

-   **LightGBM_Model.ipynb** includes

    -   Build the light gradient boosting machine (LightGBM) model

    -   Model evaluation (initial)

    -   Hyperparameter tuning (Optuna)

    -   Model evaluation (tuned with Optuna)

## Getting Started

The full list of packages in our Python environment can be found here: **DS340W/project/required/requirements.txt**

-   We are using **Python 3.12.10**

-   Main packages used:

    -   **pandas**==2.2.3

    -   **numpy**==1.26.4

    -   **seaborn**==0.13.2

    -   **matplotlib**==3.10.1

    -   **scikit-learn**==1.6.1

    -   **optuna**==4.2.1

    -   **xgboost**==3.0.0

    -   **catboost**==1.2.7

    -   **lightgbm**==4.6.0
 
## Links that might be helpful
-   Link for parent paper code: https://github.com/hiteshharsora/housepriceprediction

-   Link to Optuna official website: https://optuna.readthedocs.io/en/stable/index.html

-   Link to CatBoost official website: https://catboost.ai/

## Contact

-   Julia Q. Gui (e-mail: jqg5978@psu.edu)

-   Hannah Wu (e-mail: zmj5109@psu.edu)
