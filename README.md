# CIS-320-Final-Project

Introduction <b><p>
Part of our everyday lives is spent on the move whether it be walking, driving, or flying. When flying to a destination, we often think about whether we will depart and/or even arrive on time. This begs the question: how frequent do flights get delayed? And when the delay occurs, what are the major factors that have resulted in that particular delay. Despite a world well-connected through technology, flying has remained one of the most popular modes of transportation for various reasons, such as for business or vacation.

Hypotheses
Based on the questions mentioned, I have developed a few hypotheses I would like to try to prove. My first hypothesis is that I believe about 25% of flights are delayed according to my own flight history. I have been on 26 flights within the last two years and 6 of those 26 flights have been delayed. My next hypothesis is more specific. Taking the data regarding the flights that were delayed, I propose that the cause of delays for flights in the winter months (December to February) were the result of weather delays more than the summer months (June to August). Since the United States experiences the most unfavorable weather for aircraft during the winter months, it would make sense that the reason for flights being delayed at this timeframe would be due to the inclement weather. The winter months would also be a reasonable amount of data to utilize since approximately 23.3% of flights within the year compared to the 26.4% of the summer months.

Methods
To provide proof for the hypotheses, data from the Bureau of Transportation Statistics will be extracted, cleaned, organized, and tested for analysis. For simplicity, I took the data from flights within the domestic United States and within the last year (December 2014-November 2015). November 2015 was the recent month the Bureau of Transportation Statistics had on file in the database. To simplify matters further, I only considered the flights that were delayed, not cancelled. Cancelled flights obscured the data for delays because of their missing information. Consequently, to clean the data for delays, I filtered out cancelled flights.  With such a large volume of data, I extracted the data for every month of the period into Comma Separated Value files. I then compiled the data into IBM SPSS Statistics program and saved it as .sav file, giving me a file with all the consolidated information I would need to run various types of analysis. Using IBM SPSS Statistics even further, I ran the frequency distribution as shown below in Figure 1. By having the frequency distribution, I was able to find out which months experienced the most flights and which ones experienced the least. Using this spectrum, I was able to gather further insights about the data. As aforementioned, the summer months experienced the most, mainly due to a time period known for vacationing. Conversely, the winter months experienced the least amount of flights despite being also known for a time to vacation. The underlying reason could be that less flights are scheduled as a result of the poor weather conditions. Along with IBM SPSS Statistics, I also loaded the data through R to obtain descriptive statistics as shown in Figure 2 and create a pie chart (Figure 3) based on the frequency distribution displayed in IBM SPSS Statistics. I also utilized R to find the rate at which flights were delayed relating to one of my hypotheses. In addition, I particularly focused on the weather delay variable in both the summer and winter months since it pertained to my other hypothesis. Lastly, I ran a two sample t-test through R to determine the significance of the means for the weather delays in the summer and winter.

Analysis
In terms of the first hypothesis (how often flights are delayed throughout a one year period), I was able to obtain the rate for both arrival delays and departure delays. For simplicity, whether it be classified as arrival or departure, I generally categorized it as delays. But to give an idea of how much of a difference the rates were, I ran the data through R (Figure 4). For departure delays, R calculated 18.52% whereas for arrival delays it was 18.85%. In general, from December 2014 to November 2015, about 19% of flights were delayed, which is substantially less compared to the rate of 25% I hypothesized based on my flight history. 
The second and final hypothesis dealt specifically with the weather delays in the summer and winter months. I proposed that weather delays had a prominent occurrence in winter months due to the unfavorable conditions that happen during this period. Their rate was compared to the weather delays in the summer months since one would assume that summer weather would work in favor of aircraft. When calculating the rates, I again used R as shown in Figure 5. Initially, I used the total flights in the given seasonal period as my reference when finding the rate of weather delays. However, as seen in Figure 6, I used an R command to omit the missing data from flights that were not delayed in order to get the rate of weather delays that occur from the total amount of delays. This would give a better understanding of how often delays are caused by weather delays. For winter months, the rate was about 6.4% while for summer, it was around 6.0%. By simply comparing the rates, it exhibits that relatively speaking flights in the winter months experience slightly more weather delays than do the summer months. However, when taking into account the mean, or average, time for delays, weather delays in the winter took an average of 2.71 minutes whereas the ones in the summer took 2.77 minutes (Figure 7). Consequently, weather delays were much frequent in the winter but they took up a longer amount of time in the summer. To make a more proper assessment of these two means, I decided to test it further and ran a two sample t-test in R (Figure 8). The result was a p-value of 0.1108 which clearly is significantly higher than the alpha of 0.05. Therefore, we fail to reject the null hypothesis at the 95% confidence interval that the difference between the mean of the summer months and the mean of the winter months is equal to zero. The result, moreover, is statistically nonsignificant.

Conclusion
After running the calculations and tests in R, my first hypothesis was rejected since the rates that were computed had large difference relative to the rate that I proposed. The calculated rate was approximately 19%, which is significantly less than the predicted 25%. On the other hand, my second hypothesis was supported through the calculating the rates as done for the first hypothesis. Specifically, it was the rate of delays that occurred due to weather delays in the summer and winter months. When considering the means of the two periods, the summer months, on average, had slightly longer delays than the winter months. But after running a t-test to verify, this became statistically nonsignificant. However, this does not mean that the null hypothesis is true; it only signifies that insufficient evidence exists to reject it.
