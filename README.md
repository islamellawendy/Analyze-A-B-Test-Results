# Analyze A/B Test Results
## Dataset
The dataset was already a given in Udacity's coursework. I have been also instructed to use the template notebook provided in the project. 

An e-commerce company is looking to implement a new page, they have gathered data for the conversion for 2 groups of users, testing the old page (the control user group) and the new page (the treatment user group) by A/B testing. This is provided in the csv file.
## Summary of Findings
Initially I used A/B testing to see if the new page fared better or not. I used the following hypothesis testing.

$$H_0: p_{new} - p_{old} <= 0$$ 

$$H_1: p_{new} - p_{old} > 0$$

After using bootstrapping to simulate results, I got the difference in conversions between the old and new pages. At this stage I failed to reject the null hypothesis and the old page fared slightly better in conversions.

The next step was using the logistic regression model. In order to do so I changed the hypothesis to the following.

$$H_0: p_{new} - p_{old} = 0$$

$$H_0: p_{new} - p_{old} \neq 0$$

I observed all vairabkes, and due to having a Type I error greater than 5% I failed to reject the null again, and would state the old page still fares better.
## Key Insights and Takeouts
### Insights
In summary our variables in this dataset are simply not statistically significant, we have failed to reject the null and thus have no concrete evidence that the new page is better.
### Takeouts
I practiced timestamp regression through weekdays and weekends categories (welcome to notedown improvements here) as a further analysis scope.
