# NYC Airbnb Data Analysis

## Project Overview
This project analyzes **New York City Airbnb listings** to uncover the key drivers of rental prices and neighborhood trends.  
The goal is to demonstrate end-to-end data analysis skills: from cleaning and exploration to modeling, visualization, and storytelling.

**Business Question:**  
What factors influence Airbnb prices in NYC, and how can hosts and travelers use these insights?

---

## Dataset
- **Source:** [NYC Airbnb Open Data (Kaggle)](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data)  
- **Size:** ~49,000 listings  
- **Features:** Borough, neighborhood, latitude/longitude, room type, price, minimum nights, reviews, availability  
- **Limitations:** Snapshot in time, no seasonal demand or booking data  

---

## Tools & Libraries
- **Python**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **Jupyter Notebook** for analysis workflow  
- **GitHub** for version control and reproducibility  

---

## Data Cleaning & Preparation
- Removed extreme outliers (listings > $1,000 per night)  
- Handled missing values in host names and reviews  
- Standardized categorical features (room type, borough)  
- Engineered new features:
  - Price per review  
  - Reviews per available day  
  - Borough grouping  

---

## Exploratory Data Analysis (EDA)
Key findings from descriptive statistics and visualizations:
- **Average price overall:** \$141.31  
- **Median price:** \$105.00  
- **Most expensive borough:** Manhattan (\$178.94)  
- **Most common room type:** Entire home/apartment (25,216 listings)  

**Visuals included:**
- Histogram of prices  
- Bar chart of average price per borough  
- Boxplot of price by room type  
- Correlation heatmap of numeric features  

---

## Modeling & Advanced Analysis
- **Methodology:** Linear regression to predict price  
- **Features used:** Room type, borough, number of reviews, availability, engineered features  
- **Evaluation metric:** RMSE (Root Mean Squared Error)  

**Result:**  
Room type and borough are the strongest predictors of price. Availability and reviews show weaker relationships.

---

## Results & Insights
**Key findings:**
- Room type effect: Entire homes/apartments typically price higher than private/shared rooms.  
- Location effect: Manhattan listings are significantly more expensive; Brooklyn trends more affordable.  
- Engagement proxies: Reviews and availability show weaker linear relationships to price.  

**Business implications:**
- **Hosts:** Price competitively by benchmarking within borough and room type; highlight amenities to justify premiums.  
- **Travelers:** Target Brooklyn/Queens for savings; filter by room type for better value.  

---

## Data Visualization & Storytelling
- Interactive map of listings by price (optional dashboard layer)  
- Bar chart of average price per borough  
- Scatterplot of price vs. number of reviews  

**Narrative:**  
“Airbnb in NYC is a tale of two cities — Manhattan for luxury, Brooklyn for affordability.”

---

## Recommendations & Next Steps
- **For hosts:** Adjust pricing strategies based on borough averages  
- **For travelers:** Compare boroughs to maximize value  
- **Future improvements:** Add seasonal demand data, booking trends, and sentiment analysis from reviews  
