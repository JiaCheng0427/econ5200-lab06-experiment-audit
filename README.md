Experiment Design Audit – Power, Selection & Weighting
Objective
In this lab, I studied how experiment design and selection bias affect statistical results, and how statistical methods can help improve estimates.
Methodology
- I used power analysis to check whether an A/B test had enough users to detect a small effect.
- I calculated the required sample size and compared different group sizes.
- I examined selection bias in a wellness program by comparing participants and non-participants.
- I used inverse probability weighting (IPW) to reduce selection bias.
- I wrote a power_check() function to calculate statistical power and compared the results with statsmodels.
- I also used Meng's Data Defect Identity to calculate the effective sample size of a biased poll.
Key Findings
- The original A/B test had only 19.8% power, which was much lower than the 80% target.
- To reach 80% power, the experiment needed 12,514 users per group.
- Splitting the same 50,000 users evenly would increase power to 97.7%.
- The naive estimate suggested that the wellness program reduced healthcare costs by $1,396, while the true effect was only $500.
- After using IPW, the estimated savings were $522, much closer to the true effect.
- In the extension, I calculated a data defect correlation of -0.067445. Although the poll had 389,090 respondents, its effective sample size was only about 140.
Conclusion
This lab helped me understand that having more data does not always lead to better results. Good experiment design and reducing selection bias are important for making accurate estimates.
