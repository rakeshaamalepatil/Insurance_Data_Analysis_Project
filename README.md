# Insurance Data Analysis Project

This repository contains an Exploratory Data Analysis (EDA) project focused on understanding the factors that influence medical insurance charges. The analysis aims to uncover insights into premium costs, particularly the impact of age, BMI, and smoker status, laying the groundwork for a future predictive model.

## Objective

To analyze the dataset that will help to create a model that will predict the cost of medical insurance based on various input features.

## Domain

Healthcare

## Dataset

The project utilizes the `insurance.csv` dataset, containing information about policyholders and their medical insurance charges.

### Dataset Description:

* `age`: Age of the person
* `sex`: Female or Male
* `bmi`: BMI value to estimate an individual's health and fitness condition
* `children`: Number of children (1, 2, 3, 4, or 5)
* `smoker`: The person is a smoker or not
* `region`: Specifies the region (northeast, northwest, southeast, southwest)
* `charges`: The amount of insurance premium

## Steps Followed

The analysis was conducted following these steps:

1.  Import necessary libraries (Pandas, Matplotlib, NumPy, Seaborn) and load the `insurance.csv` dataset.
2.  Checked the shape of the data and the data types of each column.
3.  Identified and confirmed the absence of missing values in the dataset.
4.  Explored the relationship between various features and the target variable (`charges`) using count plots for categorical features and scatter plots for numerical features (colored by smoker status).
5.  Performed data visualization on feature-vs-feature relationships, including a correlation heatmap for numerical features and count plots for categorical feature interactions.
6.  Investigated the trend of premium charges with aging, specifically differentiating between smokers and non-smokers.
7.  Documented observations and insights after each analytical step.

## Key Findings

Through the exploratory data analysis, I/we uncovered several key determinants of medical insurance charges:

* **Smoker Status is the most significant predictor of insurance charges.** I/We observed that smokers consistently incur substantially higher premiums compared to non-smokers, a difference that holds true across all age groups.
* **Age exhibits a clear positive linear relationship with insurance charges.** As individuals age, their premiums tend to increase, a trend I/we found evident in both smoker and non-smoker groups.
* **BMI shows a positive correlation with charges**, indicating that higher body mass index can lead to increased premiums, though this relationship is less linear and and more scattered than age.
* Features such as **sex, number of children, and geographical region** showed less direct or significant impact on the magnitude of insurance charges compared to smoker status and age.
* The dataset was found to be clean and complete, providing a robust foundation for further analysis.

## Next Steps / Future Work

The insights gained from this exploratory data analysis lay a strong foundation for building a predictive model for medical insurance charges. The logical next steps for this project would involve:

1.  **Data Preprocessing:**
    * Encoding Categorical Features: Convert categorical variables such as 'sex', 'smoker', and 'region' into numerical representations (e.g., using One-Hot Encoding).
    * Feature Scaling (Optional but Recommended): Scale numerical features like 'age' and 'bmi'.
2.  **Model Building:** Select and train appropriate regression models (e.g., Linear Regression, Decision Trees, Random Forests, Gradient Boosting) using the prepared dataset.
3.  **Model Evaluation:** Evaluate the performance of the trained model(s) using relevant metrics (e.g., R-squared, Mean Absolute Error, Root Mean Squared Error).

By following these steps, ABC Insurance can develop a robust model to predict insurance premiums, further enhancing their business decision-making and operational efficiency.

## How to Run

To explore this analysis yourself:

1.  Clone this GitHub repository to your local machine.
2.  Ensure you have Python installed, along with the required libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, and potentially `scikit-learn` for future modeling.
3.  Open the `[Your_Notebook_Name].ipynb` (e.g., `Insurance_Data_Analysis.ipynb`) notebook in Jupyter and run the cells sequentially.
4.  The `insurance.csv` dataset should be in the same directory as the notebook.

---
