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

Overall, even though the average fares are higher for the rural area, the urban area still has the greater number of rides and drivers along with a higher total fare amount with $39,854.38 

## Summary/Recommendations
1.
2.
3.

## References
1. Save Figure solution https://stackoverflow.com/questions/30765455/why-is-my-plt-savefig-is-not-working
2. https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.sum.html
3. Numeric_Only https://stackoverflow.com/questions/72223610/dropping-invalid-columns-futurewarning
