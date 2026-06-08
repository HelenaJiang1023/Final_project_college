**1. Link to final project [to come]**

**2. A technical overview of what has been done for the project** 

Acquire:
1. We acquired our first dataset from the official website of U.S Department of Education College Scorecard using API. This data set is very reliable since it is from an official US government website. The dataset contains real data about almost all colleges and universities in the United States (last updated March 23, 2026). The reliability and wealth of variables of this dataset are the two main reasons for our choice. 
 
2. We acquired our second data set from the kaggle.com, which is a quite reliable website by Google for obtaining csv dataset . We downloaded this second dataset, which contains a list of top colleges in America in 2022, as a csv and imported it into R. We chose this dataset because it provided information about the ranking of the colleges, which is very useful if we want to narrow down our range of analysis and take a closer look at the relationship between graduates outcomes and cost of colleges people want to attend the most. The ranking of college is a potential way to show how much people want to attend the college.
3. We compiled a dataset of Undergraduate Business department graduating senior earning reports, to contrast with CollegeScorecards earnings numbers, which are based entirely on the earnings of the recipients of some form of federal finacial aid. This dataset allowed us to contrast the earnings and outcomes of students with varrying backrounds at a subset of prestigious universities, and interogate the questions of if certain schools provide more of a benefit to students of wealthier backrounds then they do to other types of students.    



Wrangle: We used `left_join` to combine the dataset obtained through API and the `clean_top_colleges.csv` dataset.  With this new combined dataset, we can narrow our analysis down to the top colleges which parents and students want to attend the most and investigate how rank of a college is associated with cost and outcomes. For the college graduation earnings data we used regex to change the existing variable names to allign with the corresponding variable names in the original dataset,then used `inner_join` to obtain a dataset that allowed us to directly compare the difference in outcomes between students at the same universities enrolled in the same programs with different finacial aid status's.

Visualize: For each part of our research questions, we created multiple graphs using ggplot and add interactives through plotly. 

Communicate: For each part of our research questions, we provide write-ups to explain the trend shown in the graphs and the associated implications.


**3 How to nativigate the repo**

`college_final_project. html`: the final project output 
`college_final_project. qmd`: Contain all the codes used to generate output 
