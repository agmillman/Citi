Module 18 Challenge - Citibike Analysis

The Tableau workbook created for this analysis contains trip hisotry data for the fourth quarter of 2024.

The trip history consists of 42 csv files combined into a single union, downloded from https://citibikenyc.com/system-data.

The landing dashboard is the Citibike Analysis for 4Q2024 and it displays:
- An interactive map of all bike stations that allows for filtering all other reports on the dashboard to the singular selected station
- Summary statistics broken down by the bike type (classic or electric) where applicable
    - Stations: Total number of stations contained in the dataset
    - Total Rides: Total number of rides started
    - Total Miles: Total miles ridden using a calculated field based on the distance between the starting and ending stations geographic coordinates
    - Avg Miles Per Ride: Average miles ridden based on the start station across all bike types
    - Avg Classic Miles: Average miles ridden based on the start station for Classic bikes
    - Avg Electric Miles: Average miles ridden based on the start station for Electric bikes
    - Avg Ride Duration: Average ride duration based on the start station across all bike types
    - Avg Classic Duration: Average ride duration based on the start station for Classic bikes
    - Avg Electric Duration: Average ride duration based on the start station for Electric bikes
- Most Popular: A listing of the Top 10 stations based on utilization within the reporting period.
- Least Popular: A listing of the Bottom 10 stations based on utilization within the reporting period.
- Stations can be filtered to a single station using either the Origination Station filter on the Map report or by directly selecting a station from either the Map or the Most / Least Popular reports
- Navigation to Citibike Station Analsysis dashboard below is triggered by selecting a station from either the Map or the Most / Least Popular report and then clicking on the link labeled View Station Analysis that is contained in the tooltip.
- Filtering for single station by selection on one of the report can be cleared by either selecting the station a second time or by clicking in a blank part of the map

The Citibike Station Analysis for {Station Name} dashboard displays data for a single station and consists of:
- The {Station Name} will automatically populate in the dashboard title based on the selected station from the main dashboard
- Rental by Bike Type: Displays a breakdown of rental volume by bike type
- Rentals by Date: A heatmap to visually indicate the busiest and slowest rental days across the reporting period
- Rentals by Day and Time: A heatmap by weekday to visually indicated the busiest and slowest rental days broken down by bike type
- Back to Stations Summary: A navigation button to return to the main dashboard

Observations
- Average miles for electric bikes across the quarter is 43% longer than classic bikes
- Average duration for electric bikes across the quarter is only 5% longer than classic bikes despite the larger average distance
- All of the top 10 utilized stations are located in Manhattan
- With one exception, the least popular stations are all outside of Manhattan
- The single outlier station in Manhattan is located at the Port, where there are mutliple other transporation options
- The most popular times for the top 10 individual stations tends to be Monday through Friday between 5 and 6pm