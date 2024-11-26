

# IPL 2025 Mega Auction: Machine Learning Analysis

## Overview

This project explores and applies machine learning (ML) techniques to analyze the IPL 2025 Mega Auction dataset. The goal is to extract insights about player evaluation, team strategies, bidding trends, and more. We aim to predict player prices, recommend team compositions, and analyze the performance trends of players.

## Dataset

The dataset contains the following columns:

- **Players**: The name of the player.
- **Team**: The IPL team the player belongs to.
- **Type**: The type of player (e.g., BAT, BOWL, AR for all-rounder, WK for wicketkeeper).
- **Base**: The base price of the player during the auction.
- **Sold**: The final sale price or "TBA" (To Be Announced) if unsold.

### Sample Data

| Players            | Team | Type | Base   | Sold   |
|--------------------|------|------|--------|--------|
| Virat Kohli        | RCB  | BAT  | -      | 21.00  |
| Rajat Patidar      | RCB  | BAT  | -      | 11.00  |
| Yash Dayal         | RCB  | BOWL | -      | 5.00   |
| Jasprit Bumrah     | MI   | BOWL | -      | 18.00  |
| Suryakumar Yadav   | MI   | BAT  | -      | 16.35  |
| Vijay Yadav        | -    | AR   | 0.30   | TBA    |

### Notes:
- The `Base` column contains missing values (`"-"`), which are handled in the preprocessing stage.
- The target variable for prediction is the **Sold** price of the player.

## Important Considerations

### 1. Player Evaluation Analysis:
   - Analyze the relationship between base price and sale price.
   - Identify which player types (BAT, BOWL, AR, WK) tend to get the highest prices.

### 2. Team Composition and Strategy:
   - Analyze how each team uses their budget.
   - Find out which type of players each team tends to target more.

### 3. Auction Trends Analysis:
   - Identify which countries have more demand for players.
   - Explore the demand for younger players (under 25).

### 4. Feature Engineering:
   - Derive features based on player performance (e.g., batting average, wicket-taking ability).
   - Analyze franchisees' past strategies or trends.

### 5. ML Model Objectives:
   - Predict the sale price of players.
   - Predict which team a player will join.
   - Analyze the probability of a player being the MVP (Most Valuable Player).

---

## Expected Results

### 1. **Evaluation and Prediction:**
   - Accurately predict a player's sale price for the upcoming auction.
   - Gain insights into future auction trends.

### 2. **Team Composition Optimization:**
   - Analyze team strengths and weaknesses.
   - Suggest optimal budget utilization strategies for franchisees.

### 3. **Player Qualification Analysis:**
   - Rate players based on past performances, providing insights into their value.

### 4. **Data Visualization:**
   - Create compelling visualizations to show trends related to teams and players.
   - Use bar charts, box plots, heatmaps, and scatter plots to present results.

### 5. **Predictive Analytics:**
   - Identify players whose demand might rise in future auctions.

---

## Machine Learning Steps

### 1. **EDA (Exploratory Data Analysis):**
   - Perform qualitative and quantitative analysis on the data.
   - Identify patterns and trends in the dataset.

### 2. **Data Preprocessing:**
   - Handle missing values (e.g., for `Base` column).
   - Encode categorical features (e.g., player type, team).
   - Scale numerical features to standardize the dataset.

### 3. **ML Model Selection:**
   - Use regression models (e.g., Linear Regression, Random Forest Regressor) to predict player prices.
   - Use classification models (e.g., Logistic Regression, Gradient Boosting) to predict which team a player might join.

### 4. **Hyperparameter Tuning:**
   - Use GridSearchCV or RandomizedSearchCV to optimize model performance.

### 5. **Reporting and Sharing Insights:**
   - Visualize results and create reports.
   - Share findings on Kaggle or GitHub to help teams in future auction strategies.

---

## Project Structure

```
├── data/
│   └── dataset.csv         # The IPL 2025 dataset
├── model/
│   └── model.py            # Machine learning model code
├── notebooks/
│   └── analysis.ipynb      # Jupyter notebook for analysis and model training
├── README.md               # This file
└── requirements.txt        # Python dependencies
```

## Installation

To run this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ipl-2025-auction-analysis.git
   cd ipl-2025-auction-analysis
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv env
   source env/bin/activate  # For Windows use: .\env\Scripts\activate
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. **requirements.txt** contains the following dependencies:
   ```
   pandas
   numpy
   scikit-learn
   matplotlib
   seaborn
   ```

---

## Contributing

Feel free to contribute to this project by opening issues or submitting pull requests. Your contributions are highly appreciated!

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

### Translation to English:

---

# IPL 2025 Mega Auction: Machine Learning Analysis

## Overview

This project explores and applies machine learning (ML) techniques to analyze the IPL 2025 Mega Auction dataset. The goal is to extract insights about player evaluation, team strategies, bidding trends, and more. We aim to predict player prices, recommend team compositions, and analyze the performance trends of players.

## Dataset

The dataset contains the following columns:

- **Players**: The name of the player.
- **Team**: The IPL team the player belongs to.
- **Type**: The type of player (e.g., BAT, BOWL, AR for all-rounder, WK for wicketkeeper).
- **Base**: The base price of the player during the auction.
- **Sold**: The final sale price or "TBA" (To Be Announced) if unsold.

### Sample Data

| Players            | Team | Type | Base   | Sold   |
|--------------------|------|------|--------|--------|
| Virat Kohli        | RCB  | BAT  | -      | 21.00  |
| Rajat Patidar      | RCB  | BAT  | -      | 11.00  |
| Yash Dayal         | RCB  | BOWL | -      | 5.00   |
| Jasprit Bumrah     | MI   | BOWL | -      | 18.00  |
| Suryakumar Yadav   | MI   | BAT  | -      | 16.35  |
| Vijay Yadav        | -    | AR   | 0.30   | TBA    |

### Notes:
- The `Base` column contains missing values (`"-"`), which are handled in the preprocessing stage.
- The target variable for prediction is the **Sold** price of the player.

## Important Considerations

### 1. Player Evaluation Analysis:
   - Analyze the relationship between base price and sale price.
   - Identify which player types (BAT, BOWL, AR, WK) tend to get the highest prices.

### 2. Team Composition and Strategy:
   - Analyze how each team uses their budget.
   - Find out which type of players each team tends to target more.

### 3. Auction Trends Analysis:
   - Identify which countries have more demand for players.
   - Explore the demand for younger players (under 25).

### 4. Feature Engineering:
   - Derive features based on player performance (e.g., batting average, wicket-taking ability).
   - Analyze franchisees' past strategies or trends.

### 5. ML Model Objectives:
   - Predict the sale price of players.
   - Predict which team a player will join.
   - Analyze the probability of a player being the MVP (Most Valuable Player).

---

## Expected Results

### 1. **Evaluation and Prediction:**
   - Accurately predict a player's sale price for the upcoming auction.
   - Gain insights into future auction trends.

### 2. **Team Composition Optimization:**
   - Analyze team strengths and weaknesses.
   - Suggest optimal budget utilization strategies for franchisees.

### 3. **Player Qualification Analysis:**
   - Rate players based on past performances, providing insights into their value.

### 4. **Data Visualization:**
   - Create compelling visualizations to show trends related to teams and players.
   - Use bar charts, box plots, heatmaps, and scatter plots to present results.

### 5. **Predictive Analytics:**
   - Identify players whose demand might rise in future auctions.

---

## Machine Learning Steps

### 1. **EDA (Exploratory Data Analysis):**
   - Perform qualitative and quantitative analysis on

 the data.
   - Identify patterns and trends in the dataset.

### 2. **Data Preprocessing:**
   - Handle missing values (e.g., for `Base` column).
   - Encode categorical features (e.g., player type, team).
   - Scale numerical features to standardize the dataset.

### 3. **ML Model Selection:**
   - Use regression models (e.g., Linear Regression, Random Forest Regressor) to predict player prices.
   - Use classification models (e.g., Logistic Regression, Gradient Boosting) to predict which team a player might join.

### 4. **Hyperparameter Tuning:**
   - Use GridSearchCV or RandomizedSearchCV to optimize model performance.

### 5. **Reporting and Sharing Insights:**
   - Visualize results and create reports.
   - Share findings on Kaggle or GitHub to help teams in future auction strategies.

---

## Project Structure

```
├── data/
│   └── dataset.csv         # The IPL 2025 dataset
├── model/
│   └── model.py            # Machine learning model code
├── notebooks/
│   └── analysis.ipynb      # Jupyter notebook for analysis and model training
├── README.md               # This file
└── requirements.txt        # Python dependencies
```

## Installation

To run this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ipl-2025-auction-analysis.git
   cd ipl-2025-auction-analysis
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv env
   source env/bin/activate  # For Windows use: .\env\Scripts\activate
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. **requirements.txt** contains the following dependencies:
   ```
   pandas
   numpy
   scikit-learn
   matplotlib
   seaborn
   ```

---

## Contributing

Feel free to contribute to this project by opening issues or submitting pull requests. Your contributions are highly appreciated!

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


