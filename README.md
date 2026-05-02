# 🍴 Zomato Restaurant Analysis

This project performs a comprehensive Exploratory Data Analysis (EDA) on Zomato's global restaurant data to uncover market trends, consumer behavior and find best location for opening new restaurant.

---

## 📊 Key Insights & Findings

Based on the analysis conducted in the Jupyter Notebook, the following data-driven insights were identified:

### **1. Global Market Presence**
*   **India Dominance:** India has the largest presence in the dataset, with the highest number of restaurant listings compared to other countries.
*   **City Hotspots:** Within India, the majority of the data is concentrated in the National Capital Region (NCR), specifically New Delhi, Gurgaon, and Noida.

### **2. Rating Patterns**
*   **Average Performance:** The most frequent rating for active restaurants ranges between **2.5 and 3.5**, which is categorized as "Average."
*   **Quality Distribution:** High-tier ratings (4.6–5.0) are rare, representing a small, elite percentage of the total restaurant count.

### **3. Service & Operational Impact**
*   **Online Delivery Advantage:** Restaurants that offer **Online Delivery** generally maintain higher aggregate ratings than those that do not.
*   **Table Booking Premium:** Establishments providing **Table Booking** facilities are frequently associated with higher price ranges and "Excellent" or "Very Good" rating categories.

### **4. Cuisine & Cost Trends**
*   **Top Cuisines:** **North Indian** is the most popular cuisine by volume, followed by **Chinese** and **Fast Food**.
*   **Price vs. Satisfaction:** The "Mid-Range" price categories (Price Range 2 and 3) contain the most balanced distribution of high ratings.
*   **Luxury Gap:** A higher "Average Cost for Two" does not linearly correlate with a higher rating, suggesting that customer satisfaction is driven by value and quality rather than price alone.

---

## 🛠️ Project Workflow

### **Data Cleaning & Preprocessing**
*   **Dataset Integration:** Merged the primary Zomato dataset with the `Country-Code` lookup table.
*   **Null Handling:** Cleaned missing values in the `Cuisines` column to ensure categorical accuracy.
*   **Feature Engineering:** Extracted Year, Month, and Quarter from opening dates to analyze growth trends over time.

### **Techniques Used**
*   **Categorical Analysis:** Grouping by Country, City, and Rating to see distribution patterns.
*   **Numerical Aggregation:** Analyzing mean costs and the relationship between votes and ratings.
*   **Visualization:** Created bar charts for top cuisines, and pie charts for market share using Matplotlib and Seaborn.

---

## 📂 File Structure
*   `Zomato_Restaurant_Analysis.ipynb`: Main Jupyter Notebook containing all Python code and visualizations.
*   `Zomato_Data_1.xlsx`-`Raw Data`: The raw restaurant dataset.
*   `Zomato_Data_1.xlsx`-`country description`: Mapping file for country names and codes.
*   `README.md`: Project documentation and findings summary.

---

