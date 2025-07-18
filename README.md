# 🍽️ Zomato Insights Dashboard – Power BI

This Power BI project presents a detailed analysis of Zomato restaurant data to uncover insights related to customer ratings, location-based trends, cuisine popularity, and online ordering behavior. The dashboard is built to assist food industry stakeholders, marketers, and analysts in understanding restaurant performance and user preferences.

---

## 📁 Dataset

**Source:** Zomato Restaurant Dataset  
**Format:** Excel/CSV (Uploaded to Power BI)  
**Fields Include:**
- Restaurant Name
- Location
- Country Code
- Cuisines
- Aggregate Rating
- Price Range
- Online Order (Yes/No)
- Delivery (Yes/No)
- Votes

📦 **Dataset Download:** [Click Here to Download Dataset](https://drive.google.com/file/d/1HZr9wtAp8FZrc9k9rrQ2B5UmXW_Ly61o/view?usp=sharing)

---

## 📊 Dashboard Overview

The dashboard is divided into **3 interactive pages** to explore different business dimensions.

### 📄 Page 1: Global Restaurant Overview
- KPIs: Total Restaurants, Average Rating, Total Countries, Total Votes
- Column Chart: Restaurants by Country
- Card: Highest Rated Country
- Donut Chart: Rating Distribution
- Slicers: Country, City, Cuisine

### 📄 Page 2: Location & Cuisine Analysis
- Tree Map: Restaurants by City
- Bar Chart: Cuisine Popularity by City
- Table: Top-Rated Restaurants (Dynamic with filters)
- Slicers: Online Order, Delivery, Price Range

### 📄 Page 3: Ratings & Pricing Trends
- Clustered Column: Price Range vs Average Rating
- Scatter Plot: Rating vs Votes
- Matrix: City vs Cuisine vs Rating
- Filters: Rating Range, Price Level

---

## 📈 Key KPIs and DAX Measures

```DAX
Total Restaurants = COUNT('Zomato'[Restaurant ID])
Average Rating = AVERAGE('Zomato'[Aggregate Rating])
Total Countries = DISTINCTCOUNT('Zomato'[Country])
Total Votes = SUM('Zomato'[Votes])
