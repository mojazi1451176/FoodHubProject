# FoodHubProject

# FoodHub Orders Analysis

## Project Overview
This project explores and analyzes customer orders from FoodHub using Python and various data analysis libraries. The dataset contains details about orders, customers, restaurants, cuisine types, order costs, ratings, food preparation time, and delivery time.

## Dataset
The dataset consists of **1,898** orders with **9** columns:
- `order_id`: Unique identifier for each order
- `customer_id`: Unique identifier for each customer
- `restaurant_name`: Name of the restaurant
- `cuisine_type`: Type of cuisine offered
- `cost_of_the_order`: Total cost of the order
- `day_of_the_week`: Indicates whether the order was placed on a weekday or weekend
- `rating`: Customer rating (including "Not given")
- `food_preparation_time`: Time taken to prepare the food (in minutes)
- `delivery_time`: Time taken to deliver the order (in minutes)

## Libraries Used
- `numpy` - For numerical computations
- `pandas` - For data manipulation and analysis
- `matplotlib.pyplot` - For data visualization
- `seaborn` - For advanced data visualization

## Exploratory Data Analysis (EDA)
### 1. Understanding Data Structure
- `df.shape`: Displays the number of rows and columns
- `df.info()`: Shows data types and missing values
- `df.describe(include='all')`: Provides summary statistics
- `df.isnull().sum()`: Checks for missing values

### 2. Data Visualization
- **Bar Plots**:
  - Cuisine type distribution
  - Orders per day of the week
  - Ratings distribution
- **Histograms**:
  - Cost of orders
  - Delivery time
- **Boxplots**:
  - Cost of orders (to identify outliers)
  - Delivery time
  - Food preparation time by cuisine type
  - Cost of orders by cuisine type
  - Delivery time by day of the week
- **Point Plots**:
  - Relationship between rating and delivery time
  - Relationship between rating and cost of orders
  - Relationship between rating and food preparation time
- **Heatmap**:
  - Displays correlation between numerical features

### 3. Key Insights
- **Most orders are placed on weekends**
- **Shake Shack** receives the highest number of orders
- **American cuisine** is the most popular
- **29.24% of orders cost more than $20**
- **Average delivery time is ~24.16 minutes**
- **Southern cuisine has the widest range of costs**
- **Weekday deliveries take longer than weekends**
- **Lower delivery time correlates with higher ratings**
- **Higher cost orders generally have better ratings**

## Usage Instructions
1. Load the dataset using `pandas.read_csv()`.
2. Perform initial exploration using `.info()`, `.shape()`, `.describe()`.
3. Use visualizations to analyze key trends.
4. Interpret insights and apply them to decision-making.

## Future Work
- Investigate outliers in food preparation time
- Explore customer ordering patterns
- Predict delivery time using machine learning

## Author
Mo Jazi
