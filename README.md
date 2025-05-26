# Exploring Trends in Housing Prices

Analysis of factors from a Kaggle data set.

**Team Members:**

| Project Contributer | Project Role |
|:--------:|:--------------|
| Jonathan Barron | Project Manager |
| Tammy Garcia | Data Analyst |
| Tiffani Lambert | Data Analyst |
| Precious Ufomadu | Data Analyst |

**Tech Stack:**

* **Backend:** Python
* **Data Science:** Pandas, Matplotlib

**Project Structure:**

``` bash
Project Structure/
|
|--- data/              # Data files (e.g., raw, extracted, transformed)
|--- notebooks/         # Jupyter notebooks with analysis
|--- assets/            # Media files (e.g., README images, analysis visualizations)
|
|--- .gitignore         # Git ignore rules
|--- README.md          # Project documentation


# Before running this project locally, ensure you have the following installed:
* IDE (VS Code, PyCharm, etc.)
* Install Python 3.10+ version > visit https://www.python.org/downloads/


# Install dependencies
pip install pandas matplotlib

```

## Project Overview

[Dataset used from Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/overview) contained 79 explanatory variables for property sales in Ames, Iowa. Two files were combined for a total of 2,919 transaction records. EDA of data was conducted in separate Jupyter notebook files by team members.

## Insights Overview

**Q1: What is the distribution of house sale prices in the market?**
     
**Answer:** Based on the histogram with the KDE curve, the sales price is right-skewed, showing that most housing prices fall between $100,000 to $250,000 which is below the average. The observed graph also shows some outliers on the higer end that are above $500,000. It is important to note that the dataset used is from 2016, as such current market prices post COVID is not reflected.

**Q2: What patterns exist in property sale prices by zoning classification from 2007 to 2010?**

**Answer:** Property sale volumes peaked in 2007 with 692 transactions and declined to a low of 339 in 2010. Sales remained above 620 in other years. The top three categories by volume were always Residential Low Density (RL), Residential Medium Density (RM), and Floating Village Residential (FV). RL outpaced RM in volume by a low and high of 3.7x (2008) and 6.2x (2009), respectively. The two zoning categories with the least transactions were always Residential High Density (RH) and Commercial (C), together accounting for only 1.2% to 2.9% of annual sales volume.

**Q3: How are the YearRemodAdd and Heating columns related?**

**Q4: What is the relationship between property functionality and property full bath amounts?**

**Q5: How does the number of garage cars significantly influence house prices?**

**Answer:** The number of garage cars statistically significantly influences house prices. A correlation matrix showed that GarageCars (r = 0.64) had the strongest positive correlations with SalePrice, indicating a moderate relationship. 
A boxplot showed that median house prices increase consistently from 0 to 3-car garages, with a notable jump for 3-car garages—homes in this category had the highest median sale prices and the widest price range, including many high-end outliers. 
Although other features like porch size or pool area showed little correlation, the Pearson correlation test between GarageCars and SalePrice produced a p-value of 0.000 (p < 0.05), confirming the relationship is statistically significant. This suggests that homes with larger garage capacity tend to command higher prices, though other factors also contribute.

## Credits & Contributions

[The Knowledge House](https://www.theknowledgehouse.org/) provided the project requirements for this project. Contributions are welcome! Feel free to submit a pull request to improve the project or open a issue to report any problems.
