# Election-survey
A sample data survey is provided for analysis. Sample were collected over a period of nine days where the respondent were ask the question related to election.

## Questions
Question 1 - Load the dataset into a pandas dataframe. Name the variable as “survey”. <br>
Question 2 - How many samples were collected on each day?<br>
Question 3 - What proportion of the total respondents were aged less than 45?<br>
Question 4 - Create a new column in the dataframe “age_group”. This column should contain the age group the respondent belongs to. The age groups are 18-25, 25-40, 40-  55 and 55+. The dataframe should look like this after the column creation.<br>
Question 5 - How many samples were collected for each age-group? Which age-group had the most samples?<br>
Question 6 - What proportion of the respondents had opted for the RJD party in both the Vote_Now and the Past_Vote questions?<br>
Question 7 - For each day of sample collection, determine the proportion of respondents who were fully satisfied with the performance of the CM. So if there were a                  total of 1000 samples on day 1 and 300 out of those said they were fully satisfied, then our answer for that day would be 0.3.<br>
Question 8 - In a similar fashion create a day-wise proportion of respondents that opted fully dissatisfied with their MLA. Create a line plot of the result with date              on x-axis and proportions on the y-axis.<br>
Question 9 - Create a pivot-table (or crosstab) with index as Past_Vote, Column as Vote_Now and cell values as the count of samples.<br>
Answer - survey.pivot_table(index = 'Past_Vote', columns = 'Vote_Now', values = 'response_id', aggfunc = 'count')<br>
Question 10 - Repeat the above question with the cell values as the sum of “weight”.<br>
Question 11 - Create a dataframe by performing a group by over age_group and calculate the count of total samples under each age_group.<br>
Question 12 - Create a dataframe by performing a group by over age_group and finding the count of total samples for each age_group that opted for the JD(U) party in                 Vote_Now.<br>
Question 13 - Join/Merge the two dataframes from questions 12 and 11 with the common column as age_group.<br>

## Functions used in analysis are as-
 head( ) <br>
 unique ( ) <br>
 nunique ( ) <br>
 value_counts ( ) <br>
 dtype <br>
 replace ( ) <br>
 "inplace = True" <br>
 astype ( ) <br>
 Filtering <br>
 Creating a new Column <br>
 copy ( ) <br>
 insert ( ) <br>
 Creating a new Dataframe <br>
 Concatenation (dataframes) <br>
 type ( ) <br>
 Line Chart <br>
 figsize ( ) <br>
 Pivot Table <br>
 Groupby <br>
 count ( ) <br>
 Merge <br>
