# Election-survey
A sample data survey is provided for analysis. Sample were collected over a period of nine days where the respondent were ask the question related to election.

## Questions
Question 1 - Load the dataset into a pandas dataframe. Name the variable as “survey”.
Question 2 - How many samples were collected on each day?
Question 3 - What proportion of the total respondents were aged less than 45?
Question 4 - Create a new column in the dataframe “age_group”. This column should contain the age group the respondent belongs to. The age groups are 18-25, 25-40, 40-55 and 55+. The dataframe should look like this after the column creation.
Question 5 - How many samples were collected for each age-group? Which age-group had the most samples?
Question 6 - What proportion of the respondents had opted for the RJD party in both the Vote_Now and the Past_Vote questions?
Question 7 - For each day of sample collection, determine the proportion of respondents who were fully satisfied with the performance of the CM. So if there were a total of 1000 samples on day 1 and 300 out of those said they were fully satisfied, then our answer for that day would be 0.3.
Question 8 - In a similar fashion create a day-wise proportion of respondents that opted fully dissatisfied with their MLA. Create a line plot of the result with date on x-axis and proportions on the y-axis.

Question 9 - Create a pivot-table (or crosstab) with index as Past_Vote, Column as Vote_Now and cell values as the count of samples.
Answer - survey.pivot_table(index = 'Past_Vote', columns = 'Vote_Now', values = 'response_id', aggfunc = 'count')

Question 10 - Repeat the above question with the cell values as the sum of “weight”.
Question 11 - Create a dataframe by performing a group by over age_group and calculate the count of total samples under each age_group.
Question 12 - Create a dataframe by performing a group by over age_group and finding the count of total samples for each age_group that opted for the JD(U) party in Vote_Now.
Question 13 - Join/Merge the two dataframes from questions 12 and 11 with the common column as age_group.

## Functions used in analysis are as-
 head( ) 
 unique ( ) 
 nunique ( ) 
 value_counts ( ) 
 dtype 
 replace ( ) 
 "inplace = True" 
 astype ( ) 
 Filtering 
 Creating a new Column 
 copy ( ) 
 insert ( ) 
 Creating a new Dataframe 
 Concatenation (dataframes) 
 type ( ) 
 Line Chart 
 figsize ( ) 
 Pivot Table 
 Groupby 
 count ( ) 
 Merge 
