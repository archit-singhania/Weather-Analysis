# Weather Analysis and Prediction System

## 📋 Overview
This project focuses on weather analysis for Indian weather data, employing advanced data cleaning, visualization techniques, and machine learning models to predict key weather-related metrics.

### Objectives:
1. Analyze and clean the weather dataset to ensure reliability.
2. Visualize data insights using various plots to identify patterns and relationships.
3. Develop predictive models to accurately forecast metrics such as temperature, humidity, and wind speed.
4. Compare and evaluate the performance of different models to determine the most effective solution.

---

## 🗂️ Dataset
The dataset contains 24 columns capturing diverse weather-related information. Key columns include:

- **`Location Name` and `Region`**: Geographical identifiers for the weather data.
- **`Latitude` and `Longitude`**: Precise coordinates of the data points.
- **`Temperature (Celsius)` and `Feels Like (Celsius)`**: Actual and perceived temperatures.
- **`Weather Conditions`**: Descriptions like "Rainy" or "Sunny".
- **`Wind Data`**: Includes `Wind Speed (Kph)`, `Wind Degree`, and `Wind Direction`.
- **`Pressure`**: Represented in `Mb` and `Inches`.
- **`Precipitation (Mm)`**: Amount of rainfall.
- **`Humidity (%)` and `Cloud Cover (%)`**: Indicators of atmospheric moisture and cloud density.
- **`Visibility (Km)` and `UV Index`**: Metrics for clarity and solar radiation.
- **`Sunrise` and `Sunset Times`**: Daily astronomical data.
- **`Moon Data`**: Includes `Moonrise`, `Moonset`, `Moon Phase`, and `Moon Illumination (%)`.
- **`Air Quality Index (AQI)`**: An environmental health indicator.

---

## 🔧 Data Preprocessing
### 1. Data Cleaning 🧹
- **Irrelevant Data**: Removed columns such as `timezone` that do not contribute to predictions.
- **Duplicates**: Eliminated redundant records to avoid skewed results.
- **Missing Values**: Imputed or removed missing entries based on the context and data distribution.

### 2. Data Visualization 📊
Data insights were explored through various techniques:
- **Bar Plot**: To observe categorical distributions.
- **Count Plot**: To count occurrences of categorical values.
- **Heat Map (Folium)**: For interactive geographical mapping.
- **Scatter Plot**: To study relationships between numerical variables.
- **Histogram and Hist Plot**: To analyze data distribution.
- **Pie Chart**: To represent proportions visually.

### 3. Feature Engineering 🛠️
- Selected statistically significant features for modeling.
- Engineered new attributes such as `Temperature Range` and `Wind Strength Indicator` to enhance model inputs.

### 4. Label Encoding and Standardization 🔤📏
- **Categorical Variables**: Converted into numerical format using Label Encoding.
- **Numerical Features**: Standardized using `StandardScaler` for better model performance.

---

## 📈 Models and Techniques
### 1. **Train-Test Split**
Data was divided into training and testing sets to evaluate model performance on unseen data.

### 2. **Machine Learning Models**
- **RandomForestRegressor**: A robust ensemble-based method.
- **GradientBoostingRegressor**: A sequential ensemble technique.
- **CatBoost Regressor**: A gradient boosting framework optimized for categorical data.
- **LSTM Neural Networks**: For sequential data analysis and predictions.

### 3. **Hyperparameter Tuning** 🔍
To optimize model performance:
- **GridSearchCV**: Exhaustive search over a specified parameter grid.
- **RandomSearchCV**: Randomized search for faster tuning with large datasets.

### 4. **Performance Metrics** 🏆
- **Mean Absolute Error (MAE)**: Measures average prediction error.
- **Mean Squared Error (MSE)**: Penalizes larger errors more heavily.
- **Standard Deviation (STD)**: Evaluates prediction stability.

---

## 🏁 Results
### Model Comparison:
| Model                  | Hyperparameter Tuning | MAE   | MSE   | STD   |
|------------------------|-----------------------|-------|-------|-------|
| RandomForestRegressor | No                    | **Best** | **Best** | **Best** |
| GradientBoostingRegressor | Yes                 | Good  | Good  | Good  |
| CatBoost Regressor    | Yes                   | Fair  | Fair  | Fair  |
| LSTM                  | No                    | Moderate | Moderate | Moderate |

**Conclusion:** Random Forest Regressor emerged as the most reliable model, achieving optimal performance without hyperparameter tuning. 🌟

---

## 🖥️ Tools and Technologies
This project utilized the following technologies:

- **Python**: Core programming language.
- **Pandas**: For data manipulation and preprocessing.
- **NumPy**: For numerical computations.
- **Matplotlib and Seaborn**: For static visualizations.
- **Plotly**: For interactive and dynamic visualizations.
- **Folium**: For interactive geographic mapping.
- **Scikit-learn**: For machine learning models and preprocessing.
- **TensorFlow/Keras**: For implementing LSTM models.
- **CatBoost**: For gradient boosting.

---

## 🚀 Future Scope
- **Real-Time Data Integration**: Expand the system to handle live weather feeds.
- **Feature Expansion**: Include additional weather-related parameters to enhance predictions.
- **Model Optimization**: Experiment with advanced neural networks for further improvement.


