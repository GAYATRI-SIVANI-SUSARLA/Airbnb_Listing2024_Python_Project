# Airbnb Listings EDA Project(New York 2024):
## Project Overview
This project performs Exploratory Data Analysis (EDA) on New York Airbnb Listing 2024 data to uncover trends and patterns in rental listings. We used Python Jupyter Notebook to do EDA and used libraries like Pandas, Numpy, Matplotlib, and Seaborn for cleaning, visualization, and analysis.
![AIRBNN NY](https://github.com/GAYATRI-SIVANI-SUSARLA/Airbnb_Listing2024_Python_Project/blob/main/Airbnb_NY.jpg)
## Objective 
The goal of this project is to:
1. Analyze room types, prices, and availability across different neighborhoods.
2. Understand host behavior and listing patterns.
3. Detect potential outliers in prices.
4. Provide recommendations for guests and hosts based on insights.

## Dataset
Dataset is uploaded: 
The dataset contains 20,765 entries and 22 features(columns), including:
- id: Unique identifier for each listing
- name: Title of the Airbnb listing
- host_name: Name of the host
- neighborhood_group: Group (borough) where the listing is located
- latitude/longitude: Geolocation of listings
- price: Nightly rental price
- room_type: Type of accommodation (e.g., entire home, private room)
- reviews_per_month: Average monthly reviews for the listing
- availability_365: Number of available days in the year

## Steps & Workflow
### 1. Data Cleaning 
- **Handle missing data:** `price`, `neighborhood`, and `beds` columns had null values.
- **Fix data types:** Converted `last_review` to a datetime object.
- **Remove outliers:** Listings with prices > $1,000 were capped to avoid skewed visualizations.
 ### 2. EDA(Exploratory Data Analysis)
 **1. Room type distribution:**






















