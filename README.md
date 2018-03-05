
# Understanding voter turnout among the youth: evidence from Chile

This repository contains the material for the final project of course Topics in Applied Data Science of Columbia University. It contains the data set, a data dictionary, code, papers and reports. 

The main goal of the project is to predict electoral participation among a cohort of Chilean youngsters, by using an individual-level data set drawn from 2 sources. The first source is the university admission test (PSU) from December 2007, the main test that high-school graduates have to take in order to apply for college in 2008. This test is a pre-requisite to apply to most undergraduate programs. This data set contains test scores, school-level variables and household variables (see Final-project-QMSS-GR5069/reference/dictionary/Dictionary.xlsx) The second source is the electoral records of the presidential election of 2009. In that year, voting in Chile was mandatory, but registration was voluntary. Thus, individuals that are present in the electoral records made a conscious decision of participating in the election. By merging two sources by national id, we can observe whether the individual decided to participate in the election. The data set is located in Final-project-QMSS-GR5069/data/raw/electoral_chile.csv

# Research questions

This project has two research question: 1) what are the most predictive variables of electoral participation among this subset of Chilean youngsters? 2) How predictive are the measures of cognitive skills, namely, math, verbal and history test scores? The first question could be answered by estimating different models (e.g logit regressions, regression trees, random forest). The second question could be answered by interpreting the results of these models. For a longer discussion on the effect of cognitive skills on electoral participation, and the relevance of studying voter turnout with individual-level data and behavioral outcomes, please see Final-project-QMSS-GR5069/reference/motivation/cognitive-skills-electoral-PA-DRAFT.pdf, which is a first draft of paper using this data set. 

# Output

By the end of the semester, we expect to write a report/presentation where we show which variables are more relevant in prediction accuracy, paying special attention to the role of test scores. 




