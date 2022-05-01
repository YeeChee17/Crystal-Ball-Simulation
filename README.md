# Monte Carlo Simulation
Software: Excel, Crystall Ball

Monte Carlo simulation is a technique used to predict the probability of different results when risk and uncertainty are present in forecasting models. Monte Carlo simulation often invloves more than thousands of trials. In each trial, it will assign random values to uncertain variables to obtain a result. And the results of all tials will be summaries to achieve certain estimates at the end. The more trials, the more accurate of the estimate.

## Birthday Paradox
[Introduction on Wikipedia](https://en.wikipedia.org/wiki/Birthday_problem)

Birthday Problem: in N randomly chosen people, what is the probability of at least two people sharing the same birthday.

Birthday Paradox: counterintuitively, you only need 23 people to achieve a probability of 50%.

I turned this problem into a forecasting model and applied Monte Carlo simulations to obtain an estimate of the probability.
Below is the base model. And I also uploaded the Excel file for anyone wants to test different number of people.

<img width="688" alt="BP1" src="https://user-images.githubusercontent.com/102925575/166130038-229186a8-d5b9-4c0a-9f1f-b5806b41e468.PNG">

In the base model, the number of people is 23. I utilized data table to simulate 1000 trials and the resulting probability of two people sharing the same birthday is about 53%. To get a more accurate estimate, I also ran 10,000 trials using Cystall Ball and got a probability of 50.64%. Below is the frequency chart aftering running 10,000 trials.

<img width="481" alt="BP2" src="https://user-images.githubusercontent.com/102925575/166130353-d064c0dc-8b83-45aa-bdfd-485cb80207ab.png">
