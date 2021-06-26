# Kickstarter-Challenge

Overview of Project

In this Kickstarter Challenge, we focused on campaigns for how the play Fever fared in relation to their launch dates and funding goals. In this report, we will analyze the data we calculated after determining the campaign outcomes based on their launch dates and their funding goals. 

The purpose of this analysis is to determine the outcome of the play Fever based on launch date and goals. In the first part of this analysis, we will focus on the total Theater outcomes according to Launch date. There were three outcomes for this play, Successful, failed and canceled and we will go over the result for each in further detail. We will also examine the possible reasons why some months fared better than others. In the second part of this analysis, we will focus on outcomes based on goals and some challenges encountered while determining the data for this analysis. 

THEATER OUTCOMES BASED ON LAUNCH DATE

In the chart below, we can see that the May and June had the most successful launch dates with 111 and 100 outcomes, respectively while December had the least successful with 37 outcomes for the play Fever. May and July had the highest number of failed outcomes with 52 and 50 failed outcomes while November had the least failed outcomes at 31. Finally, January had the highest level of canceled shows with 7 outcomes while July had 1 canceled outcome and October had no data whatsoever for canceled shows.

!Theater_Outcomes_vs_Launch](path/to/Theater_Outcomes_vs_Launch.png)

CHALLENGES
When plotting this graph, I initially used Scattered line chart, but that selection did not display the results in the correct format needed to analyze the data. The data points were on the wrong side of the axis and did not align with the numbers on the y-axis. Due to this mishap, I used the line chart instead and it displayed the data correctly and made it easier to successfully analyze the data.

OUTCOMES BASED ON GOALS

To determine the outcomes based on goals, we created 12 rows with goals that are less than 1000, between 1000 and 4999, 5000 and 9999, 10000 and 14999, 15000 and 19999, 20000 and 24999, 25000 and 29,999, 30000 and 34999, 35000 and 39999, 40000 and 49999, and greater than 50000. Then we created columns for the number of outcomes that were successful, failed and canceled, determined the total of all three and percentages for each. To determine the number of outcomes, we used the COUNTIFS formula, and I used the ROUND formula to determine the percentages of each. 


!Outcomes_vs_Goals](path/to/Outcomes_vs_Goals.png)


According to the graph above, we can see that goals less than 1000 had the highest number of successful outcomes at 76% while goals between 45000 and 49,999 had the least successful rate at 0%. In contrast, goals between 45000 and 49999 had the highest rate of failed outcomes with 100% while goals less than 1000 had the least failed outcome with 24%. There were no canceled outcomes for this analysis. 


	CHALLENGES
Using the COUNTIF formula was a bit of a challenge because I entered the wrong information several times and excel would not allow me to proceed or my formula produced a 0 result, which I know was false. Initially, I entered =COUNTIFS(Kickstarter!D:D, "<1000", Kickstarter!R:R, "plays"), which generated a zero result. Then I used =COUNTIFS(Kickstarter!D:D, "<1000", Kickstarter!F:F, Kickstarter!R:R, "plays"), which generated an error before using the correct formula (=COUNTIFS(Kickstarter!D:D, "<1000", Kickstarter!F:F,"successful", Kickstarter!R:R, "plays")) to determine the result for Cell B2. After completing the number of Successful outcomes, I used the SUM function to determine the total of all the successful outcomes for all the goals, which was 694. To confirm that my calculations was correct, I used the COUNTIF formula to determine if the total was correct and used the formula =COUNTIFS(Kickstarter!D:D,">=0",Kickstarter!F:F,"successful",Kickstarter!R:R,"plays") which also gave a total of 694. I did the same for the failed and canceled outcomes to cross check my work. 

RESULTS

 We can determine from our analysis that the play Fever had the most successful and failed theater outcomes during the Spring/Summer months (May, June, July and August) and least successful and failed outcomes at the beginning and towards the end of the year. For more successful shows, it is better for Louise to launch her theater shows during the Spring/Summer. 

Based on our analysis for Outcomes based on goals, goals less than 5000 produced the highest percentage of successful outcomes while goals less than 5000 produced the least percentage of filed outcomes. In this analysis, we can conclude that the higher the success rate based on goals the lesser the failure rate and vice versa. We can also conclude that goals less than 100 produced the most positive outcome for Louise’s play Fever. Line charts is the best graphs we can use to view and analyze the data provided efficiently.

In conclusion, for more successful theater outcomes, it is advisable that Louise play should be in the Spring/Summer and the goals should be less than 1000. 




