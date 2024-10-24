# Airbnb Listings EDA Project: New York 2024

## Project Overview
This project conducts an **Exploratory Data Analysis (EDA)** on Airbnb listings in New York to uncover trends and patterns in rental data. It utilizes Python libraries like **Pandas, Numpy, Matplotlib, and Seaborn** for data cleaning, visualization, and analysis.

## Objective
The primary goals of this project are to:
- Analyze room types, prices, and availability across different neighborhoods.
- Understand host behavior and listing patterns.
- Detect potential outliers in prices.
- Provide recommendations for guests and hosts based on insights.

## Dataset
The dataset contains **20,765 entries** and **22 features**, including:
- `id`: Unique identifier for each listing
- `name`: Title of the Airbnb listing
- `host_name`: Name of the host
- `neighborhood_group`: Group (borough) where the listing is located
- `latitude`, `longitude`: Geolocation of the listings
- `price`: Nightly rental price
- `room_type`: Type of accommodation (e.g., entire home, private room)
- `reviews_per_month`: Average monthly reviews for the listing
- `availability_365`: Number of available days in a year

## Steps and Workflow

### 1. Data Cleaning
- **Handle Missing Data**: Addressed null values in `price`, `neighborhood`, and `beds` columns.
- **Fix Data Types**: Converted `last_review` to a datetime object.
- **Remove Outliers**: Capped listings with prices > $1,000 to avoid skewed visualizations.

### 2. EDA (Exploratory Data Analysis)
- **Room Type Distribution**: 
  - Visualized the count of each room type using bar plots.
  - Found that "Entire home/apartment" is the most common room type.
  
- **Neighborhood Group Insights**:
  - Analyzed price variations across boroughs.
  - **Manhattan** had the highest average prices.

- **Availability Trends**:
  - Used heatmaps to show correlations among `price`, `availability_365`, `number_of_reviews`, and `beds`.

- **Price Distribution**:
  - Used histograms to display price distributions, with most listings priced between $50 - $300.

- **Host Listings**:
  - Analyzed hosts with multiple listings using boxplots to identify key contributors.

- **Review Behavior**:
  - Used pair plots to explore relationships between `number_of_reviews`, `price`, and `availability`.

### 3. Data Visualization
- **Pairplot**: Explored correlations among `price`, `availability`, and `number_of_reviews`.
- **Heatmap**: Showed correlations among numerical features.
- **Histograms and Boxplots**: Detected outliers in `price`.
- **Bar Charts**: Displayed distributions of room types and neighborhood groups.

## Key Findings and Insights

- **Price Trends**:
  - Manhattan has the most expensive listings, followed by Brooklyn.
  - Entire homes/apartments are significantly pricier than private or shared rooms.

- **Room Type Distribution**:
  - Entire homes/apartments are the most common, but private rooms offer more budget-friendly options.

- **Outliers in Price**:
  - A few listings were priced above $10,000, which suggests filtering of extreme values is necessary.

- **Availability Patterns**:
  - Listings with higher availability tend to have lower prices and more reviews, possibly indicating better guest experiences.

- **Host Behavior**:
  - Some hosts manage multiple listings, indicating a trend toward professional hosting.

## How to Run This Project

1. **Clone the repository**:
   ```bash
   git clone https://https://github.com/chiranjeev1cd/air_bnb_da.git
