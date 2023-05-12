# PyBer Ride Sharing Data Challenge

## Purpose
To use Python, Pandas, and Matplotlib to create a summary DataFrame by city type and a multiple-line graph of total fares by each city type using the city and ride data csv.

## Results

Before getting the results we want to merge the two datasets into one DataFrame

    pyber_data_df = pd.merge(ride_data_df, city_data_df, how="left", on=["city", "city"])


### Total Rides
- Rural: 125
- Suburban: 625
- Urban: 1,625

### Total Drivers
- Rural: 78
- Suburban: 490
- Urban: 2,405

### Total Fares
- Rural: 4,327.93
- Suburban: 19,356.33
- Urban: 39,854.38

### Average Fare Per Ride and Driver
- Rural: 55.48
- Suburban: 39.50
- Urban: 16.57

### Total Fare by City Type
- Rural: 34.62
- Suburban: 30.97
- Urban: 24.52

Clean and formatted table:

![Screenshot 2023-05-12 at 5 03 27 PM](https://github.com/Jall3n/Module-5-Ride-Sharing/assets/119149740/3b41242e-b0ac-472d-8ff2-fa794808f2bb)

### Differences in Ride-Sharing Data among Different City Types

When looking at the city types the first thing that stands out is the difference in number of rides and drivers when comparing them. It makes sense that rural areas will have less drivers than the urban areas. However, even though there are less drivers in rural areas their average fare per ride and average fare per driver is higher than the suburban and urban areas. This is most likely because they are traveling longer distances on their routes and you could consider the higher rates are impacted by supply and demand.

Overall, even though the urban area has the greater number of rides and drivers along with a higher total fare amount with $39,854.38 the drivers are not earning as much as their sububran and rural counterparts.

![image](https://github.com/Jall3n/Module-5-Ride-Sharing/assets/119149740/e7ff0532-4b90-479a-b3cd-b7b69b809198)


## Summary/Business Recommendations
1. In order to help out the urban drivers we implement surge rates based on demand in the area. This can increase the amount of drivers in the area and allow them to earn some more money.
2. Add some incentives for rural drivers such as gas cards and car maintenance checks since they are driving longer distances. However, would need to see more data on average mileage between the city types. 
3. Improve the marketing strategy in months that have lower earnings and increase job advertising for rural areas

## References
1. Save Figure solution https://stackoverflow.com/questions/30765455/why-is-my-plt-savefig-is-not-working
2. https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.sum.html
3. Numeric_Only https://stackoverflow.com/questions/72223610/dropping-invalid-columns-futurewarning
4. Surge Rates https://www.uber.com/us/en/drive/driver-app/how-surge-works/#:~:text=Prices%20go%20up,to%20be%20a%20reliable%20choice.
