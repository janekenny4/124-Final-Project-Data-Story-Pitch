# J124 Data Journalism Final Project: Story Pitch on U.S. Criminal Homicide Data
By Jane Kenny
## Story Summary
For thousands of families, the pain of losing a loved one is magnified by the denial of justice – or even answers. Since the Washington Post began its data collection on criminal homicide cases in the United States in 2015, the publication has recorded 16,505 homicide cases left unresolved. Although impacting every major city across the nation, data shows a wide disparity in the number of unsolved cases in several primary cities in particular. Chicago and Baltimore have amassed the most unsolved homicide cases, while Tampa trails greatly behind with under 100 unsolved cases. I will explore the racial realities behind America’s homicide numbers, as the data indicates that homicides with black victims have the highest unresolvement rate in every single state. To illustrate this, I will comparatively analyze the number of unsolved murders in major cities and population demographics.
## Sources
### The Data
The data used in this project comes from the Washington Post. Since 2015, the publication has collected data on over 52,000 homicides in the United States, including information on location, the victim's racial demographic and if an arrest was made. The original data set can be found [here](https://github.com/washingtonpost/data-homicides). The aggregate data set can be found [here](https://docs.google.com/spreadsheets/d/e/2PACX-1vQ5P8EO1n8b11GTNaKQ8jTERns77HZEc-mP9VQkJ895jzDsmlcAED4fgDMuNmxS_-TInHceDBl65tji/pubhtml).

### Potential Interview Contacts
1. Fred Waller – Interim Superintendent of Police at the Chicago Police Department<br>
Appointed by the mayor of Chicago, Waller is the figure who oversees the entire police department, particularly as it pertains to legislative matters, public coverage and community strategies. As Chicago leads all other major cities in unsolved murders since 2015, I would like to talk to Waller about what the city and department are doing to bring justice to the victims’ families and what types of roadblocks have prohibited resolutions. I would also ask Waller to describe the strategies his force has amended to combat a leading homicide rate. 
I would get in contact with Waller through the Chicago Police Department’s media team, reachable via this email social.media@chicagopolice.org. While a mobile number is not accessible, a second contact would be through the department spokesperson, who can be reached via this email RandD@chicagopolice.org.
2. Liza Bayless – Policy Specialist for the Council on Criminal Justice<br>
Bayless has an extensive background in working with formerly incarcerated individuals and is an expert in criminal justice police. She could offer a unique perspective on unsolved homicides in the Seattle area, as her expertise would round out the details of this story surrounding how conviction and prosecution of murderers plays out. I would ask Bayless about her experience advocating for a less-than-equitable system, and how she works to bring forth justice, as well as promote safety, in her work. 
I can contact Bayless via email lbayless@counciloncj.org or send her a message via LinkedIn linkedin.com/in/lizabayless. 
### Additional Sources
1. This chart breaks down the population in U.S. cities by racial demographic https://public.opendatasoft.com/explore/dataset/us-cities-demographics/table/ .
- I would use this source to illustrate that the cities with higher unsolved murder rates have greater black and POC populations than cities with fewer unsolved homicides. 
- This dataset would contribute to my reporting plan, as it helps to draw a bridge between the violent crime reported, the neglect of investigative forces and how this ties into racial systems of inequity. 
2. The Washington Post investigative report breaks down a similar story, but from five years ago https://www.washingtonpost.com/graphics/2018/investigations/where-murders-go-unsolved/ .
- Not only does this report include a wide variety of data visualizations, but it touches on some of the human faces behind these statistics. In this way, familiarizing myself with real stories could help me to put a real face to an otherwise hard-to-conceive story. 

## Data Analysis

### Question #1: Which age group of criminal homicide victims mostly frequently results in a ‘case closed without arrest’?
__Data Analysis Process :__<br>
1. Using the cleaned Washington Post dataset on Homicide Data, I created a pivot table to display victim age, disposition and COUNTA of case ID.<br>
2. Using the filter function in the pivot table, I filtered the disposition to show only ‘closed without arrest’ on the table.
3. With victim age and disposition under ‘rows’ and case ID under ‘values,’ I sorted the victim age by COUNTA of case ID.<br>

!['#1','Case Closed by Age'](https://github.com/janekenny4/124-Final-Project-Data-Story-Pitch/blob/fdc73d507a810bfe741f0851a2ad0f165d92a1bb/%231.png)

Now, from this pivot table it is clear that the 20s-30s age range most frequently results in a ‘case closed without arrest.’ The data reveals that from 2015-2022 there have been 105 22-year-old criminal homicide victims, the most of any known age.<br>

5. After making my initial observations, I wanted to compare the number of recorded victims aged 20-29 to the number of victims of all other ages. To do this, I began by creating a separate table with one row labeled AGE, which included 20-29, then one row labeled # of CASES, which I filled out to correspond with the COUNTA of case ID in the pivot table. I then found the sum, using the formula =sum(h2:h11) and found that there have been 879 homicides in which the victim age has been identified, and is between 20-29 years old.<br> 

!['#2','20-29 Homicides'](https://github.com/janekenny4/124-Final-Project-Data-Story-Pitch/blob/0abbf4514b9834caeca7612b4afc7ca1a2b95c64/%232.png)

6. Referring back to the pivot table, I added a filter on the basis of victim age – deselecting the values 20-29, to include all ages outside of this specified range.<br> 

7. Removing the 215 victims of unknown ages, I used the =sum formula to find the total number of victims outside of the 20-29 year old age range. The total is 1,828 recorded homicide victims who are not in their twenties, as compared to the 879 victims in the 20-29 year old age range.<br>

!['#3','20-29 Outside Homicides'](https://github.com/janekenny4/124-Final-Project-Data-Story-Pitch/blob/b26cb814d28d43a59708452dc5a18b0a06ff7fdd/%233.png)

This data analysis reveals that about 62.5% of recorded homicide victims were outside of 20-29 years old (on either end), while about 30.1% were aged 20-29 years old and about 7.4% of recorded victims were of an unknown age. To find this, I divided the value of each age category by the total 2,922 reported homicides.<br>
 
### Question #2: Which states have recorded the most criminal homicide cases in which the victim is identified as female? Most male victims?
__Data Analysis Process :__<br>
1. I used the dataset to create a pivot table including state and sex as rows, then placing case ID under values, using COUNTA. 
2. Referring back to the pivot table, I added a filter on the basis of sex – unknown and male, so the pivot table shows data for female victims only. I sorted the COUNTA of case ID in descending order.<br>

!['#4','Females'](https://github.com/janekenny4/124-Final-Project-Data-Story-Pitch/blob/9a94808573c3c2630acc6173de72e734602defd4/%234.png)

4. To meaningfully compare state homicide data on the basis of sex, the changed the filter to deselect female and reselected male. Once again, I sorted to descending order to show the leading states at the top of the pivot table.<br>

!['#5','Males'](https://github.com/janekenny4/124-Final-Project-Data-Story-Pitch/blob/12a2e0a3a15f0dea39f20f1364573ab05a8b979d/%235.png)

The data reveals that the top five states that have recorded the most homicides with female victims are CA with 908 homicides, TX with 802 homicides, IL with 576 homicides, PA with 437 homicides and TN with 383 homicides. Comparatively, the top five states that have recorded the most homicides with male victims are CA with 5,368 homicides, IL with 4,952 homicides, TX with 3,518 homicides, PA with 3,230 homicides and MD with 2,569 homicides. CA, TX, IL and PA are in the top five for homicides of both genders.<br> 

### Question #3:Which city in the United States has the most unsolved criminal homicides?
__Data Analysis Process :__<br>
1. I used the dataset to create a pivot table including city and disposition as rows, then placing case ID under values, using COUNTA.<br>
2. Referring back to the pivot table, I added a filter on the basis of disposition – removing ‘closed by arrest,’ so that only ‘closed without arrest’ and ‘open/no arrest’ appear on the table. These two types of dispositions constitute unsolved homicides.I then sorted the cities by COUNTA of case ID in descending order.<br>

!['#6','Unsolved'](https://github.com/janekenny4/124-Final-Project-Data-Story-Pitch/blob/05ab6ba2f9ced802acc137f6033bb05a9a6e5aaf/%236.png)

This pivot table reveals that Chicago, Baltimore, Houston, Detroit and Philadelphia are the top cities with the most recorded, but unsolved homicide cases in the United States. Interestingly, Los Angeles has not closed a homicide case without an arrest.<br> 
### Question #4: Which state has recorded the most criminal homicides with black victims?
__Data Analysis Process :__<br>
1. I used the dataset to create a pivot table including victim race as a row, then placing case ID under values, using COUNTA. Then, I changed the case ID value to show as a percentage of the column, so I could more readily see the racial breakdown of the homicide data. I decided to keep ‘other’ as it likely refers to a victim’s mixed racial background.<br>

!['#7','Races Number'](https://github.com/janekenny4/124-Final-Project-Data-Story-Pitch/blob/b2c0cf2703c5751e00e1491f6cf6a5b5c38cee4c/%237.png)

!['#8','Races Percent'](https://github.com/janekenny4/124-Final-Project-Data-Story-Pitch/blob/8e45e9459f5153bcfb7691ab7fc6dbf144ec15f3/%238.png)

2. Then, added state as a row, and filtered the victim race display to only show black victims by state. I sorted the states in descending order by COUNTA of case ID.<br>

!['#9','Black victims by state'](https://github.com/janekenny4/124-Final-Project-Data-Story-Pitch/blob/1ef6e37d7864cefb4df0a5a075a1439ad76a68b2/%239.png)

This pivot table reveals that IL significantly leads the nation in homicides with black victims.<br> 
### Question #5: Which race has the highest percentage of unsolved homicide cases in each state?
__Data Analysis Process :__<br>
1. Using the cleaned dataset, created a pivot table that included state and victim race as rows, then placed case ID under values as COUNTA.<br>
2. Filtered the disposition to show the two types of unsolved cases.<br>

!['#10','Unsolved By Race'](https://github.com/janekenny4/124-Final-Project-Data-Story-Pitch/blob/332e14bdf98688c2130d72fa16527045d531dda8/%2310.png)

3. To calculate percentage for each state, I used the equation (highest # race)/total for each state.<br>

This data overwhelmingly reveals that in all states the racial demographic for victims of unsolved homicide cases is black.

### Data Visualization Link
Utilizing data from the Washington Post, I created a line chart to illustrate the number of unsolved murders in major cities across the United States. This chart visualizes the significant disparity between various cities – and a further comparison would reveal this disproportion as backed by systemic racism.<br>

!['#11','Data Viz'](https://github.com/janekenny4/124-Final-Project-Data-Story-Pitch/blob/40eea111fe541c69741551aa282ae71fc25b76ba/%2311.png)

https://datawrapper.dwcdn.net/AOiqF/1/ 
