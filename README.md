# Canada Housing Prices Analysis

This project performs analysis of key factors 
affecting housing prices in Canada through 
exploratory data analysis, statistical testing 
and machine learning validation.

## Objective

The goal of this project is to explore how
property characteristics (number of bedrooms,
population size, median family income etc.) relate to 
housing prices across provinces of Canada.

## Dataset
- Source: Kaggle — Canadian house prices for top cities
  (https://www.kaggle.com/code/ryotapy/canadian-house-prices-for-top-cities/input).

- ~35,000 listings.
- Features include location, median family income, 
population, price, number of bedrooms and bathrooms.

## Methodology
- Data cleaning and validation.
- Exploratory data analysis (EDA)
- Hypothesis-driven analysis.
- Statistical testing (one-way ANOVA).
- Machine learning (Random Forest) for 
validation of EDA results.

## Key findings
- Housing prices increase with both the number of bedrooms and bathrooms,
  with bathrooms showing a stronger association.
- Province-level differences are 
statistically significant (ANOVA, p < 0.05).
- Population size correlates with listing density, but not fully with price levels.
- Extreme values (large properties) are rare and introduce noise into mean-based metrics.

## Machine learning validation
The model (using Random Forest method) was 
trained to validate findings of EDA. 
According to this model, the most important 
factors are Province and City-level 
features, which is supporting the relevance of 
location-based effects identified earlier.

## Limitations
- Uneven data coverage across provinces (e.g., Quebec underrepresentation)
- Skewed price distribution
- No temporal dynamics included

## Tools
- Python (pandas, numpy)
- Data visualization: matplotlib, seaborn
- Statistics: scipy
- Machine learning: scikit-learn

## Instructions
- Use your path to the dataset in this part:
"df = pd.read_csv(r"[YOUR PATH TO DATASET]", encoding='latin1')"
