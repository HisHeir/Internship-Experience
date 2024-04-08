# Internship-Experience

## Data Analysis of Time and Amount spent

## Project Overview
As a microbiology student of Federal University of Technology, Akure, I decided to make my internship year count by finding a standard laboratory to learn hands-on expereince lab practices. This desire and pursuit made me to thorough online research until I found The Nigerian Institute of Medical Research, located at Yaba, Lagos.
The program took place for 5 months, and I limited my going to work 3 days in a week after about 6 weeks I started and discovered that going to everyday wouldn't be sustanable due to stress of transportation and financial incapability.
From the first day of work, I began to take data which I later develpoed into a dashboard in this project.

### THE DASHBOARD
![IT dashboard](https://github.com/HisHeir/Internship-Experience/assets/165808027/502bb6bb-f51a-407f-ae1f-08fe86bc7f00)

### The data looks like this:
![IT dashboard 2](https://github.com/HisHeir/Internship-Experience/assets/165808027/74e77dd6-fd39-4da8-95c1-e257ea12dfef)


## About the Data
The data was collected daily and it captures variables such as:
- Time out of home
- Time in for work
- Time out of work
- Time back home
- Amount spent on transport
- Transport medium

## Tools used
- Notepad
- Microsoft Excel
- MySQL
- PoweerBI

## Data Collection and Preparation
The data collection was done on my notepad everyday and data entry was done using MysQL, it was exported to excel where dew columns were added and later laoded on PowerBI for report and visualization.

## Sample of the code written on MySQL
```sql
CREATE TABLE daily_transport_details2 (
    Date date,
    Time_out_of_home timestamp,
    Time_in_for_work timestamp,
    Time_out_of_work timestamp,
    Time_back_home timestamp,
    Transport_medium VARCHAR(10),
    Amount_spent int,
    PRIMARY KEY (Date)
);
```
```sql
insert into daily_transport_details(Date,Time_out_of_home,Time_in_for_work,Time_out_of_work,Time_back_home,Transport_medium,Amount_spent)
 values ('2023-01-16', "06:26", "09:04",'16:10', '20:50', 'Tata', 1150),('2023-01-17', "06:30", "08:24",'16:25', '21:00', 'Tata', 1100),
```

### The table was checked using:
```sql
select * from daily_transport_details2
```
## Focus of the analysis
- To keep track of the amount spent per day, resultung to weekly amount and eventually total amount per month
- To know the time spent using various transport medium

## Findings of the Analysis
- More than #103,000 was spent on transport fare,
- BRT recorded 50% faster than using Tata on Lagos road,
- The least amount was spent in April and the highest amount spent in March,
- Tata was used the most in the first month of the program.

## Limitataions

  1. The use of timewatch could have done better if used
  2. Some data were miossing by the time of data entery, so approximate values were entered to avoid missing records
