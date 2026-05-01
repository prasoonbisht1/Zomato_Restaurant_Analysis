# Zomato_Restaurant_Analysis

---

> **Note:** This project was developed as part of a data analysis course to simulate real-world business strategy consulting.

Does this summary align with the specific insights you'This README provides an overview of the **Zomato Restaurant Analysis** project, a data science objective aimed at deriving strategic insights for restaurant expansion.

---

## 🍴 Zomato Restaurant Analysis

Zomato is looking to expand its footprint by opening new establishments. This project analyzes existing restaurant data to provide data-driven strategies and suggestions for identifying the best opportunities for new openings.

### **Table of Contents**
1. [Project Objective](#project-objective)
2. [Dataset Overview](#dataset-overview)
3. [Workflow](#workflow)
4. [Key Features](#key-features)
5. [Installation & Requirements](#installation)

---

### **Project Objective** <a id="project-objective"></a>
The primary goal is to perform an Exploratory Data Analysis (EDA) on Zomato's global restaurant listings to determine:
*   Optimal locations for new restaurants.
*   Popular cuisines across different countries.
*   Price range segments with the highest growth potential.
*   Correlation between features like online delivery, table booking, and restaurant ratings.

---

### **Dataset Overview** <a id="dataset-overview"></a>
The analysis is performed on two primary datasets:
*   **Raw Data:** Contains details for over 9,500 restaurants, including location, cuisines, average cost, ratings, and service availability.
*   **Country Description:** A lookup table mapping country codes to country names (e.g., India, Australia, UAE, USA).

---

### **Workflow** <a id="workflow"></a>

#### **1. Data Cleaning and Preprocessing**
*   **Null Handling:** Removed missing values (specifically in the `Cuisines` column).
*   **Duplicate Check:** Verified dataset integrity by checking for duplicate records.
*   **Date Normalization:** Converted `Datekey_Opening` into standard datetime objects.

#### **2. Feature Engineering**
*   **Time Features:** Extracted `Year` and `Month` from opening dates to analyze seasonal trends.
*   **Data Merging:** Integrated country names into the main dataset via `CountryCode`.
*   **Boolean Mapping:** Converted categorical "Yes/No" flags (Delivery, Booking) into Boolean types for easier mathematical processing.
*   **Cost Binning:** Segmented restaurants into cost brackets (e.g., `0-275`, `275-550`, `1375+`) based on the Interquartile Range (IQR) to handle outliers.

#### **3. Exploratory Data Analysis (EDA)**
*   Statistical summary of prices and ratings.
*   Outlier detection using Seaborn boxplots.
*   Visualizing global distribution and price range distributions.

---

### **Key Features** <a id="key-features"></a>
*   **Global Scope:** Analysis covers 15 different countries.
*   **Financial Insights:** Identifies the "Average Cost for Two" across different regions.
*   **Operational Analysis:** Evaluates the impact of `Has_Online_delivery` and `Has_Table_booking`.

---
