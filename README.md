## Market Campaign Sales Prediction Project 
-- By Linear Regression--

A machine learning project that uses Linear Regression to predict sales based on market campaign and business-related data. The notebook covers exploratory data analysis, data cleaning, feature transformation, statistical analysis, regression assumptions, model training, and evaluation.
Project Overview
The goal of this project is to understand how marketing and website-related factors influence sales and to build a regression model that can estimate sales from the available features.
- Problem type: Supervised Machine Learning – Regression
- Target variable: Sales
- Main algorithm: Linear Regression
- Evaluation metrics: R² Score and Root Mean Squared Error (RMSE)
Tools and Libraries
- Python
- Jupyter Notebook
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Statsmodels
- SciPy (for statistical analysis)
Project Workflow
1. Data loading – Load the market campaign sales dataset into a Pandas DataFrame.
2. Exploratory Data Analysis (EDA) – Inspect the dataset, understand its structure and descriptive statistics, and check missing values, duplicates, distributions, and outliers.
3. Train-test split – Separate Sales as the target variable and split the data into training and testing sets (80:20).
4. Data preprocessing
   - Handle missing numerical values using the median.
   - Handle missing categorical values using the mode.
   - Examine outliers and skewness; apply transformations where appropriate.
   - Encode categorical variables using one-hot encoding.
   - Scale numerical features using StandardScaler.
5. Statistical analysis – Explore the relationship between sales and numerical/categorical features and perform statistical tests.
6. Regression diagnostics – Examine linear regression assumptions, including linearity, multicollinearity (correlation and VIF), residual normality, homoscedasticity, and independence of errors.
7. Model training – Train a Linear Regression model using the processed training data.
8. Model evaluation – Evaluate training and testing predictions using R² Score and RMSE.
Key Findings
The notebook's analysis highlights the following business observations:
- Conversion Rate has a strong positive relationship with sales and is identified as the most influential factor in the analysis.
- Marketing spend across Search Engine Marketing, Social Media, and TV is positively associated with sales. Search Engine Marketing shows the strongest estimated contribution per unit of spend among these channels.
- Discounts also show a positive relationship with sales.
- Website traffic alone has very little estimated effect on sales after accounting for other features in the model.
- The notebook reports an approximate test R² score of 0.95 and test RMSE of 6,400, indicating that the model explains around 95% of the variation in test-set sales. These are approximate results reported in the notebook and may vary if the data or workflow changes.
Repository Structure
Market-Campaign-Sales-Prediction/
│
├── Market campaign sales prediction.ipynb
├── market_sales - LMS.csv        # Add the dataset here, if permitted to share
└── README.md
The notebook currently reads the CSV from a local file path. Update the pd.read_csv() path in the notebook to match the location of the dataset on your system. The dataset is not included in this project unless you add it separately.

How to Run the Project
1. Clone or download this repository.
2. Make sure Python and Jupyter Notebook are installed.
3. Install the required libraries:
   pip install pandas numpy matplotlib seaborn scikit-learn statsmodels scipy jupyter
4. Place the dataset CSV in the project folder, if you have permission to share and use it.
5. Open the notebook:
   jupyter notebook
6. Open Market campaign sales prediction.ipynb, update the dataset path if needed, and run the cells.
Future Improvements
- Use a Scikit-learn Pipeline and ColumnTransformer to make preprocessing more consistent and reproducible.
- Compare Linear Regression with Ridge, Lasso, Random Forest, and other regression algorithms.
- Apply cross-validation and hyperparameter tuning.
- Track additional metrics such as MAE and adjusted R².
- Save the trained model and build a simple interface for making sales predictions.
Author
Aniket Yadav
If you find this project useful, feel free to ⭐ the repository.
