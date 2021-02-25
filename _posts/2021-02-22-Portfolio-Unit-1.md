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



---

## The Intro
Have you ever wondered what are the odds that a player from a small college will have a successful professional career? Well, I have. So I tried to determine if attending a Power Six Conference for college basketball correlates to having a successful career in the NBA. 

Many times watching the NBA or NFL, I am surprised when the players share the name of the college they attempted. I am often expecting to hear nothing but Alabama or Oklahoma for football, or only Kentucky or Duke for basketball. But often, what I hear is not what I expected. So, I wanted to test and see if there is truly a correlation to having a long, successful career and the college attended. If there is, it would make sense to me. But maybe the big school only helps you get into the professional league, and from there everyone has as good of a shot at having a long career. 

## The Background

Same Bowie is a name you may or may not know. He was a 7’1 center at Kentucky. He was picked by the Trailblazers in the 1984 NBA draft, the second pick in the first round. He was picked BEFORE Michael Jordan. And he was one of the biggest NBA busts of all time. Tyler Hansborough was a more recent player for UNC, from 2005 to 2009. He was a star in the ACC and was the 13th pick in the 2009 draft to the Pacers. He bounced around from the Pacers to the Raptors to the Hornets for seven years with little playing time before moving to the basketball leagues in China, where he currently plays. On the other hand, the Celtics’ Larry Bird was one of the greatest players of all time, and he attended Indiana State University.

For a certain number of years attending college wasn't mandatory, and several notable players were drafted straight from high school. A few of these players include Kevin Garnett (‘95), Kobe Bryant (‘96), and LeBron James (‘03). In 2005 the rules of the league were updated, and to be eligible for the draft one had to be 19 years old. So since then, and before 1995, every player had at least attended some college. It is likely that any player good enough to be drafted from high school would have attended a major conference. However, since we are only looking at the relationship between conference attended and lasting NBA career, this will not affect our data, as players that had no college experience were dropped from the list. 

## The Data

The dataset used was found on Kaggle, published by Omri Goldstein. The data on this file was scraped from basketball-reference.com. The data-set contains aggregate individual statistics in the NBA since 1950, 67 seasons, from basic box-score attributes such as points, assists, and rebounds to more advanced money-ball like features such as Value Over Replacement. It does not have data from seasons since 2017.

## The Statistics 

For determining if there is a relationship between attending a Power 6 Conference and having a successful NBA Career, we will use a Chi-Square Test of Independence. The hypotheses are as follows:

-Ho: There is no relationship between college attended and successful NBA career.

-Ha: There is a relationship between college attended and successful NBA career.

### Data Wrangling // Feature Engineering
The dataset only showed the starting and ending year for each player. From here I subtracted the two to calculate the total years played for each player. Then I created a new "Successful Career" that includes those players that played for at least double the amount of time as an average NBA career. I calculated the average number of years played for each player, then doubled that, and applied it to each player that qualified. Roughly 20% of the players received a “Yes” for “Successful Career”, so this seemed like a fitting measure.
 
I also created a label for Power Six Conference, and I applied to each row to find who attended a qualifying school. 
I dropped any row with a null college value, as we only want to compare those that went.

### Statistical Methods
I used a chi square test of independence, the chi2_contingency function, to see if there was a correlation between Power 6 conference and a successful career in the NBA.

## The Results

After doing the test, the p-value is: 2.9795317795864165e-08. This is a very small p-value, so we would reject the null hypothesis and assume there is a relationship between college attended and successful NBA career. 

## The Conclusion
There, in fact, is a relationship between attending a Power 6 Conference for basketball and having a successful NBA career.


This barplot from Seaborn shows that the average number of years played for not attending a Power6 is just under 4, for attending a Power6 just over 4


This catplot shows different career lengths and how many players correspond. A hue was added to show the difference between conference attended. Something to consider with this graph is that overall there are more NBA players that attended a Power Conference School, than those that didn’t. 

### run df['Power School'].value_counts() To give percentage for each


This barplot shows that those that had a successful career more often attended a Power6

### Limitations
Some schools, like Gonzaga, are top programs, though they are in a smaller conference. Adam Morrison, from Gonzaga was one of the top picks in his draft year, although he did become a bust. These programs help the cause for conferences outside of the Power 6 overall. We could also have dropped the years from circa 1995 to 2005, where players would've attended a power 6 school, but didn't need to go to college.

### Similar Analyses
- need to find another similar analysis. check conferences websites perhaps..
- 
### Questions Raised
Is it only if they were a starter in college that there is a correlation? If we took out Division 2 and lower schools, would there be a difference in Power 6 Conferences to other Division 1 schools. We could break down the data further to understand this relationship. 

## The Recap

While there is no proven causation, there is a significant correlation with attending a major conference and having a long NBA career. So, I would recommend anyone interested in that to go to Duke.

# Thank You.

---

