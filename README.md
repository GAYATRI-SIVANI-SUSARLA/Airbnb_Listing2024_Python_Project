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
The dataset is uploaded: [Airbnb dataset](https://github.com/GAYATRI-SIVANI-SUSARLA/Airbnb_Listing2024_Python_Project/blob/main/datasets.csv).

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
 - Visualized the count of each room type using **bar plots**.
 - Identified entire home/apt as the most common room type.
 
 **2. Neighbourhood group insights:**
   - Analyzed price variations by boroughs.
   - Manhattan had the highest average prices.
     
 **3. Availability trends:**
   - Used **heatmaps** to show correlations among `price`, `availability_365`, 
       `number_of_reviews`, and `beds`.
     
 **4. Price Distribution:**
 - Used **histograms** to show the distribution of prices.
    The majority of the listings were priced between $50 and $300.
 
 **5. Host listings:**
 - Analyzed hosts with multiple listings using **boxplots** to identify key contributors.
 
 **6. Review Behaviour:**
  - Used **pair plots** to show relationships between a number of reviews, price, and availability.

  
 ### Data Visualization
 - **Pairplot:** To see correlations among `price`, `availability`, `minimum nights`, and `number of reviews`.
   ![image](https://github.com/user-attachments/assets/54c75592-3b6d-44a6-9e0c-34f9c6ee4f3f)

 - **Heatmap:** Showing correlations among numerical features.
   ![image](https://github.com/user-attachments/assets/3374b97a-921d-4e40-a765-fe0db58349eb)

 - **Histograms & Boxplot:** To detect outliers in `price`
   ![image](https://github.com/user-attachments/assets/3ede359c-cbe0-48f7-a62e-4c0fdb783684)
   ![image](https://github.com/user-attachments/assets/32010d6d-f6fe-4bd1-a465-6558ec2b0ead)


 - **Bar Charts:** Displaying `room types` and `neighborhood group` distributions
  ![image](https://github.com/user-attachments/assets/ecfbe718-60ef-498c-a34d-39b0f236e90e)
- **Scatter Plot:** Geographical distribution of Airbnb with `latitude` and `longitude` concerning `room types`
  ![image](https://github.com/user-attachments/assets/3f7da110-0098-4cde-b7f8-8f2bf8a31a30)

  ## Key Findings & Insights
  1. **Price Trends:**
     - **Manhattan** has the most expensive listings, followed by Brooklyn.
     - **Entire homes/apartments** cost significantly more than private or shared rooms.
  2. **Room type Distribution:**
     - **Entire homes/apartments** are the most common, but **private rooms** offer budget- 
        friendly options.

  3. **Outliers in Price:**
      - Few listings priced at **$10,000+** were detected, indicating the need to filter such 
       extreme values.
     
  4. **Availability Patterns:**
    - Listings with **high availability** tend to have lower prices and more reviews, likely due to better guest experience
      
     
  5. **Host Behaviour:**
     - Some hosts manage **multiple listings**, indicating a trend toward professional hosting
    
 ## Install & Import Libraries
 Install the required libraries:
 ```python
 pip install pandas numpy matplotlib seaborn
 ```
Import the required libraries:
 ```python
 import pandas as pd
 import numpy as np
 import seaborn as sns 
 import matplotlib.pyplot as plt
 ```
## Recommendations
- **For Guests:**
   - Look for listings with high availability and good reviews for a better experience.
   - Private rooms in Brooklyn offer affordable stays compared to Manhattan.
- **For Hosts:**
   - Improve availability and review response rates to attract more bookings.
   - Manage pricing effectively to compete within the borough's market.
 
  ## Future Work
  - Use machine learning to predict prices based on room type and location.
  - Perform sentiment analysis on reviews to better understand guest experiences.
  - Create an interactive dashboard for live monitoring using Plotly or Power BI.
 
  ## Conclusion
  This project offers valuable insights into the New York Airbnb market, helping both guests and hosts make informed decisions. By using EDA techniques, we identified key trends and developed actionable recommendations. Future improvements can involve advanced analytics and predictive modeling to enhance the findings further.
  

   


 






















