# Price-Prediction-on-Ford-Car-Dataset

This project is a **Machine Learning regression project** that aims to **predict the selling price of Ford cars** using various vehicle attributes. The project demonstrates a complete supervised machine learning workflow:

1. Data loading and inspection.
2. Exploratory Data Analysis (EDA).
3. Data preprocessing (encoding and feature scaling).
4. Train-Test Split.
5. Building a Linear Regression model.
6. Evaluating the model using **R²** and **Adjusted R²**.
7. Comparing different encoding methods to identify the better preprocessing approach for price prediction.

The project begins by importing essential Python libraries such as **NumPy, Pandas, Matplotlib, Seaborn, and Scikit-learn**. The Ford car dataset(Kaggle) is then loaded and inspected to understand its structure, dimensions, summary statistics, and missing values.

Next, **Exploratory Data Analysis (EDA)** is performed to understand the relationships between different variables and the target variable (car price). Several visualizations, including histograms, scatter plots, box plots, and a correlation heatmap, are used to examine how factors such as **year of manufacture, mileage, engine size, fuel type, transmission type, tax, and fuel efficiency (mpg)** influence the selling price.

Since the dataset contains categorical variables, the project experiments with **two different encoding techniques**:

* **One-Hot Encoding** for categorical features.
  -Here we create a dummy variable for each category excludingone to avoid Multicollinearity.
* **Label Encoding** for categorical features.
  -It transform each unique category in a column into a distinct number between 0 to n-1; where n is the number of distinct category.  
The numerical variables are then standardized using **StandardScaler** to ensure they are on a comparable scale before model training.

After preprocessing, the dataset is divided into **training and testing sets** using a train-test split. A **Linear Regression** model is trained to predict car prices. The project builds and compares two versions of the model—one using one-hot encoded data and another using label-encoded data.

Finally, the performance of the models is evaluated using **R² (Coefficient of Determination)** and **Adjusted R²**. These metrics help determine how well the model explains the variation in car prices and assess its predictive capability.



