
# Understanding voter turnout among the youth: evidence from Chile

This repository contains the material for the final project of course Topics in Applied Data Science of Columbia University. It contains the data set, a data dictionary, code, papers and reports. 

The main goal of the project is to predict electoral participation among a cohort of Chilean youngsters, by using an individual-level data set drawn from 2 sources. The first source is the university admission test (PSU) from December 2007, the main test that high-school graduates have to take in order to apply for college in 2008. This test is a pre-requisite to apply to most undergraduate programs. This data set contains test scores, school-level variables and household variables (see Final-project-QMSS-GR5069/reference/dictionary/Dictionary.xlsx) 

The second source is the electoral records of the presidential election of 2009. At that time, voting in Chile was mandatory, but registration was voluntary. Thus, individuals that are present in the electoral records made a conscious decision to participate in the election. By merging two sources by national id, we can observe whether the individual decided to vote. The data set is located in Final-project-QMSS-GR5069/data/raw/electoral_chile.csv

The purpose of our investigation is two-fold. First, we would like to offer our insights to inform policy and make Chile a more equitable political system. Second, during the next election, we would like to share a profile of the typical young voter with the candidates we endorse to help them better target the younger generation of voters.

# Research questions

This project has two research question: 1) What is the effect of cognitive skills on political participation? 2) What set of variables, including cognitive skills, household demographics (in particular, income) and school characteristics, are the most predictive of political participation?

For a longer discussion on the effect of cognitive skills on electoral participation, and the relevance of studying voter turnout with individual-level data and behavioral outcomes, please see Final-project-QMSS-GR5069/reference/motivation/cognitive-skills-electoral-PA-DRAFT.pdf, which is a first draft of paper using this data set. 

# Methods

The inital data set included every student who took the PSU test in 2007, regardless of the age. There is the possibility that some older people had taken the test in 2007, since there is no age restrictions. For instance, a person who finished high school at the age of 30 may have taken the test. We decided to restrict the sample to students who were born betwen 1988 and 1991 and who finished high school in 2007, since our substantive focus is to study determinants of electoral participation among the youth. The data set that restricts the sample to this subset is located in the folder "processed".

We used both inferential and predictive models on our data. We wanted to better understand past voter behavior and predict the likelihood of voting based on the profile of a recent graduate. Our methods included Linear Regression, Logistic Regression, Random Forests, SVM, Naive Bayes, KNN and LDA. Our data is just not predictive enough with all of the aucs not much greater than .5.

Our predictive methods failed. Since only 14% of the population in our data voted, our models were incredibly biased. We tried a wide range and couldn’t find one that worked, so we decided to focus on the inferential findings instead. We learned from our presentation feedback that next time we should approach the predictive models with bootstrap samples to make up for the bias.

# Insights
We discovered that the turnout of young voters is very low, allowing us to assume that this population is generally apathetic. Consequently, the small percentage of voters made it difficult to predict who is likely to vote in future elections. We were able to find some important insights from those who did vote. 

Our findings reveal the percentage of voters increased in the highest income group compared to the lowest income group. We also discovered that the higher the income, the higher the tests scores and grades, leading us to believe that wealthier students receive a better education. 

Out of all the testing categories, higher verbal scores are correlated with increased voting. We can assume from our findings that increased literacy is correlated with increased political participation. 

# Recommendations 

We’ve all heard that knowledge is power. However, when demonstrated knowledge is connected to income, power is not evenly distributed. The citizens from low income backgrounds, who have more to gain from strong government programs, don’t exercise their power through voting. This is especially problematic when we’re looking at the youngest generation of voters. If no action is taken and the trends continue, political power will remain disproportionately with the wealthy and educated.

Long term, we can increase voting in low income communities by increasing literacy programs in lower income schools. If we can build a strong foundation in reading from an early age, we are likely to see more young people vote in the future. 

For more immediate effects, we recommend implementing programs at schools to inform students about why it is important to vote. People can be motivated by why. If we can help young people understand a few good reasons why they should vote, as well as instruct them on how to vote, more might go to the polls for future elections. 

We can also use these insights in support of candidates that we endorse. Politicians often seek to mobilize younger generations of voters. However, if their efforts are not targeted, they may be a waste of time. We can encourage them to campaign more heavily in higher income areas. We can also suggest adding more educational elements in their messaging to lower income communities to continue to promote equal empowerment.

# Next Steps

In order to support our recommendations and increase the impact of our project, we plan to pursue a few more avenues of information. 

We want to better understand the profile of the likely voter and nonvoter by further exploring a few things. We plan to produce several graphs with voter registration data, income levels and test scores spatially located across Chile. We may be able to find geographic trends in the data that will allow us to focus our recommended programs in areas of need. 

We also failed to apporpriately adjust our data to work well with predictive models. There were far more observations that were categorized as nonvoters than voters, so our models were incredibly biased. We received feedback to do some random sampling, so we will retry some predictive models using bootstrapped data. 

In addition, we can explore data from a more recent election when the mandatory voting law was lifted. We’re curious if it changed the qualities of a voter. Did more low income, less educated Chileans vote or less? What other trends are revealed in these more recent elections? What does it mean for the trajectory of voting in Chile? How can we compare the two findings? If we want to influence the trajectory of voting participation in Chile, we need to better understand the trends in participation since this election.  







