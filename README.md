# Hotel_Booking_EDA_Project
# **Project Summary -**

* This hotel booking analysis project aimed to enhance booking efficiency , predict guest preferences, and tailor hotel offerings to better meet market demands. The purpose of this exploratory data analysis (EDA) is to analyze customer data, uncover patterns in booking behavior, and identify key trends and  correlations
* This project is divided into five parts:
  1. Knowing Data
  2. Understanding dataset  Variables
  3. Data Wrangling
  4. Data Visualization, Storytelling & Experimenting with charts : Understanding  the relationships between variables and finding  insight
  5. Solution to Business Objective and  Conclusion
* In first step knowing data i find below information about dataset:

  *  In this project  dataset  have 119390 rows and 32 columns and this dataset include customer booking information.
  * All the columns are categorized into three data types: object, float64, and int64.
  * The column  present in dataset are  'hotel', 'is_canceled', 'lead_time', 'arrival_date_year','arrival_date_month', 'arrival_date_week_number','arrival_date_day_of_month', 'stays_in_weekend_nights','stays_in_week_nights', 'adults', 'children', 'babies', 'meal','country', 'market_segment', 'distribution_channel','is_repeated_guest', 'previous_cancellations','previous_bookings_not_canceled', 'reserved_room_type','assigned_room_type', 'booking_changes', 'deposit_type', 'agent','company', 'days_in_waiting_list', 'customer_type', 'adr','required_car_parking_spaces', 'total_of_special_requests''reservation_status', 'reservation_status_date
  * The dataset contains **31,994** duplicate rows and missing values in the **Company (112,593), Agent (16,340), Country (488), and Children (4)** columns.
* The second step was understanding the variables. I used the describe() method to analyze the central tendency and dispersion of the data. Additionally, I identified the unique values for each variables.
* Third step data wrangling involves data cleaning,handling outlier and variable classification,and last data transformation
  * In the Data Cleaning part, I dropped the **Company** column because  it had more than 50% null values and also  replaced null values with appropriate data types in the **Children, Agent, and Country** columns.Furthermore, I removed duplicate and inappropriate rows to ensure data quality and accuracy.
  * Variable classification and outlier handling step, I categorized the variables into categorical, numerical, discrete numerical, and continuous variables. The dataset contained 12 categorical variables, 19 numerical variables, 17 discrete numerical variables, and 2 continuous variables. Additionally, in the continuous variables, the columns **ADR** and **Lead Time** contained potential outliers, which I handled using the IQR (Interquartile Range) method.
  * In the data transformation phase, I converted dataset variables into appropriate data types. Further, I added some columns to the dataset to make it easier to use in data visualization and finding insights. The columns I added are **lead_time_classification, total_stay, total_people, total_children, is_room_assigned_as_mentioned,** and **guest_type.**
* The most important step in EDA is **Data Visualization**, experimenting with charts, understanding the relationships between variables, and finding insights. In this step, I plotted between different variable  simple charts like **bar chart, grouped bar chart, scatter plot, box plot, heatmap,** and **pairplot.** Based on these graphs, I extracted insights and performed **univariate, bivariate, and multivariate analysis.** .After data visualization, I discovered amazing and  highly useful insights, which are  few  listed below.
  *  City hotels are more preferred than resort hotels .
  * The most number of customers arrived in August, followed by July and May. The least number of customers arrived in January.
  * Most number of served meal type is BB after SC
  * Most bookings are for short-duration stays, as the majority of customers are transient travelers.
  * Most people do not required car parking space
  * In 2016, 33.3% more bookings were made compared to 2015. After 2017, this dropped to 12.2%
  * The highest number of bookings were made in 2016, followed by 2017 and 2015.
  * Bookings are higher on weekdays compared to weekends, with more reservations made on weekdays.
  * City hotels are more prone to cancellations than resort hotel
  * Longer stays are associated with lower ADR
  * The most frequently booked number of nights is 3, followed by 2, 1, and 4. Very few people book stays longer than 7 nights.
  * People from Portugal (PRT) made the most bookings, followed by Great Britain (GBR) and France (FRA) and  also the highest revenue (ADR) was also generated by Portugal (PRT), followed by Great Britain (GBR) and France (FRA).

   These are some important insights which i mentioned  there are also many other insights I discovered in this project.
* Overall this project provided valuable insights into hotel booking patterns. However, we faced challenges like handling duplicate and missing data and selecting effective visualizations. Despite this, our findings can help improve booking efficiency and customer satisfaction.

# **Problem Statement**
  
 The hospitality industry faces challenges in understanding customer booking behavior, predicting guest preferences, and optimizing hotel offerings to improve business efficiency. This project aims to analyze hotel booking data to uncover key trends, identify factors affecting cancellations, and explore patterns in customer preferences.  
# **Business Objective**
 The business objective of this project is to analyze hotel booking patterns to improve booking efficiency,finding factor affecting cancellation, predict guest preferences, and optimize hotel offerings

# **Solution to Business Objective**

* City hotels are more preferred than resort hotels focusing on city hotel offerings, promotions, and services can increase customer satisfaction and revenue.
* With 27.5% of customers canceling bookings, introducing non-refundable booking options with slight discounts could help reduce cancellations.
* Most customers do not require parking spaces, hotels can optimize space utilization and reduce costs. Eliminating unnecessary parking spaces, such as 3 and 8 cars spaces and  keeping only 1 or 2 car spaces, can improve cost efficiency and allow for better use of available space
* Since most customers book in advance, hotels should offer discounts and special deals for bookings made at least 90 days ahead.
* The high customer arrival in August, July, and May indicates opportunities for targeted marketing and special offers during these peak months, while addressing lower occupancy in January with off-season promotions.
* Since BB (Bed & Breakfast) is the most popular meal plan, hotels should enhance breakfast quality and variety to improve guest satisfaction.
* With 59.1% of bookings coming from Online Travel Agents (OTAs), hotels should partner with more OTAs and offer exclusive deals for direct website bookings to reduce commission costs.
* Since most bookings are made by new customers, hotels should introduce  discounts, or special perks for returning guests to increase repeat bookings.
* Rooms A and D are the most popular, the hotel should maintain their quality, ensure availability during peak seasons, and enhance them with premium services to attract more bookings and improve guest satisfaction.
* Customers prefer not to pay a pre-deposit for reservations, but hotels should encourage advance deposits as they help secure revenue faster and significantly reduce cancellation risks.
* As most bookings are for two people, hotels should encourage family and group reservations by offering discounted packages to maximize revenue.
* Since longer stays are associated with lower ADR, businesses should focus more on short-stay customers for any facility or accommodation. By improving pricing and management strategies for short stays, businesses can attract more bookings and increase revenue
# **Conclusion**

* City hotels are more preferred, have higher ADR, experience more cancellations, and are busier than resort hotels.
* Out of total booking 27.5% of customers canceled their bookings, while 72.5% did not.
* Bookings are higher on weekdays compared to weekends, with more reservations made on weekdays.
* People from Portugal (PRT) made the most bookings, followed by Great Britain (GBR) and France (FRA) and also the highest revenue (ADR) was also generated by Portugal (PRT), followed by Great Britain (GBR) and France (FRA)
* In hotel bookings, advance reservations are the most common among customers.
* The highest number of bookings were made in 2016, followed by 2017 and 2015
* The highest number of customers arrived in August, followed by July and May, while January saw the lowest arrivals. Additionally, July and August were the peak months for revenue generation.
* In hotels, the majority of guests are couples, followed by single travelers and families.
* The most frequently served meal type in hotels is Bed & Breakfast (BB).
* Online Travel Agents (59.1%) dominate the market segment, while Offline Travel Agents/Operators (15.9%) have a significantly lower share.Additionally people who booked a hotel through an online travel agent  have a higher cancellation rate compared to direct bookings
* Most number booking is made by new customer rather than repeated customer
* Room types A and D have the highest number of customer reservations, making them the most preferred rooms  choices among guests.
* Room type A is the most popular among customers, with the highest number of reservations compared to other room categories.
* About 85 % chance that room is resereved by customer is assigned to the customer.Additionally, Not assigning a reserved room to the customer does not affect the cancellation rate
* Most bookings (82.4%) are for short-duration stays, as the majority of customers are transient travelers.
* The Transient customer type generates the highest revenue in both Resort Hotels and City Hotels. Additionally, the Group customer type generates the lowest revenue.
* Most people do not required car parking space
*  The most common stay duration is 3 nights, followed by 2, 1, and 4 nights, while stays longer than 7 nights are rare.
* A longer waiting period does not lead to booking cancellations.
* Higher lead time increases the chances of booking cancellations
# Author
* Vimal Solanki
