# Kickstarting with Excel
## Overview of The Project
We have been given some data/information about an organization which does event management. We have been provided with dates , goal, pledged, countries, and so on and forth. some of the data is in readable for and some we have to make them readable/understable. Louise wants to understand how much fundraising can she do with plays; and what would be the best way to go about it.
### Purpose
The purpose of this project is to help Louise to raise fund by understanding how different campaigns fared in relation to their launch dates and their funding goals.
## Analysis and Challenges
I performed an anlysis on the dataset given by using excel function
convert the dates into a readable format
`=(((J2/60)/60)/24)+DATE(1970,1,1)`
Getting year from dates
`=YEAR(S2)`
### Analysis of Outcomes Based on Launch Date
creating pivot table
![image](https://user-images.githubusercontent.com/90114686/132110633-1e724ae2-d37e-4286-b116-d3bde570a67c.png)
The challenge I faced in this was giving the chart the title name, but after going throught the chart section again. I was able to fix it and give it a title.
### Analysis of Outcomes Based on Goals
The formula used in this function was a bit complex, we had to determine the number of successful plays with a goal of less than $1000, and we were able to determine that by following formula. Similarly we found the number of successful, failure and cancelled plays with different goals.
`=COUNTIFS((Kickstarter!$F:$F),"successful",Kickstarter!$D:$D,"<1000",Kickstarter!$P:$P,"=plays")`
Then I found the total and percentage of the upper data set
Then I created a chart by going in insert and selecting a line chart. On left clicking on chart and selecting the option of 
>select data
I unchecked number of successful challenge, failure, canceled and total projects.
### Challenges and Difficulties Encountered
The challenge I faced in this was giving the chart the title name, but after going throught the chart section in module again. I was able to fix it by clicking on the plus sign near chart and giving it a title.
The other difficulty i faced was with the outcome based on goal formula in this formula I was making a mistake of seleceting the dataset in the criteria and comparing it to successful, and hit and run and taking help from hint I was able to correct my formula.
## Results
The conclution we can draw from the Outcomes based on Launch Date are that the plays are most successfull during the month of May and June and least successful in December.
Therefore, Louise should launch the play in May or June and should avoid launching it in December.
The conclution we can draw from the Outcomes based on Goals is that Louise should have the goal of the play to be less than $5000 to have more chance of success. Althouth upto $20000 he can still have around 50% chance of success.
Limitation of this dataset is that it is not confined to one country, secondly some of the plays are live and we still have to determine their status.
We also need to consider if ther are any outliers in data and dealing with them
I would suggests we take out standard diviation of the data so that we can understand how scattered is data and which side is it skewed.
