# Airbnb_Analysis


### **Overview**

The Airbnb Listings Data Analysis project focused on exploring a large dataset of Airbnb listings to extract insights about pricing, room types, neighborhood popularity, and user engagement. Executed using **Python in Google Colab**, this project employed tools such as **Pandas**, **NumPy**, **Matplotlib**, and **Seaborn** for end-to-end data exploration, cleaning, transformation, and visualization. The goal was to answer key analytical questions and support stakeholders in understanding platform usage and performance trends.

---

### **Project Objectives**

The core objectives of the project were to:

* Perform exploratory data analysis on Airbnb listings data.
* Clean and preprocess the dataset to handle missing and inconsistent values.
* Answer business questions related to pricing, room type distribution, and customer engagement.
* Visualize the results to reveal trends and patterns across time and geography.

---

### **Data Processing and Analysis**

#### **Data Preparation**

* **Data Import**: Imported a CSV file (`compressed_data.csv`) containing 100,000+ Airbnb listings into a Pandas DataFrame.
* **Initial Inspection**: Used `.info()` and `.isnull().sum()` to inspect column data types and missing values.
* **Data Cleaning**:

  * Converted the `last review` column to datetime.
  * Filled missing values in `reviews per month` with 0, and `last review` with the earliest date.
  * Removed rows with missing critical identifiers like `NAME` and `host name`.
  * Dropped columns with excessive missing data: `house_rules` and `license`.
  * Standardized and converted `price` and `service fee` from strings to float.
* **Data Deduplication**: Removed duplicate rows to maintain data integrity.

#### **Descriptive Statistics**

* Generated summary statistics using `.describe()` to understand distributions and identify anomalies (e.g., extreme values in `price`, `minimum nights`, and `availability`).

---

### **Key Business Questions and Insights**

1. **What is the distribution of listing prices?**

   * A histogram revealed that most listings were priced below \$1,000, with a long tail representing high-end or outlier listings.

2. **How are the different room types distributed?**

   * Count plot analysis showed that "Entire home/apt" and "Private room" were the most commonly listed room types.

3. **How are listings distributed across different neighborhoods?**

   * Neighborhood group analysis highlighted which city areas had the highest concentration of listings, providing insights for potential marketing or operational focus.

4. **What is the relationship between price and room type?**

   * Box plots indicated that "Entire home/apt" listings typically command higher prices, while "Shared rooms" had the lowest price distribution.

5. **How has the number of reviews changed over time?**

   * A time series line plot showed trends in user engagement and platform activity by tracking the number of reviews per month.

---

### **Visualizations**

The project featured several informative plots:

* **Histogram** for price distribution.
* **Count plots** for room types and neighborhood group distributions.
* **Box plot** to analyze the relationship between room type and price.
* **Line plot** to show the temporal trend of reviews over months.

---

### **Insights and Conclusions**

* **Price Sensitivity**: The majority of listings are priced within an affordable range; outliers skew the average.
* **Room Type Preferences**: Users favor entire apartments or private rooms, reflecting demand for privacy.
* **Neighborhood Density**: Certain city areas have higher listing densities, likely due to tourist hotspots.
* **Temporal Engagement**: Fluctuations in review count over time reveal seasonal trends and user activity cycles.
* **Data Quality Challenges**: The dataset had significant missing values and outliers that required careful preprocessing.

---

### **Tools Used**

* **Python (Google Colab)**: Primary platform for analysis.
* **Pandas & NumPy**: Data cleaning, manipulation, and statistics.
* **Matplotlib & Seaborn**: Data visualization and plotting.

---

### **Key Takeaways**

This project highlights how structured data analysis can deliver valuable insights into user behavior, pricing strategies, and product offerings on a platform like Airbnb. By identifying trends, preferences, and anomalies, the analysis empowers decision-makers to improve user experience, pricing models, and operational planning.
