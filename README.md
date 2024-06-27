# Forest_Fire_Prediction-CodXo_Internship
### Summary of Analysis on Algerian Forest Fires Processed Dataset

#### Dataset Overview
The dataset used is the **Algerian Forest Fires Cleaned Dataset** downloaded from Kaggle. It contains various meteorological data points collected in 2012 to predict forest fires. The dataset has 243 rows and 15 columns, including attributes like Temperature, Relative Humidity (RH), Wind Speed (Ws), Rain, and several fire indices (FFMC, DMC, DC, ISI, BUI, FWI), along with the target variable 'Classes' (fire/not fire) and the region.

#### Data Preprocessing
- **Missing Values**: No missing values were present in the dataset.
- **Categorical Data**: The target variable 'Classes' was converted to numerical values (fire = 1, not fire = 0).
- **Normalization**: Numerical features were standardized using `StandardScaler`.

#### Exploratory Data Analysis (EDA)
- **Correlation Matrix**: Displayed to understand the relationships between features.
- **Distribution Analysis**: Histograms were plotted for numerical features.
- **Box Plots**: Created to identify outliers and understand feature distributions.
- **Time Series Plot**: Analyzed average temperature over time.
- **Scatter Plots**: Visualized pairwise relationships between features colored by class.
- **Bar Plots**: Displayed frequency of fire occurrences by month.

#### Model Selection and Training
The **Random Forest Classifier** was chosen for predictive modeling. The dataset was split into training and testing sets with a 70-30 split.

##### Initial Model Performance
- **Accuracy**: 99%
- **Precision**: 0.97 (class 0), 1.00 (class 1)
- **Recall**: 1.00 (class 0), 0.98 (class 1)
- **F1-Score**: 0.98 (class 0), 0.99 (class 1)
- **ROC AUC Score**: 0.9886
- **Matthews Correlation Coefficient**: 0.9719

#### Hyperparameter Tuning
A grid search with cross-validation was performed to find the best hyperparameters for the Random Forest model.

##### Tuned Model Performance
- **Accuracy**: 99%
- **Precision**: 0.97 (class 0), 1.00 (class 1)
- **Recall**: 1.00 (class 0), 0.98 (class 1)
- **F1-Score**: 0.98 (class 0), 0.99 (class 1)
- **Best ROC AUC Score**: 0.9886
- **Best Matthews Correlation Coefficient**: 0.9719

#### Results and Conclusion
The Random Forest Classifier performed exceptionally well with an accuracy of 99%, indicating a robust model capable of accurately predicting forest fires based on the provided features. The high ROC AUC score and Matthews Correlation Coefficient further confirm the model's reliability.

In summary, the analysis involved comprehensive data preprocessing, exploratory data analysis, model training, and hyperparameter tuning, resulting in a highly accurate predictive model for forest fires in Algeria.
