# 🏠 Airbnb Toronto 2019 Data Cleaning and Preprocessing

This project focuses on cleaning and preparing Airbnb listings data from **Toronto in 2019**. It was developed as part of the **Oasis Infobyte Internship Program (OIBSIP)** to demonstrate essential data preprocessing skills required for high-quality data analysis and modeling.

---

## 📌 Project Objectives

The core objective of this task is to ensure data quality and consistency through a series of systematic data preprocessing steps. Specific goals include:

- **Data Integrity**: Ensure the dataset is accurate, reliable, and consistent during the cleaning process.
- **Missing Data Handling**: Address null or missing values with appropriate imputation strategies or decisions based on data context.
- **Duplicate Removal**: Identify and remove redundant records to prevent analysis bias.
- **Standardization**: Apply uniform formatting (e.g., date formats, price formatting) and consistent units for seamless analysis.
- **Outlier Detection**: Locate and treat outliers that may distort statistical analysis or model outcomes.

---

## 📁 Dataset Overview

The dataset contains Airbnb listings data from **Toronto, Canada** for the year **2019**, with the following key columns:

- **id**: Unique identifier for each listing
- **name**: Title of the listing
- **host_id**: Unique ID of the host
- **neighbourhood_group**: Administrative area (not always populated)
- **neighbourhood**: Local area of the listing
- **latitude` & `longitude**: Geographic coordinates
- **room_type**: Type of room (e.g., Entire home, Private room)
- **price**: Price per night (CAD)
- **minimum_nights**: Minimum nights required per bookin
- **number_of_reviews**: Total number of reviews
- **last_review**: Date of the most recent review
- **reviews_per_month**: Average reviews per month
- **calculated_host_listings_count**: Total listings by the host
- **availability_365**: Availability of the listing in days per year

---

## 🔧 Tools

- **Python** for scripting and data manipulation
- **Pandas** – for data cleaning, transformation, and analysis
- **NumPy** – for numerical operations
- **Interquartile Range(IQR)**-For identifying outliners.
- **Matplotlib**/**Seaborn** – for data visualization
- **Google Colab** – for documenting and running code

---

## 🧹 Data Cleaning Steps

1. **Data Integrity Checks**
   - Checked column data types, shape, and summary statistics.
   - Validated categorical values and range of numerical fields.

2. **Handling Missing Values**
   - Imputed missing values in `reviews_per_month` with 0.
   - Dropped rows with critical missing identifiers when necessary (e.g., `name`, `host_id`).

3. **Duplicate Removal**
   - Identified and removed duplicate entries based on `id` and other key attributes.

4. **Standardization**
   - Ensured consistency in room type values and price formatting.
   - Converted `last_review` to datetime format.
   - Normalized strings for uniformity.

5. **Outlier Detection**
   - Detected outliers in `price`, `minimum_nights`, and `availability_365`.
   - Used boxplots and statistical thresholds to isolate extreme values.
   - Treated or removed data points that could skew results.

---

## 📊 Visualizations Included

- Boxplots for spotting outliers in numerical columns

  
