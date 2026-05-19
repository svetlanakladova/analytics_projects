## Moscow Food Market Analysis

### Project Overview

This project analyzes the food and beverage market in Moscow using data from Yandex Maps and Yandex Business (summer 2022).

The goal is to help investors choose the best type of restaurant and location for opening a new food service business.

Has been studied how the market is structured, how competitive it is, and what factors affect ratings, prices, and restaurant size.


### Project Goal

To analyze the Moscow restaurant market in order to identify:

- Understand the structure of Moscow’s food service market
- Analyze competition between different types of venues
- Study restaurant characteristics (rating, size, price, location)
- Explore price segments across the city
- Provide business recommendations for investors

---

### Contents

**1. Data Loading and Initial Exploration**
- Data Overview
- Merging into a Single DataFrame
  
**2. Data Preprocessing**
- Data Types
- Missing Values
- Duplicate Records (Explicit and Implicit)
- Intermediate Conclusion
  
**3. Exploratory Data Analysis**
- Types of Establishments
- Distribution by Districts
-3 Chain vs Independent Businesses
- Number of Seats
- Ratings Analysis
- Correlation of Ratings with Other Features
- Top 15 Most Popular Chains in Moscow
- Average Bill Analysis
- Intermediate Conclusion
  
**4. Final Conclusions and Recommendations**
- Overview of the Work Done
- Key Findings
- Data-Based Recommendations


### Key Insights

- Moscow market is dominated by cafes, restaurants, and coffee shops
- Central district is the most competitive and expensive area
- Chain businesses are common but not dominant
- Restaurant size depends strongly on category
- Higher prices usually mean higher ratings
- Location strongly influences pricing and business type


### Recommendations:

**1. Best business types**
- `Cafe` → safest and most flexible option
- `Restaurant` → best for premium strategy
- `Bar` → good for nightlife areas

**2. Best locations**
- `Central` & `Western districts` → premium and expensive restaurants
- `Eastern` & `South-Eastern districts` → budget-friendly cafes and fast food

**3. Pricing strategy**
- Premium places should clearly show pricing and focus on quality
- Budget places should focus on promotions and fast service

**4. Size planning**
- `50–90` seats is optimal for most restaurants
- Smaller venues work better for cafes and coffee shops

**5. Chain strategy**
- `Chains` are popular in cafes and restaurants
- But quality control is important — `chain` status does not guarantee high ratings


---

### Dataset Description

Two datasets were used:

The dataset `rest_info.csv` сontains information about restaurants:

- `name` — restaurant name  
- `address` — location  
- `district` — administrative district of Moscow  
- `category` — restaurant type (cafe, restaurant, etc.)  
- `hours` — working hours  
- `rating` — user rating (1–5 scale)  
- `chain` — `1` if chain restaurant, `0` otherwise  
- `seats` — number of seats  

The dataset `rest_price.csv` сontains pricing information:

- `price` — price category (low, medium, high, etc.)  
- `avg_bill` — textual description of average bill range  
- `middle_avg_bill` — numeric average bill (processed)  
- `middle_coffee_cup` — coffee cup price (derived field) 


---

### Tools & Technologies

`Python` `Pandas` `Seaborn` `Matplotlib` 
