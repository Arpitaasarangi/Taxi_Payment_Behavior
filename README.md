🚕#Taxi_Payment_Behavior
A Hypothesis-Driven Analysis of Fare Amounts by Payment Type

#📌Project Overview
This project investigates whether the method of payment (Card vs. Cash) influences the total fare amount in NYC taxi rides. Using Python, descriptive statistics, and hypothesis testing, I explored patterns in fare behavior to help taxi drivers identify which payment types may lead to higher earnings.

🎯 Problem Statement
Our research aims to determine whether payment methods have an impact on fare pricing by focusing on the relationship between payment type and fare amount.

🧪 Objective
To conduct an A/B test comparing total fare amounts between card and cash payments. The goal is to extract actionable insights that can help taxi drivers generate more revenue without negatively impacting customer experience.

❓ Research Question
Is there a relationship between total fare amount and payment type — and can we nudge customers toward payment methods that generate higher revenue for drivers?

📁 Dataset Columns
- VendorID
- tpep_pickup_datetime, tpep_dropoff_datetime
- passenger_count, trip_distance, RatecodeID
- store_and_fwd_flag, PULocationID, DOLocationID
- payment_type, fare_amount, extra, mta_tax, tip_amount, tolls_amount, improvement_surcharge, total_amount, congestion_surcharge
- duration (calculated in minutes)

🛠️ Tools & Libraries
- Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy)
- Jupyter Notebook
- Statistical Testing: QQ Plot, Histogram, t-test

🔍 #Workflow Summary
#1. Data Loading & Cleaning
- Loaded NYC taxi dataset
- Converted pickup and dropoff columns to datetime
- Calculated trip duration in minutes
- Removed extra spaces and unwanted columns
- Checked and dropped nulls and duplicates
- Replaced encoded payment_type values (1 → Card, 2 → Cash)
  
#2. Exploratory Data Analysis (EDA)
- Descriptive statistics of fare and trip data
- Outlier detection using boxplots and histograms
- Payment type distribution visualized via pie chart
- Passenger count percentages calculated
- Created a new DataFrame to store payment type distributions
  
#3. Normality Check
- Used histograms and QQ plots to assess normality of fare distributions
- Found that fare amounts are not normally distribute
  
#4. Hypothesis Testing
- Null Hypothesis (H₀): No difference in average fare between card and cash users
- Alternative Hypothesis (H₁): There is a difference in average fare between card and cash users
- Performed independent t-test
- Result: p-value < 0.05 → Reject the null hypothesis

#📈 Key Insight
💳 Card payments are statistically associated with higher average fares than cash payments.
This suggests that encouraging card usage could help taxi drivers increase revenue without changing the customer experience.

