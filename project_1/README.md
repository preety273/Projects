# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Testing, Statistical Summaries and Inference


### Overview and Problem Statement 


Though standardized tests such as **American College Testing (ACT)** and **Standardised Aptitude Tests (SAT)** are considered by a number of states as a prerequisite for higher education enrolment in the universities in United States, according to recent statistics produced by National Center for Fair and Open Testing (Fair Test) – a non-profit civil society group – more than a 1,000 four-year colleges and universities in the US have discontinued the practise of mandatory SAT or ACT scores for student admissions. These colleges and universities are spread across the US and now include some of the top institutions such as the University of Chicago. 

Given this increasing trend against standardised exams, what measures should be taken to increase the total participation of high school students in ACT or SAT? 

---

### Executive Summary


This project investigates the data on participation rates and average scores for students taking the SAT and ACT exams in all US states. The data contains participation rates and total/composite and section scores for the year 2017 and 2018. Since the data is organised state-wise, it allows for state-to-state comparison of participation rates and scores for each tests. 

Broad observation of dataset reveals the following trends:

- Many states in the US mandate taking either SAT or ACT as a requirement for high school graduation. Currently, a total of 16  states have made ACT mandatory for high school graduation, 9 states have SAT as the basic requirement for high school graduation and 2 states mandate students to either take SAT or ACT tests before graduating high school. These states also have the highest participation of students in SAT or ACT exams depending upon the mandated exam set by the state. State policy is a major factor in students participation. 

- Very few students choose to take both the tests. There is a negative correlation between participation rates for SAT and ACT exams. 

- There is also a negative correlation between participation rate and average scores for both the exams. Higher the number of students taking the tests; lower are the average scores or vice-versa. 

- This negative correlation can be explained by the fact that higher participation rates are often a result of state policy and making these exams mandatory creates a compulsion among non-interested students to give the tests. 

---

### Datasets


The project uses the following datasets. 

- [2017 SAT Scores](./data/sat_2017.csv)
- [2017 ACT Scores](./data/act_2017.csv)
- [2018 SAT Scores](./data/sat_2018.csv)
- [2018 ACT Scores](./data/act_2018_updated.csv)

These data give average SAT and ACT scores by state, as well as participation rates, for the graduating class of 2017 and 2018.

---

### Data Dictionary


|Variable|Type|Dataset|Description|
|---|---|---|---|
|state|object|SAT (2017, 2018), ACT (2017, 2018)|Name of the state|
|percent_of_students_taking_SAT_2017|float|SAT 2017|Percentage of the total high school graduates in each state who took the SAT test in a given year|	
|SAT_average_reading_and_writing_score_2017|integer|SAT 2017|Average of the scores of all the test takers on the Evidence-based Reading and Writing section of the test for each state in a given year| 
|SAT_average_math_score_2017|integer|SAT 2017|Average of the scores of all the test takers on the Math section of the test for each state in a given year| 
|SAT_total_average_score_2017|integer|SAT 2017|Total average scores of all the test takers for each state in a given year| 	
|percent_of_students_taking_ACT_2017|float|ACT 2017|Percentage of the total high school graduates in each state who took the ACT test in a given year| 	
|ACT_average_english_score_2017|float|ACT 2017|Average of the scores of all the test takers on the English section of the test for each state in a given year| 	
|ACT_average_math_score_2017|float|ACT 2017|Average of the scores of all the test takers on the Math section of the test for each state in a given year| 
|ACT_average_reading_score_2017|float|ACT 2017|Average of the scores of all the test takers on the Reading section of the test for each state in a given year| 	
|ACT_average_science_score_2017|float|ACT 2017|Average of the scores of all the test takers on the Science section of the test for each state in a given year| 	
|ACT_total_average_score_2017|float|ACT 2017|Total average scores of all the test takers for each state in a given year| 	
|percent_of_students_taking_SAT_2018|float|SAT 2018|Percentage of the total high school graduates in each state who took the SAT test in a given year| 	
|SAT_average_reading_and_writing_score_2018|integer|SAT 2018|Average of the scores of all the test takers on the Evidence-based Reading and Writing section of the test for each state in a given year| 	
|SAT_average_math_score_2018|integer|SAT 2018|Average of the scores of all the test takers on the Math section of the test for each state in a given year| 	
|SAT_total_average_score_2018|integer|SAT 2018|Total average scores of all the test takers for each state in a given year| 	
|percent_of_students_taking_ACT_2018|float|ACT 2018|Percentage of the total high school graduates in each state who took the ACT test in a given year| 	
|ACT_total_average_score_2018|float|ACT 2018|Total average scores of all the test takers for each state in a given year| 	
|ACT_average_english_score_2018|float|ACT 2018|Average of the scores of all the test takers on the English section of the test for each state in a given year| 	
|ACT_average_math_score_2018|float|ACT 2018|Average of the scores of all the test takers on the Math section of the test for each state in a given year| 
|ACT_average_reading_score_2018|float|ACT 2018|Average of the scores of all the test takers on the Reading section of the test for each state in a given year| 	
|ACT_average_science_score_2018|float|ACT 2018|Average of the scores of all the test takers on the Science section of the test for each state in a given year| 

---

### Conclusion and Recommendations

Three states are selected as a case study, namely, Colorado, Illinois and Florida, on the basis of some interesting trends observed in the participation rates for these states. 

Out of these, the state of low participation rate in both ACT and SAT is Florida. The case of Florida is interesting because the participation rate has decreased considerably between 2017 and 2018. Unlike any other state, Florida is the only state where both ACT and SAT participation rates have come down. Through external research, we can now come to a definitive conclusion of why these rates are falling and what can be done to arrest the fall in participation rates. 

1) First, both the College Board and ACT must realign some of their exams to better suit the individual needs of the Florida state. As we saw in case of successes such as Colorado and Illinois, relevance to existing school curriculum is fundamentally determinative of a state’s choice to incorporate these tests in their high school graduation programs. 

2) Second, both SAT and ACT have to address the issue of accommodation of social, gender, economic and ethnic differences into their test scores. Making the tests more representative of a student’s background will help address the biases such tests would have against underprivileged students. This will help address not only the requirements set by the Florida Board of Education but would also help in countering the arguments forwarded by organisations such as FairTest against standardized exams. 
