# 124-Final-Project-Data-Story-Pitch
Jane Kenny's Final Project for J124 Data Journalism at UC Berkeley
# Story Summary
write paragraphs here
# Sourcing
People

Two Additional Sources

# Preparing for Data Analysis
1. Source the Data

2. Clean the Data

3. Ask Questions

4. Define Key Assumptions

# Data Analysis
The following are...
Question #1: Which age group of criminal homicide victims mostly frequently results in a ‘case closed without arrest’?
1. Using the cleaned Washington Post dataset on Homicide Data, I created a pivot table to display victim age, disposition and COUNTA of case ID.
2. Using the filter function in the pivot table, I filtered the disposition to show only ‘closed without arrest’ on the table.
3. With victim age and disposition under ‘rows’ and case ID under ‘values,’ I sorted the victim age by COUNTA of case ID.

Now, from this pivot table it is clear that the 20s-30s age range most frequently results in a ‘case closed without arrest.’ The data reveals that from 2015-2022 there have been 105 22-year-old criminal homicide victims, the most of any known age. 
4. After making my initial observations, I wanted to compare the number of recorded victims aged 20-29 to the number of victims of all other ages. To do this, I began by creating a separate table with one row labeled AGE, which included 20-29, then one row labeled # of CASES, which I filled out to correspond with the COUNTA of case ID in the pivot table. I then found the sum, using the formula =sum(h2:h11) and found that there have been 879 homicides in which the victim age has been identified, and is between 20-29 years old. 

5. Referring back to the pivot table, I added a filter on the basis of victim age – deselecting the values 20-29, to include all ages outside of this specified range. 

6. Removing the 215 victims of unknown ages, I used the =sum formula to find the total number of victims outside of the 20-29 year old age range. The total is 1,828 recorded homicide victims who are not in their twenties, as compared to the 879 victims in the 20-29 year old age range.
This data analysis reveals that about 62.5% of recorded homicide victims were outside of 20-29 years old (on either end), while about 30.1% were aged 20-29 years old and about 7.4% of recorded victims were of an unknown age. 
Question #2:
Question #3:
Question #4:
Question #5:

# Data Visualization

