 Used Car Price Prediction

 1) Problem Statement

This project aims to predict the selling price of used cars based on a dataset of used cars sold on cardehko.com in India. The prediction results can be used to provide price suggestions to new sellers based on market conditions.

 2) Data Collection

The dataset was collected by scraping data from the cardekho website. It contains 13 columns and 15411 rows with various features related to used cars.

 3) Data Cleaning and Preprocessing

*   **Handling Missing Values:** Checked for and handled any missing values in the dataset.
*   **Handling Duplicates:** Checked for and handled any duplicate entries.
*   **Data Type Check:** Ensured that features have the correct data types.
*   **Feature Engineering:** Created new features or transformed existing ones as needed.
*   **Feature Encoding:** Applied one-hot encoding to categorical features with a small number of unique values and that were not ordinal.
*   **Feature Scaling:** Scaled numerical features using StandardScaler.

 4) Exploratory Data Analysis (EDA)

Initial EDA was performed to understand the data distribution, identify missing values, and visualize relationships between features. Post-cleaning EDA was conducted to visualize the distribution of scaled features, correlations, and model performance metrics.

 5) Model Training and Selection

Several regression models were trained and evaluated:

*   Linear Regression
*   Lasso
*   Ridge
*   K-Neighbors Regressor
*   Decision Tree
*   Random Forest Regressor

Model performance was evaluated using metrics such as Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and R2 Score.

 6) Hyperparameter Tuning

Hyperparameter tuning was performed using RandomizedSearchCV for the K-Neighbors Regressor and Random Forest Regressor to find the best parameters for these models.

 7) Model Evaluation

The models were re-trained with the best hyperparameters and evaluated on the test set. The performance metrics for the retrained models were compared.

**Model Performance (After Hyperparameter Tuning):**

*   **Random Forest Regressor:**
    *   Test RMSE: 236926.6454
    *   Test MAE: 98552.6419
    *   Test R2 Score: 0.9254

*   **K-Neighbors Regressor:**
    *   Test RMSE: 295441.3065
    *   Test MAE: 127369.3886
    *   Test R2 Score: 0.8840

Based on the evaluation metrics, the Random Forest Regressor performed best on the test set.

 8) Conclusion

The Random Forest Regressor model demonstrated the best performance in predicting used car prices on this dataset after hyperparameter tuning. The model can be used to provide price suggestions to sellers.

 9) Future Work

*   Explore other regression models and ensemble techniques.
*   Perform more in-depth feature engineering.
*   Implement cross-validation for more robust model evaluation.
*   Deploy the trained model as a web service for real-time predictions.
