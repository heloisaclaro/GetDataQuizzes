# GetDataQuizzes
Quizzes of the Coursera Getting and Cleaning Data Course

Question 1
The American Community Survey distributes downloadable data about United States communities. Download the 2006 microdata survey about housing for the state of Idaho using download.file() from here: 

https://d396qusza40orc.cloudfront.net/getdata%2Fdata%2Fss06hid.csv 

and load the data into R. The code book, describing the variable names is here: 

https://d396qusza40orc.cloudfront.net/getdata%2Fdata%2FPUMSDataDict06.pdf 

Apply strsplit() to split all the names of the data frame on the characters "wgtp". What is the value of the 123 element of the resulting list?
Your Answer		Score	Explanation
"w" "15"			
"15"			
"wgtp"			
"" "15"	Correct	3.00	
Total		3.00 / 3.00	
Question 2
Load the Gross Domestic Product data for the 190 ranked countries in this data set: 

https://d396qusza40orc.cloudfront.net/getdata%2Fdata%2FGDP.csv 

Remove the commas from the GDP numbers in millions of dollars and average them. What is the average? 

Original data sources: http://data.worldbank.org/data-catalog/GDP-ranking-table
Your Answer		Score	Explanation
377652.4	Correct	3.00	
387854.4			
379596.5			
293700.3			
Total		3.00 / 3.00	
Question 3
In the data set from Question 2 what is a regular expression that would allow you to count the number of countries whose name begins with "United"? Assume that the variable with the country names in it is named countryNames. How many countries begin with United?
Your Answer		Score	Explanation
grep("^United",countryNames), 4			
grep("^United",countryNames), 3	Correct	3.00	
grep("*United",countryNames), 5			
grep("United$",countryNames), 3			
Total		3.00 / 3.00	
Question 4
Load the Gross Domestic Product data for the 190 ranked countries in this data set: 

https://d396qusza40orc.cloudfront.net/getdata%2Fdata%2FGDP.csv 

Load the educational data from this data set: 

https://d396qusza40orc.cloudfront.net/getdata%2Fdata%2FEDSTATS_Country.csv 

Match the data based on the country shortcode. Of the countries for which the end of the fiscal year is available, how many end in June?

Original data sources: 
http://data.worldbank.org/data-catalog/GDP-ranking-table 
http://data.worldbank.org/data-catalog/ed-stats
Your Answer		Score	Explanation
7			
13	Correct	3.00	
15			
16			
Total		3.00 / 3.00	
Question 5
You can use the quantmod (http://www.quantmod.com/) package to get historical stock prices for publicly traded companies on the NASDAQ and NYSE. Use the following code to download data on Amazon's stock price and get the times the data was sampled.
library(quantmod)
amzn = getSymbols("AMZN",auto.assign=FALSE)
sampleTimes = index(amzn) 
How many values were collected in 2012? How many values were collected on Mondays in 2012?
Your Answer		Score	Explanation
252, 50			
251,51			
250, 51			
250, 47	Correct	3.00	
Total		3.00 / 3.00
