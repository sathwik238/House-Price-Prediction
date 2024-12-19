# House-Price-Prediction

This project predicts house prices using a **Decision Tree Regression model**. The dataset includes features such as square footage, number of bedrooms, location, and more, which are used to train and evaluate the model.

---

## **Table of Contents**
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Technologies Used](#technologies-used)
4. [Model Workflow](#model-workflow)
5. [Results](#results)
6. [Visualization](#visualization)
7. [How to Run the Project](#how-to-run-the-project)
8. [Future Work](#future-work)
9. [References](#references)

---

## **Project Overview**

The goal of this project is to predict house prices based on given features using a **Decision Tree Regressor**. Decision Tree models are intuitive, interpretable, and effective for regression tasks involving non-linear relationships.

---

## **Dataset**

- **File**: `house_price.csv`
- **Description**:
   - The dataset contains multiple features like:
     - Square Footage
     - Number of Bedrooms
     - Number of Bathrooms
     - Lot Size
     - Location
     - Year Built
     - House Price (Target)
- **Target Variable**: `Price`

**Sample Data**:
| SquareFootage | Bedrooms | Bathrooms | YearBuilt | Location      | Price     |
|---------------|----------|-----------|-----------|---------------|-----------|
| 2100          | 3        | 2         | 2001      | Seattle       | $540,000  |
| 1500          | 2        | 1         | 1998      | Los Angeles   | $410,000  |
| 3200          | 4        | 3         | 2010      | New York      | $750,000  |

---

## **Technologies Used**

- **Programming Language**: Python
- **Libraries**:
   - pandas: Data manipulation and analysis
   - numpy: Numerical operations
   - matplotlib & seaborn: Data visualization
   - sklearn: Machine learning (Decision Tree Regressor)

---

## **Model Workflow**

1. **Data Preprocessing**:
   - Load the dataset
   - Handle missing values (if any)
   - Encode categorical variables (e.g., `Location`)
   - Feature scaling (optional for Decision Tree models)

2. **Exploratory Data Analysis (EDA)**:
   - Visualize feature distributions
   - Analyze correlations between features and the target variable

3. **Model Training**:
   - Split the data into training and testing sets (e.g., 80% train, 20% test).
   - Train the **Decision Tree Regressor**.

4. **Model Evaluation**:
   - Evaluate model performance using:
     - Mean Squared Error (MSE)
     - R² Score (Coefficient of Determination)

---

## **Results**

- **Performance Metrics**:
   - Mean Squared Error (MSE): `398`
   - R² Score: `0.96` 

**Key Findings**:
- The model performs well with an R² score of **96%**, indicating it can explain most of the variance in house prices.
- Features like `price_per_sqft`, `total_sqft_int`, and `bhk` are significant predictors of price.

---