# ✈️ Flight Fare Prediction

A machine learning regression project that predicts flight ticket prices based on flight details such as airline, source, destination, journey date, departure time, arrival time, duration, total stops, and additional flight information.

This project demonstrates an end-to-end machine learning workflow, including data cleaning, feature engineering, exploratory data analysis (EDA), preprocessing with Scikit-learn pipelines, model comparison, hyperparameter tuning, and model evaluation.

---

## 📂 Project Structure

```text
flight-fare-prediction/
│
├── data/                         # Dataset
├── notebooks/
│   └── flight_fare_prediction.ipynb
├── requirements.txt              # Project dependencies
├── README.md                     # Project documentation
└── .gitignore
```

---

## 📊 Dataset

The dataset contains flight information used to predict ticket prices.

### Features

- Airline
- Source
- Destination
- Journey Date
- Departure Time
- Arrival Time
- Duration
- Total Stops
- Additional Information

### Target Variable

- **Price**

---

## 🔧 Project Workflow

1. Data Cleaning
2. Feature Engineering
3. Exploratory Data Analysis (EDA)
4. Data Preprocessing
5. Train-Test Split
6. Baseline Model Training
7. Hyperparameter Tuning
8. Model Evaluation

---

## 📈 Exploratory Data Analysis (EDA)

Some key observations from the analysis include:

- Flight prices are right-skewed with a few high-value outliers.
- Ticket prices generally increase as the number of stops increases.
- Airline selection has a significant impact on ticket prices.
- Journey month shows seasonal variation in airfare.
- Flight duration is positively related to ticket price.
- Source and destination contribute to fare variation when combined with other flight attributes.

---

## 🤖 Baseline Model Comparison

| Model | RMSE | R² Score |
|-------|------:|---------:|
| **XGBoost** | **1420.30** | **0.9064** |
| Random Forest | 1619.13 | 0.8785 |
| Gradient Boosting | 1858.25 | 0.8399 |
| Linear Regression | 2568.31 | 0.6941 |

---

## 🏆 Final Model

After comparing multiple regression algorithms, the top-performing models (XGBoost and Random Forest) were further optimized using **RandomizedSearchCV**.

Hyperparameter tuning improved the performance of **XGBoost**, while Random Forest showed minimal improvement. The final XGBoost model achieved the best predictive performance.

### Final Performance

| Metric | Value |
|---------|------:|
| **RMSE** | **1345.72** |
| **R² Score** | **0.9160** |

---

## 📈 Results

Among the evaluated regression models, **XGBoost** consistently outperformed Linear Regression, Random Forest, and Gradient Boosting.

The superior performance of XGBoost indicates that flight fare prediction involves complex, non-linear relationships that are better captured by boosting-based ensemble models.

The final tuned model achieved:

- **RMSE:** **1345.72**
- **R² Score:** **0.9160**

This means the model explains approximately **91.6% of the variance** in flight ticket prices while maintaining a relatively low prediction error.

---

## ⭐ Project Highlights

- Built an end-to-end machine learning regression pipeline.
- Performed comprehensive data cleaning and feature engineering.
- Extracted useful date and time features from raw flight information.
- Compared multiple regression algorithms.
- Optimized the best-performing model using RandomizedSearchCV.
- Achieved an **R² Score of 0.9160** using XGBoost.

---

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

---

## 💡 Skills Demonstrated

- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Data Preprocessing
- Feature Encoding
- Scikit-learn Pipelines
- Regression Modeling
- Hyperparameter Optimization
- Model Evaluation
- Machine Learning

---

## 🚀 How to Run

Clone the repository:

```bash
git clone https://github.com/<your-username>/flight-fare-prediction.git
```

Navigate to the project folder:

```bash
cd flight-fare-prediction
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
notebooks/flight_fare_prediction.ipynb
```

---

## 👤 Author

**Chandrapal Rajput**

* Linkedin : https://www.linkedin.com/in/chandrapal-deora/

---
