# Monte Carlo Simulation
Software: Excel, Crystall Ball

Monte Carlo simulation is a technique used to predict the probability of different results when risk and uncertainty are present in forecasting models. Monte Carlo simulation often invloves more than thousands of trials. In each trial, it will assign random values to uncertain variables to obtain a result. And the results of all tials will be summaries to achieve certain estimates at the end. The more trials, the more accurate of the estimate.

## Value of Customers (CLV)
Monte Carlo simulation can very useful when estimating the value of customers.

Here is a project I did for a company who runs a subscription business model. All data is modified from the real data.
The model below is one simulation for one random sample of their customers. By applying cohort analysis which groups customers basing on the time of their first subscription, the average monthly retention rate can be obtained. Acquiring costs are estimated based on their ads expenditure on Facebook. The rests are assumptions. All these estimates and assumptions can be improved by acquiring more data and consulting experts, which will also improve the model accuracy. 

<img width="659" alt="CLV1" src="https://user-images.githubusercontent.com/102925575/166136057-23bae289-8771-4990-a8fd-46798538192c.PNG">

We can see from the model that this sample customer's lifetime value is $902.76 with 11-month life time. By repeating such simulation for 10,000 times using Cystall Ball, we can generate 10,000 sample customer lifetime values and customer life time periods. Then we can obtain some business insights by summarizing these results:

<img width="745" alt="CLV2" src="https://user-images.githubusercontent.com/102925575/166137125-066f2977-2eac-4f45-8cde-02c6e5d77394.PNG">
<img width="751" alt="CLV3" src="https://user-images.githubusercontent.com/102925575/166137460-9e713670-462e-4815-af50-3dbf47cdebb1.PNG">

The above charts indicate that 95% of customers' CLV are between -$198.24 and $1230.78. And around 25.72% of customers have negative customer lifetime values, which means they usually unsubscribe after first or second month. The retaining month charts show that 65.97% of customers leave after the third month and 16.64% of customers will stay over 6 months. 
 
The first-month retention rate, acquiring costs mean, acquiring costs standard deviation are potential key drivers of this model. We can also use Monte Carlo simulations to test the impact of these key drivers. Let's see, how would the result change if the first-month retention rate is increased to 75%: the percentage of customers having negative CLV drops from 25.72% to 18.27%; 19.88% of customers will stay over 6 months, 3.24% higher than before.

<img width="794" alt="CLV4" src="https://user-images.githubusercontent.com/102925575/166138817-1f2cb81c-d8d3-4e52-882f-610c2b968c2b.PNG">


## Birthday Paradox
[Introduction on Wikipedia](https://en.wikipedia.org/wiki/Birthday_problem)

Birthday Problem: in N randomly chosen people, what is the probability of at least two people sharing the same birthday.

Birthday Paradox: counterintuitively, you only need 23 people to achieve a probability of 50%.

I turned this problem into a forecasting model and applied Monte Carlo simulations to obtain an estimate of the probability.
Below is the base model. And I also uploaded the Excel file for anyone wants to test different number of people.

<img width="688" alt="BP1" src="https://user-images.githubusercontent.com/102925575/166130038-229186a8-d5b9-4c0a-9f1f-b5806b41e468.PNG">

In the base model, the number of people is 23. I utilized data table to simulate 1000 trials and the resulting probability of two people sharing the same birthday is about 53%. To get a more accurate estimate, I also ran 10,000 trials using Cystall Ball and got a probability of 50.64%. Below is the frequency chart aftering running 10,000 trials.

<img width="481" alt="BP2" src="https://user-images.githubusercontent.com/102925575/166130353-d064c0dc-8b83-45aa-bdfd-485cb80207ab.png">
