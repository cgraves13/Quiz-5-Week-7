# Quiz-5-Week-7 Write-up
Thank you for providing more structure and incorporating fill-in-the-blank code on this quiz. I appreciated the extra structure to figure out the r code since I am a beginner.

To figure out which variables in CivicData are discrete and continuous, I looked back at the example from Discussion 5 to compare the data. Once I figured out which variable was which, I entered additional data into the example to represent two more discrete and two more continuous data points.

In order to complete the code to generate the Poisson distribution, I needed to figure out which value “lamda” represents. I looked this up and learned that lamda is the mean, which in this case was stated to be 8 calls/hour in the example. Setting n to 100 hours, this function created a table with random values where each column represents the number of calls/hour from 2-16, and the values in the row represent how many times each of those numbers appeared in the data. The distribution makes sense for an example that has a mean of 8.

When I ran the code block mean(wait_times > 8) it returned 0.048. This represents the average number of wait times greater than 8 minutes. Only 4.8% of wait times were longer than 8 minutes, indicating that it is not very likely for someone to wait longer than 8 minutes for the bus.

For question 4, I had the wrong idea at first. I thought that if I selected the same number of data points from each income group that it would be more comparable. Once I tried explaining that, I realized that what I really needed were proportional representations in order to compare them. This was confirmed in the code line below. I decided to randomly sample 70% from each income group. I needed to use ChatGPT to determine how to fill in the missing code. I saw that to select 70% from each group, I needed to enter simple_frac(0.7) to generate a proportional sample.

Question 5 was difficult. I needed to run the code several times, but kept getting errors. Once I was able to create the histogram, I found that the density line was not displaying correctly. I pasted my code into ChatGPT which said that I should add “aes(y = ..density..)” to hae the line display correctly, and it worked.
