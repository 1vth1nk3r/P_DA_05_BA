# Research on ticketing platform users' behaviour patterns
The project from the Business Analytics sprint of the Practicum DA/DS course.

## Description
Here we have a dataset on Yandex.Afisha visits, orders and marketing expenses. We want to explore users' behaviour patterns. It would allow us to optimize marketing campaigns.

First, we should do some data preprocessing: clean the data, fill in the missing values (if any), and change data types. Also, we need to add some new columns to help our analysis. After doing so, we could explore our data.

## Conclusion
After preprocessing, I've added additional date parameters and dropped those not helpful for further analysis.  
There were no missing values and no duplicates in this dataset.

We are starting the analysis with information about visits. The average MAU is 23228, and WAU is 5724, with highs in cold months and lows in summer.  
The average DAU is 908, the average number of sessions per day is 987,  and the average number of sessions per user is 1.08.  
It would not be beneficial to talk about the overall average session length  (the mean is 644 seconds, and the median is 300) since we have 9.96% zero-length sessions and 6.86% lengthy sessions (larger than Q3+1.5IQR). If we exclude these sessions, we get the average session length for desktop users of 515 seconds and touch users of 427 seconds.  
We don't see a high retention rate, and it is getting lower with later cohorts.

Looking at the orders' data, we see that the overall conversion rate is 16%. Half of the visitors convert in zero days and 3/4 in two days.  
The median number of purchases per customer is 1.43, which correlates with our low retention rates.  
The average purchase size has a mean of 5 and a median of 2.5. Its starting size is almost similar across all the cohorts, but the cohorts from September and December have significantly larger average purchase sizes in further months.  
This phenomenon contributes to different LTV across the cohorts. For example, the one from September has a significantly larger LTV in three months. Also, the cohort from June with the highest retention rate is doing better than the others.

And finally, we analyzed marketing expenses.   
Total marketing cost was 329131, with the expenses on the third source being almost half of it (141321). Also, plotting the change in marketing costs over time, we found the cause of a more significant number of visitors in winter. These were the months with higher expenses.  
The average overall CAC was pretty stable (and high) for the whole time except for the last month. Splitting CAC by source, we found that it differs significantly.    
ROI per cohort was not impressive. The September and June cohorts show the best results here. The reason for it is the difference in CAC by sources. The third source haves a tiny ROMI of 0.36, while the first is much better, with the ROMI of 1.71.

Based on this data, I recommend cutting the expenses on source number three and redirecting these finances to the first source.
