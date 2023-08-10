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
## Question #1: Which age group of criminal homicide victims mostly frequently results in a ‘case closed without arrest’?
__Data Analysis Process :__<br>
1. Using the cleaned Washington Post dataset on Homicide Data, I created a pivot table to display victim age, disposition and COUNTA of case ID.<br>
2. Using the filter function in the pivot table, I filtered the disposition to show only ‘closed without arrest’ on the table.
3. With victim age and disposition under ‘rows’ and case ID under ‘values,’ I sorted the victim age by COUNTA of case ID.<br>

!['#1','Case Closed by Age'](https://github.com/janekenny4/124-Final-Project-Data-Story-Pitch/blob/fdc73d507a810bfe741f0851a2ad0f165d92a1bb/%231.png)

Now, from this pivot table it is clear that the 20s-30s age range most frequently results in a ‘case closed without arrest.’ The data reveals that from 2015-2022 there have been 105 22-year-old criminal homicide victims, the most of any known age.<br>
5. After making my initial observations, I wanted to compare the number of recorded victims aged 20-29 to the number of victims of all other ages. To do this, I began by creating a separate table with one row labeled AGE, which included 20-29, then one row labeled # of CASES, which I filled out to correspond with the COUNTA of case ID in the pivot table. I then found the sum, using the formula =sum(h2:h11) and found that there have been 879 homicides in which the victim age has been identified, and is between 20-29 years old.<br> 

6. Referring back to the pivot table, I added a filter on the basis of victim age – deselecting the values 20-29, to include all ages outside of this specified range.<br> 

7. Removing the 215 victims of unknown ages, I used the =sum formula to find the total number of victims outside of the 20-29 year old age range. The total is 1,828 recorded homicide victims who are not in their twenties, as compared to the 879 victims in the 20-29 year old age range.<br>
This data analysis reveals that about 62.5% of recorded homicide victims were outside of 20-29 years old (on either end), while about 30.1% were aged 20-29 years old and about 7.4% of recorded victims were of an unknown age. To find this, I divided the value of each age category by the total 2,922 reported homicides.<br>
 
## Question #2: Which states have recorded the most criminal homicide cases in which the victim is identified as female? Most male victims?
__Data Analysis Process :__<br>
1. I used the dataset to create a pivot table including state and sex as rows, then placing case ID under values, using COUNTA. 
2. Referring back to the pivot table, I added a filter on the basis of sex – unknown and male, so the pivot table shows data for female victims only. I sorted the COUNTA of case ID in descending order.<br>

3. To meaningfully compare state homicide data on the basis of sex, the changed the filter to deselect female and reselected male. Once again, I sorted to descending order to show the leading states at the top of the pivot table.<br>

The data reveals that the top five states that have recorded the most homicides with female victims are CA with 908 homicides, TX with 802 homicides, IL with 576 homicides, PA with 437 homicides and TN with 383 homicides. Comparatively, the top five states that have recorded the most homicides with male victims are CA with 5,368 homicides, IL with 4,952 homicides, TX with 3,518 homicides, PA with 3,230 homicides and MD with 2,569 homicides. CA, TX, IL and PA are in the top five for homicides of both genders.<br> 

## Question #3:Which city in the United States has the most unsolved criminal homicides?
__Data Analysis Process :__<br>
1. I used the dataset to create a pivot table including city and disposition as rows, then placing case ID under values, using COUNTA.<br>
2. Referring back to the pivot table, I added a filter on the basis of disposition – removing ‘closed by arrest,’ so that only ‘closed without arrest’ and ‘open/no arrest’ appear on the table. These two types of dispositions constitute unsolved homicides.I then sorted the cities by COUNTA of case ID in descending order.<br>

This pivot table reveals that Chicago, Baltimore, Houston, Detroit and Philadelphia are the top cities with the most recorded, but unsolved homicide cases in the United States. Interestingly, Los Angeles has not closed a homicide case without an arrest.<br> 
## Question #4: Which state has recorded the most criminal homicides with black victims?
__Data Analysis Process :__<br>
1. I used the dataset to create a pivot table including victim race as a row, then placing case ID under values, using COUNTA. Then, I changed the case ID value to show as a percentage of the column, so I could more readily see the racial breakdown of the homicide data. I decided to keep ‘other’ as it likely refers to a victim’s mixed racial background.<br>

2. Then, added state as a row, and filtered the victim race display to only show black victims by state. I sorted the states in descending order by COUNTA of case ID.<br>

This pivot table reveals that IL significantly leads the nation in homicides with black victims.<br> 
## Question #5:
__Data Analysis Process :__<br>


# Data Visualization

