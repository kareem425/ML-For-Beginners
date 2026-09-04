# Regression Analysis on the Linnerud Dataset (Scikit-Learn)

## Methodology & Workflow

1. **Data Loading & Feature Selection:**
   * Load the dataset using `sklearn.datasets.load_linnerud()`.
   * Separate exercise variables from physiological variables.
   * Select **Situps** as the independent feature ($X$) and **Waistline** as the target variable ($y$).

2. **Model Training & Prediction:**
   * Split the dataset into training and testing sets using `train_test_split()`.
   * Instantiate a `LinearRegression` model from `sklearn.linear_model`.
   * Fit the model using $X_{train}$ and $y_{train}$.
   * Predict the target values using $X_{test}$.

3. **Visualization & Generalization:**
   * Create a scatter plot of the original data points alongside the fitted regression line using `matplotlib.pyplot`.
   * Apply this exact methodology iteratively to analyze other exercise and physiological pairs across the dataset (e.g., *Chins* or *Jumps* vs. *Weight* or *Pulse*).

---

## Descriptive Paragraph (For Submission)

> To analyze the relationship between exercise and physiological metrics using Scikit-learn's Linnerud dataset, I start by loading the dataset and separating the exercise features from the physiological targets. To evaluate the relationship between situps and waistline, I select 'Situps' as the independent variable ($X$) and 'Waist' as the target variable ($y$). Next, I split the data into training and testing sets using `train_test_split()`, instantiate a `LinearRegression` model, and fit it on $X_{train}$ and $y_{train}$. After generating predictions for $X_{test}$, I plot a scatter plot of the data points alongside the fitted regression line to visualize the trend. This exact pipeline—feature isolation, train-test splitting, model fitting, prediction, and plotting—can then be repeatedly applied to examine the other exercise and physiological variable pairs in the dataset, such as Chins or Jumps against Weight or Pulse.