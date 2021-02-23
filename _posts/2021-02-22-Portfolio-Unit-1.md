---
layout: post
title: Portfolio Unit 1
subtitle: College Predicted Successful NBA Career
cover-img: assets/img/thumb.png
thumbnail-img: assets/img/thumb.png
share-img: assets/img/thumb.png
tags:[portfolio]
---

# Relationship Between Attending a Power 6 Conference for Basketball and Having a Successful NBA Career

## Chi-Square Test of Interdependence

---

# Introduction 
Determine if attending a Power Six Conference for college basketball correlates to having a successful career in the NBA. 
## Provide relevant background information on your topic.
Have player examples of big time stars that didn't attend big schools, and bust players that led to decision.
For a certain number of years attending college wasn't mandatory(LeBron), but we're focusing on if attending a power school relats to success, so it's fine
# Description of the data
## Provide a description of your dataset.  Where did you find it?  What data does it contain?  Are there any limitations to your dataset?
-Found on kaggle.com/dataset
-Information on every NBA player since 1950, including years played, height, weight position, college attended
-Limitations:
# Statistical methods
## Describe your hypotheses.
-Ho: There is no relationship between college attended and successful NBA career.
-Ha: There is a relationship between college attended and successful NBA career.
## Describe any data wrangling or feature engineering you had to do.
-calculate total years played
-create new "Successful Career" by finding average number of years played, double that, -> over double an average career sounds successful
-label for Power Six Conference, apply to each row to find who attended
-dropped any NAN for college, only comparing those that went
## Provide a description of the statistical methods you used to analyze your data.
-chi square test of independence, is there a correlation between Power 6 conference and successful career in NBA
# Results
## Describe the results of your analyses.
-The p-value is: 2.9795317795864165e-08
-This is a very small p-value, so we would reject the null hypothesis and assume there is a relationship between college attended and successful NBA career.
## Present two visualizations related to your hypotheses.
# Conclusion
## Report the conclusions of your hypothesis test(s).
-So, there, in fact, is a relationship between attending a Power 6 Conference for basketball and having a successful NBA career.
## Summarize the key features of your visualizations.
- shows that the average number of years played for not attending a Power6 is just under 4, for attending a Power6 just over 4
- shows that those that had a successful career more often attended a Power6
## Discuss any limitations of your analyses.
-should drop out any new players that haven't had time to have a successful career yet
-drop years like Lebron that would've attended a power 6 school, but didn't need to go to college
-drop foreigners? only limited to those
## Compare your results to other, similar analyses.
- need to find another similar analysis. check conferences websites perhaps..
## Discuss new questions your results raise or new directions for further research.
-is it only if they were a starter in college that there is a correlation?
-break down data further
-if we took out and D-2 schools, would there be a difference in Power6 to other D-1 schools

# Thank You.

---
