## Final Project Submission

Please fill out:
* Student name: Felista Kiptoo
* Student pace: Remote
* Scheduled project review date/time: 
* Instructor name: Lucille Kaleha
* Blog post URL:



#### Project Title

### Accident Trends and Risk Factors in Aviation and Insights for Safer Business Operations

### Introduction
Dataset Overview

In this project we will be working with a dataset from the National Transport Safety Boards (NTSB) covering aviation data accident from 1962 to 2023.This dataset provides a comprehensive information on data points such as aircraft involved ,causes of accidents and the severity of accidents etc.

### Objectives 
1. To ensure the dataset is completly clean and accurate for analysis.

2. To analyze the dataset to identify patterns and trends and the risk factors associated with different types of aircraft.

3. To create visualizations and interprate our findings using our dataset.

#### Business Problem 
-The company is expanding in to new industries to diversify its portfolio. Specifically, they are interested in purchasing and operating airplanes for commercial and private enterprises, but do not know anything about the potential risks of aircraft. You are charged with determining which aircraft are the lowest risk for the company to start this new business endeavor. You must then translate your findings into actionable insights that the head of the new aviation division can use to help decide which aircraft to purchase.
  

### Data Understanding

###  Import pandas using the standard alias 


#### Load the dataset 


#### Displaying the first few values 


#### lets display the last rows of dataframe 

#### lets get  about the summary of our dataframe 


##### datatypes = dtypes float64 (5) ,object (26)
#### rows = 90348 entries 
#### columns = 31 columns
#### memory used = 21.4 mb
#### non-null count = this shows the total number of non-missing values in each column and in this case we its only investigation.type that has no missing value all the rest of the columns have missing values. 

#### lets find the summary statistics 

 It gets  summary statistics like the mean, median, min, max, standard deviation, and quartiles of the numerical columns.

### Data Cleaning
We are going to identify missing values and handle them by either imputing missing values,removal ,dropping etc 

We are going also to check for and handle duplicates, inconsistent data formats and outliers in our data

#### Lets check for missing values in our dataframe 


 Drop columns with too many missing values.
 Drop columns where more than a certain threshold of data is missing


 Impute the numerical columns with median e.g Latitudes,longitude, Total.serious.injuries , etc


 impute the categorical columns with modes or placeholder
 



#### Validate the data 


#### Check the results and inspect cleaned data


The Latitude and Longitude data appears cleaned and processed since we have no NaN values ,there is numerical values and the values fall within acceptable geographical ranges:
Latitude: -90 to 90 and Longitude: -180 to 180

#### Lets check for the remaining missing values 


### Exploring and understanding the data 

#### Summarize the data by getting  by generating summary statics 


lets confirm if our dataset is fully cleaned 

Yes great! since our data set is now fully cleaned now we can go ahead to  visualize our dataset by creating charts and graphs and giving our Findings

### Data Visualization & Exploratory Data Analysis(EDA)

Lets understand the distribution of each feature by Using visualizations like histograms, box plots, and scatter plots to identify patterns and relationships within our dataset.

Our main aim is to look for the Root Cause Analysis and Investigate the causes of accidents to see if certain aircraft types are more prone to specific issues. 

we can also analyze our data by looking at the frequency of accidents for different types of aircraft

 Lets use bar chart for counts for each weather condition



# Bar plot
![Image A](Images/imageA.png)


#### Findings 
The graph depicts the distribution of weather conditions with 4 categories:VMC(Visual Meteorological Conditions),IMC(Instrumental Meteorological Conditions),UNK(Unkown),Unk(Lowercase Unknown).

VMC is the most prevalent weather condition in this dataset i.e it has the highest number of counts while IMC and UNK/Unk make up very small proportions of the total

 Fatal Injuries vs Broad Phase of Flight

![Image A](Images/imageB.png)


#### Findings 
This graphs illustrates fatal injuries across different phases of flight.
1. Unknown and other phases have the highest fatal injuries with their bars  nearly reaching the maximum of of scale 1.0.This suggests that many fatal injuries are either not attributed to specific phases or they occur in 'other'.
2. Approach and maneuvering are phases that exhibit high fatal injuries and they indicate that it might be critical stages of flight that are prone to accidents.
3. cruise and decent have moderate fatal injury counts.
4. Taxi and Landing have the least fatal injuries highlighting their safety compared to other phases


![Image A](Images/imageC.png)


#### Findings

This graph illustrates the accident rates by aircraft type(Top 10),with the accidents rate measured in perecentages.
From our graph we can conclude that:
1. Cessna has the highest accident rate among all aircraft types,
2. Piper has the second highest accident rate Beech and boeing and bell have moderate rates accident Grumman,Mooney,Robinson and Hughes have lower rates of accidents with Mooney being the least
3. The dominance of Cessna and Piper in the higher accident rates indicates thats there is need for enhanced safety meausures and pilot training for these aircraft types.
4. Hughes and Belianca have shown lower accidents rates which may reflect stricter regulations and safety protocals



![Image A](Images/imageD.png)


#### Findings
The above graph illustrates severe accidents by aircraft type or make:
1.Cessna make have high rates of number of injuries which is almost more than 20000 which then followed by pipper and boeing which has nearly half number of injuries and bell has the lowest risk  




![Image A](Images/imageE.png)

#### Findings 
This graph illustrates top 10 countries with high accidents rates .This is our Findings:

1.The country with most number of accidents is United States while the rest of the countries have low number of accidents rate in the country 



# Plot number of accidents per year
![Image A](Images/imageF.png)




### Findings
The above graph shows the number of engines vs number of accidentand we can conclude that ;
1. It suggests that single-engine aircraft might be more prone to accidents, possibly due to the lack of redundancy in engine power
2. it also suggests that engines which are doubled-engine are likely to cause accidents but its a small number ,we can also say that more doubled -engines aircraft are the best type of aircraft since the number of accidents are very minimal.


#### Group Data by Flight Purpose and Number of Engines
The following graph shows Number of accidents by flight purpose and number of engines.



![Image A](Images/iamgeG.png)


### Findings 
1. Single engine aircraft are prone to accidents which is evident by spike in accident frequency.
2. Flight purpose like personal and instructional appear more frequent compared to specialized activities like Airdrop,AirRace/show
3. Accidents becomes less frequent as the number of engines increases.


### Bussiness Reccomendation

Basing our analysis from our dataset,we have the following business recommendations:

1. The company should focus on purchasing multi-engine aircraft since the accidents rate are very low and hence they will have to train pilots from transitioning from single-engine to multi-engine planes inorder to handle the complexities of multi-engine systems efficiency.

2. f the company wants to focus on single-engine Aircraft, they shoulod enhance pilot training since most accidents are involved in single-ngine,they should have regular maintainace and create awareness for private owners and operations about the risk associated with single-engine.

 
3.The company should establish a strict maintenance schedule and invest in advanced diagnostic tools and training for maintenaing  personnel ,this will ensure the safety of the aircraft this applies to all makes of aircraft 

4.The company should implement comprehensive training programs and ensure that pilots have ample practice and real-world experience before operating new aircraft. Prioritize hiring pilots with extensive training and experience. 

5.The company should invest in technology inorder to promote development and adoption of advanced safety technologies like automatic emergency landing systems,especially for smaller aircraft






