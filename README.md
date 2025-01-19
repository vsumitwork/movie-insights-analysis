
# 🎬 Movie Data Analysis Project

## 📖 Overview

This project involves analyzing a dataset of movies to uncover insights into relationships between various features, such as budget, gross revenue, and ratings. The analysis was performed in Python using Jupyter Notebook, employing data cleaning, visualization, and statistical methods.

## 🗂️ Dataset

The dataset consists of **7,668 movies** with the following features:
- **name**: Title of the movie
- **rating**: Movie rating (e.g., PG, R)
- **genre**: Genre of the movie (e.g., Action, Drama)
- **year**: Year of release
- **released**: Exact release date
- **score**: IMDB score
- **votes**: Number of IMDB votes
- **director**: Director's name
- **writer**: Writer's name
- **star**: Lead actor/actress
- **country**: Country of production
- **budget**: Production budget
- **gross**: Gross earnings
- **company**: Production company
- **runtime**: Duration of the movie (in minutes)

## 🛠️ Steps Performed

### 1️⃣ Data Cleaning
- Checked for missing values in all columns and calculated the percentage of missing data.
- Handled missing values by:
  - Filling budget data with the column's median value.
  - Dropping rows with any remaining NaN values.
- Ensured proper data types for numeric columns (`budget`, `gross`, etc.).

### 2️⃣ Exploratory Data Analysis (EDA)
- **Identified missing data patterns** to understand how incomplete the dataset was.
- Checked for duplicates and removed them to ensure data integrity.
- Used visualizations like **box plots** to detect outliers in the `gross` earnings column.

### 3️⃣ Correlation Analysis
- Explored the relationships between numeric features using:
  - **Pearson**, **Spearman**, and **Kendall** correlation coefficients.
  - Heatmaps to visually represent correlations.
- Significant correlations:
  - **Budget and Gross Revenue** (Strong Positive Correlation: 0.746)
  - **Votes and Gross Revenue** (Moderate Positive Correlation: 0.631)

### 4️⃣ Data Visualization
- **Scatter Plots**:
  - Budget vs. Gross Earnings
  - IMDB Score vs. Gross Earnings
- **Regression Analysis**:
  - Applied regression lines to visualize relationships.
- **Correlation Heatmaps**:
  - Analyzed how numeric and categorical data relate to revenue.

## 📊 Key Findings
- Movies with higher budgets tend to earn higher gross revenue.
- Audience votes have a strong correlation with revenue, suggesting popular movies are more likely to be financially successful.
- IMDB score has a weaker but positive correlation with gross earnings, showing that quality does impact revenue, but not as strongly as budget or popularity.

## 🛠️ Technologies Used
- **Libraries**:
  - `pandas` for data manipulation
  - `numpy` for numerical calculations
  - `matplotlib` and `seaborn` for data visualization
- **Jupyter Notebook** for running Python scripts interactively

## 🧩 Future Enhancements
- Add time-series analysis to explore trends in budget and revenue over the years.
- Expand the dataset to include more recent movies and additional features like streaming popularity.
- Implement machine learning models to predict gross revenue based on features like budget, rating, and genre.

---

## 🚀 Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/vsumitwork/movie-insights-analysis.git
   ```
2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Run the notebook and explore the visualizations and insights.

---

### 🌟 Contributions
Feel free to contribute by submitting a pull request or opening an issue. Suggestions for improving the analysis or adding new features are welcome!

