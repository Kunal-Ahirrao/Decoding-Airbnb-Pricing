# Decoding Airbnb Pricing: Insights into Trends and Influencing Factors

## Group 9: Kunal Ahirrao, Praveen Bharathi

### 1. Background
New York City (NYC) is one of the world's most recognized and populous urban centers. With its five boroughs—Manhattan, Brooklyn, Queens, The Bronx, and Staten Island—NYC attracts millions of visitors annually, leading to a booming short-term rental market dominated by Airbnb. Understanding the factors affecting Airbnb pricing can provide valuable insights for hosts, travelers, and policymakers.

### 2. Motivation
- **Hosts:** Optimize listings to attract more bookings.
- **Travelers:** Find affordable accommodations.
- **Policymakers:** Manage Airbnb's impact on housing affordability and neighborhood dynamics.

### 3. Research Questions
1. **Neighborhood Trends:** What are the average prices across boroughs and neighborhoods?
2. **Room Type Analysis:** How does the average price vary by room type?
3. **Price and Reviews Relationship:** How does the number of reviews correlate with listing prices?
4. **Room Types in Top Neighborhoods:** Which room types are preferred in premium locations?
5. **Availability Impact on Pricing:** How does listing availability influence pricing trends?
6. **Characteristics of High- and Low-Priced Listings:** What factors contribute to pricing differences?

### 4. Dataset
- **Source:** [Inside Airbnb](https://insideairbnb.com/get-the-data/)
- **Dataset Size:** 37,541 rows, 18 columns
- **Key Columns:**
  - `neighbourhood_group` (borough)
  - `room_type`
  - `price`
  - `availability_365`
  - `number_of_reviews`

### 5. Methodology
#### 5.1 Data Cleaning
- Removed redundant columns (`license`, `number_of_reviews_ltm`).
- Handled missing values in `reviews_per_month` and `listing_name`.
- Applied **Interquartile Range (IQR)** method to remove price outliers.
- Renamed key columns for clarity.

#### 5.2 Data Transformation
- Encoded categorical variables.
- Created `price_per_day_available` as a new feature.

#### 5.3 Exploratory Data Analysis (EDA)
- Visualized price distributions using histograms.
- Analyzed borough-wise pricing trends.
- Assessed the correlation between reviews and pricing.

### 6. Results and Discussion
#### 6.1 Neighborhood Trends
- **Premium:** Manhattan (Tribeca, SoHo) has the highest Airbnb prices.
- **Budget-Friendly:** The Bronx and Staten Island offer lower-priced listings.
- **Mixed Pricing:** Brooklyn and Queens provide a range of pricing options.

#### 6.2 Room Type Analysis
- **Entire Homes:** Most expensive, commonly found in Manhattan.
- **Private Rooms:** Moderately priced, common in Brooklyn and Queens.
- **Shared Rooms:** Most affordable, limited availability.

#### 6.3 Price and Reviews Relationship
- Listings with fewer reviews tend to have higher prices.
- High-reviewed listings are moderately priced, indicating guest engagement.

#### 6.4 Room Types in Top Neighborhoods
- Premium neighborhoods favor **entire apartments**.
- Private rooms are more common in **Williamsburg (Brooklyn) and Astoria (Queens)**.
- Shared rooms are primarily available in budget-friendly areas.

#### 6.5 Availability Impact on Pricing
- **Year-round listings (365 days)** exhibit lower prices due to competition.
- **Seasonal listings** leverage high-demand periods for higher pricing.

#### 6.6 Characteristics of High- and Low-Priced Listings
- **High-priced:** Entire apartments in premium areas with high availability.
- **Low-priced:** Private/shared rooms with fewer reviews and lower availability.

### 7. Lessons Learned
- **Data Cleaning is Crucial:** Handling missing values and outliers significantly improves analysis quality.
- **Visualization Enhances Insights:** Boxplots and histograms helped identify trends.
- **Market Dynamics Matter:** Room types, availability, and reviews impact pricing strategies.

### 8. Future Improvements
- **Advanced Statistical Modeling:** Implement machine learning for price prediction.
- **Integration of External Data:** Include factors like seasonality and local events.
- **Stakeholder Collaboration:** Work with real estate experts for deeper insights.

### 9. Conclusion
This project provided an in-depth analysis of Airbnb pricing in NYC, identifying key trends and influencing factors. The insights gained can help hosts, travelers, and policymakers make data-driven decisions to optimize Airbnb usage in urban environments.

