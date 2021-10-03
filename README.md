# surfs_up

## Overview of the Analysis

### Purpose of the Analysis:
The purpose of this analysis is to analyze the weather to invest in 'surf n shake' shop, which serves surf boards and icecreams. In this challenge, we are analyzing the temperature data for june and december months in Oahu.

## Results

**Summary Statistics for June:**

   We are filtering date column in measurements table to display june month's data, converting it to a list and dataframe to show summary statistics for june.

![](https://github.com/Nikhila999/surfs_up/blob/main/images/june_temp.png)

**Summary Statistics for December:**

   We are filtering date column in measurements table to display december month's data, converting it to a list and dataframe to show summary statistics for december.

![](https://github.com/Nikhila999/surfs_up/blob/main/images/dec_temp.png)

Looking at the summary statistics for june and december, we are making following observations:
- Number of records in june is 1700 and december is 1517.
- Mean and median for june is around 75 and for december its 71, and the data is evenly distributed over median.
- The max temp in june is 85 and in december it is 83. Although december is winter the temperatures are fairly high.

## Summary
    
The temperatures in june and december months are somewhat similar or close by eventhough june is summer and december is winter. Summer is surfing and icecream season, also more than half days in december have temperatures over 71. So, we can conclude based on temperatures alone that an icecream and surf shop will run very well through out the year.
    
To answer the question about running the store through out the year, it would also help to analyze the precipitation data for june and december months.

    # Write a query that filters the Measurement table to retrieve the precipitation for the month of June. 
    june_prcp = session.query(Measurement.prcp).filter(extract('month', Measurement.date) == 6)
        
    # Write a query that filters the Measurement table to retrieve the precipitation for the month of December. 
    dec_prcp = session.query(Measurement.prcp).filter(extract('month', Measurement.date) == 12)

[June Precipitation](https://github.com/Nikhila999/surfs_up/blob/main/images/june_prcp.png)<p>&nbsp;</p>[December Precipitation](https://github.com/Nikhila999/surfs_up/blob/main/images/dec_prcp.png)
