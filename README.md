# eda-capestone-project
exploratory data analysis has been performed on hotel booking data set 
and tried to obtain information based on previous data. Matplotlib and seaborn of python is used to 
perform EDA. Initially data collection and data cleaning has been done. Then for analysis project is 
divided into many parts. They are univariate analysis, Hotel analysis, Cancellation analysis, Room type 
analysis, Resesrvation type analsis, Parking Space analysis and Special request analysis. Hotel booking 
analysis will help the hotel management to understand the patterns in booking and about customers. It 
helps to increase the revenue and profit of the hotel.

### DATASET:

We were provided with 32 datasets and 119390 rows. The given datasets are: 'hotel', 'is_canceled', 'lead_time', 'arrival_date_year', 'arrival_date_month', 'arrival_date_week_number', 'arrival_date_day_of_month', 'stays_in_weekend_nights’, 'stays_in_week_nights', 'adults', 'children', 'babies', 'meal', 'country', 'market_segment', 'distribution_channel', 'is_repeated_guest', 'previous_cancellations 'previous_bookings_not_canceled', 'reserved_room_type', 'assigned_room_type', 'booking_changes', 'deposit_type', 'agent', 'company', 'days_in_waiting_list', 'customer_type', 'adr', 'required_car_parking_spaces', 'total_of_special_requests', 'reservation_status', 'reservation_status_date'.
### DATA CLEANING

To remove missing values and Replace the null/NaN values.
- It is observed that agent and company column has null values so replacing null 
values in country and agent clumn with 0.
- Replacing missing values in children column with mean of that column. This column 
has zero as value so it is inappropriate to replace missing value with 0.
- Column country is objective type so to deal with missing value replacing missing 
values in country column with the mode of country column.

Converting some of the columns datatype:

- Datatype of children,agent and company if float64, converting that to int64.
- reservation_status_date column datatype is changed to data_type

Removing of unnecessary rows/columns.

- There is 31994 rows of duplicate values, removing of such rows.
- some rows have zero values in adults, children and babies columns. There is 166 
rows of such type dropping that rows

### OVERVIEW OF ANALYSIS

In this exploratory data analysis, data is analyzed and tried to explore some of the results. Important 
questions for which answers are explored are as follows:

- In which month, the hotel received more bookings?
- which company and agent makes more no. of bookings?
- Which meal is most ordered by guests?
- To which country more no of customers belongs to ?
- Which type of customers are more?
- How many guests arrived yearwise and hotelwise?
- Which hotel has more adr?
- Which hotel is more likely to put the customer in waiting list before confirming?
- Which hotel has more cancellations?
- Which distribution channel has made more cancellation?
- Does making customers to wait causes cancellation of bookings?
- Which type of customers cancel the bookings most?
- Which type of room is in demand?
- What percentage of customers have checked out?
- What is the optimal length of stay in order to get the best daily rate?
- What percentage of customers opt for car parking?
- Which month of the year has recieved mmore no of special requests?
- Now analyzing the change of trend in special requests made yearwise?
- predict whether or not a hotel was likely to receive a disproportionately high number of special 
requests

### IMPORTANT LIBRARIES.
- NUMPY
- PANDAS
- MATPLOTLIB
- SEABORN

### GRAPHS AND PLOT

The important graphs and plots used are  
- Bar graph
- Pie Chart
- Histogram
- Scatter Plot
- Heat Map
- Box Plot.

### CONCLUSION:

- The arrival of guests is more in August and july
- The most bookings is made by company 40 and agent 9. 
- About 78% of guests has ordered BB(bread and breakfast).
- Most of the customers are from Portugal(PRT). Bookings from other countries are very less.
- Transient type of customers has made more bookings where they have not included in contract
- Bookings in city hotel is about 60% and 40% in resort hotel out of total bookings. City hotel has 
more bookings. 
- That city hotel has more adr. Therefore city hotel generates more revenue compared to resort 
hotel.
- City hotel has more chances of putting it's customer in waiting list. This is because due to city 
hotel receives more bookings. 
- Cancellations are made more in city hotel. Transient type of customers and TA/TO has more 
chances of doing cancellations.
- Waiting period does not effect on cancellations.
- Room type A is in demand. D and E room type also are in slight demand.
- In city hotel 70% of the customers who booked are checked out. In resort hotel 76% of the 
customers are checked out.
- It can be inferred that optimal lenght of stay in both the hotels is less than 5 days.
- Most of the guests i.e. About 93% does not require parking space. Few guests have booked for 
one car parking. 2, 3 and 8 parking space requirement is very less
