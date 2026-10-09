ZoomRide Trip Data Analysis Using SQL

  Project Overview

The ZoomRide project involved analyzing ride-hailing data to understand revenue performance, customer activity, and trip patterns across different cities and vehicle categories. SQL was used to examine the data, correct inconsistencies, and generate insights that could help management make informed business decisions.

  Business Objectives

The analysis focused on three main questions:

Which city contributes the most revenue?
During which month is ride activity highest?
Which vehicle category generates the most revenue?

Other objectives included checking the reliability of trip records, identifying incomplete information, and examining customer booking and spending patterns.

  Tools Used

OneCompiler –   MySQL:   https://onecompiler.com/mysql/455k6ffn6

  Database Structure

The project used three related tables:

Trips: Records of journeys, including dates, locations, fares, distances, and trip statuses.
Drivers: Information about drivers and their assigned vehicle categories.
Customers: Details of customers registered on the platform.

  Data Preparation

Before analyzing business performance, I examined the trip records to understand the dataset and identify potential data quality problems.

Record verification: Counted the available trip records to establish the initial dataset size.
Duplicate detection: Used grouping and aggregate functions to identify trips with matching customer, driver, date, and fare details. Duplicate entries were removed while retaining the original records.
Missing-value assessment: Checked for completed trips without recorded fares. These records were retained for investigation rather than assigning unsupported values.
City-name standardization: Corrected inconsistent city labels and removed unnecessary spaces to ensure that trips from the same location were analyzed together.
SQL Analysis

  Several SQL techniques were applied throughout the project:

COUNT() to measure trip volumes and customer activity.
SUM() and AVG() to evaluate revenue and average fares.
GROUP BY to compare results across cities, months, and vehicle categories.
ORDER BY and LIMIT to identify leading performers and the longest completed trips.
JOIN to combine trip information with driver details.
LEFT JOIN to identify registered customers with no recorded trips.

The analysis focused on completed trips when calculating revenue.

  Key Findings
1. Revenue Performance by City

Lagos was the strongest-performing city in terms of revenue, generating ₦218,890 from 93 completed trips. This makes Lagos a potential priority for targeted marketing and further business growth.

2. Monthly Ride Activity

December 2025 recorded the highest number of completed trips, with 31 rides. The month also generated ₦66,980 in revenue, making it a useful period for examining seasonal demand and planning driver availability.

3. Revenue by Vehicle Category

Economy vehicles generated the highest revenue among the vehicle categories, contributing ₦262,550 from 121 completed trips. This suggests that the category plays an important role in ZoomRide's overall revenue performance.

  Additional Data Quality Observations

The review uncovered duplicate trip entries, inconsistent city labels, and nine completed trips with missing fare values. These issues demonstrate the importance of maintaining accurate records before drawing conclusions from business reports.

  Recommendations
Grow the Lagos market: Consider targeted campaigns and customer-retention initiatives to build on the city's revenue performance.
Prepare for demand fluctuations: Review December's ride activity to identify factors that may help with planning for future peak periods.
Review Economy vehicle operations: Examine demand, driver availability, and operating costs before deciding whether to expand this category.
Improve data entry controls: Introduce checks to reduce duplicate records and ensure consistent city names.
Resolve incomplete fare records: Investigate completed trips with missing fares to improve revenue reporting.

  Conclusion

This project demonstrated how SQL can transform raw trip records into useful business information. The findings highlighted Lagos as the leading city by revenue, December 2025 as the busiest month, and Economy as the highest-revenue vehicle category. The analysis also emphasized the importance of data quality in producing reliable reports and supporting management decisions.
