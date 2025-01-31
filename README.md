
# Lagos House Price Prediction Model

This project predicts house prices in Lagos based on a dataset containing various features such as house type, location, and amenities. It uses **Linear Regression** and data preprocessing techniques to train and test the model.

---

## **Table of Contents**

1. [Project Overview](#project-overview)
2. [Data Preprocessing](#data-preprocessing)
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
4. [Model Training](#model-training)
5. [Model Evaluation](#model-evaluation)
6. [Visualization](#visualization)
7. [Installation and Usage](#installation-and-usage)
8. [Contributing](#contributing)
9. [License](#license)

---

## **Project Overview**

The goal of this project is to predict the price of houses in Lagos based on various factors. The dataset used in this project contains information about houses like **location**, **house type**, and **size**. We use machine learning techniques such as **Linear Regression** and **Ridge Regression** to train the model.

---

## **Data Preprocessing**

The data goes through the following steps for preprocessing:
- **Handling Missing Values**: Missing values in the dataset are handled using techniques like filling missing numerical values with the mean or dropping rows with missing target values.
- **Encoding Categorical Variables**: Categorical features like house type and location are transformed into numerical values using **OneHotEncoder**.
- **Feature Scaling**: Numerical features are scaled to ensure uniformity.

The `wrangle` function handles the preprocessing of the dataset by:
1. Dropping rows with missing target values.
2. Filling missing values in numerical columns.
3. One-hot encoding categorical features.

---

## **Exploratory Data Analysis (EDA)**

Before building the model, we conduct an exploratory data analysis to better understand the dataset. This includes:
- **Distribution of House Prices**: We plot the histogram to analyze how house prices are distributed.
- **Average Price per House Type**: Calculate and visualize the average price for different house types.
- **Mean Price per Town**: Group the dataset by town and compute the mean house price per town.
- **Correlation Heatmap**: Visualize relationships between numerical features to understand their correlations.

---

## **Model Training**

We split the dataset into **training** and **testing** sets, using the training set to build and tune the model. The machine learning pipeline includes:
- **OneHotEncoder**: To transform categorical variables.
- **SimpleImputer**: To fill in missing values.
- **Ridge Regression**: For improved regularization over linear regression.

The model is trained on the training set, and predictions are made on the test set.

---

## **Model Evaluation**

The model is evaluated using the **Mean Absolute Error (MAE)** metric. This metric calculates the average absolute difference between the predicted and actual house prices.

---

## **Visualization**

We use various visualizations to analyze the data:
- **Price Distribution**: A histogram to understand the distribution of house prices.
- **Geospatial Distribution of Prices**: Scatter Mapbox plots to show how house prices vary across different locations in Lagos.

---

## **Installation and Usage**

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/lagoshomepredictionmodel.git
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Jupyter Notebook**:
   Launch Jupyter Notebook and open the `Lagos_House_Price_Prediction.ipynb` file to explore the code and results.

---

## **Contributing**

Contributions are welcome! Feel free to fork the repository, create a branch, and submit a pull request with any changes.

---

## **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
