# Project Name: Canadian_Immigration_DV
Consider the Canadian Immigration Data set. It is available in Github as well as Kaggle. Using this I perform data manipulation and based on that Data Visualization using python libraries. Libraries that are used here are - **numpy**, **matplotlib**, **pandas**, **seaborn** etc.

## Data Manipulation

The technique to change or transform a data set into another format, so that we can easily use plotting functions on them. Data manipulation basically helps us by providing the mother data set of plottng. For example, suppose we have a data set that has column **Name**. If we can change the index of the data frame by name then we can easily access the rows using those names as loc or iloc parameters. Python library **pandas** is considered as most important data manipulation library, as most of the data manipulation functions come under this library.

## Data Visualization

It is the techniqe of graphically visualizing the data to understand the hidden patterns or making insights from them easily. The advantage of using data visualization is it makes the data story telling very easy, efficient and to the point. Data visualization can be static by graph of runs a  player make or can be dynamic (real time data) like stock market price graph. There are many libraries to create live interactive Dashboards to make plot interactive. The libraries **matplotlib**, **seaborn** creates statisc graphs where as **plotly**, **folium** creates live interactive graphs. **Folium** is used to represent geospatial data effectively.

## About the Cnadian Immigration Data Set

Here we consider the Canadian Immigration Data set. This data set contains information of number of immigrants that came to Canada during the time period 1980 to 2013 for some reasons. It may be Economical crisis (like Pakistan and India) or it may be Natural Phenomenon (like Haiti, 2010 earthquake). This data set 195 rows/observation and 39 columns. Each row/observation represents each country. These 195 countries are grouped into 6 Continents. They are - **Asia**, **Europe**, **Africa**, **Oceania**, **Northern America** and **Latin America and Caribbean**. The columns 1980 to 2013 gives the number of immigrants to Canada in this time gap. Also total number of Immigrants from each country is included in this data set and represented by the **Total** column.

## Project Stages

I gone through some stages to finish the project and making it a well organized one. The stages of the project are well described and to the point. In the project, all the steps are done with notations, so that there will be no problem to understand each part of the project. The steps of the project are - 

**1. Basic Data Exploration:**

In this step, I read the data set using pandas read_csv() function as data. Then I find the first 5 rows/observations of the data frame using .head() method. I also found the shape of the data frame (row and column number). I found the coulmn names and data types of each column. Then I check for any possible mising values in the data set. There is no missing value in thje data set. I then used the .describe() method to get a statistical summary of the numerical columns of the data set (which was the year columns) These are the basic data exploration step.

**2. Data Manipulation:**

As discussed above, data manipulation means transforming the data as our need. In this step, I firstly rename the columns. Then I drop unimportant columns. After that I manually index the data frame by Country. Then using .loc method I fetch value of a country. After that I filter the data frame as per condition specified. After that I Remove the name of index parameter. Here 'Country' (This is optional, done to avoid confusion). Then I write code to get the top 5 and least 5 countries that contribute to Canadian Immigration.

**3. Data Visualization:**

After the data manipulation stage, I used different manipulated data set from the same original data (Canadian Imiigration data, here named as data) to plot graphs of different types. It gives me some hidden patterns and insights that can help every one to understand the data very effectively.

## Data Visualization List

Here , I will cover the data visualization list that I created one by one. They are - Line plot, area plot, pie chart, bubble chart, subplots and regression plot. They are discussed below - 

**1. Line Plot:**

Line plot or line graph is a plot that is used to detect trend in any data. It is good till there are 5 variables. If more than 5 variables are there, these plot doesn't work well. After getting the indexed data set (indexing by country) I fetch the data from India, Pakistan, UK, USA, and China. Then I plot line graphs of them to understand the trend of immigration of these countries to Canada against years (1980-2013). Among all these graphs, I notice that with year, there is an increasing trend in number of immigrations for India.

**2. Area Plot:**

Also known as Area chart. It displays magnitude and proportion of multiple variables over a continuous axis. It represents time or other ordered dimensions. It works best for population demographic data. Here I create an area plot for the countries that contribute to the Immigration data set most. The countries are - **India**, **China**, **UK**, **Philippines** and **Pakistan**. 

**3. Pie Chart:**

Pie chart or pie hraph is a type of data visualization tool that is used to depict the percentage or proportion contribution of an item in any case. It can be percentage of students who scores more than 90 in maths, it can be proportion of teachers that played football etc. In this project, I created a pie chart to depict the percentage contribution of 6 Continets in Immigration data. To do this, first I group the data by the column **Continet** and get the total for each continent by using the .sum() methid on it. As discussed earlier, 6 continents are - **Asia**, **Africa**, **Europe**, **Latin America and Caribbean** and **Northern America**. By the pie chart it is evident that, the decreasing order of these continents are - **Asia(Highest Immigration)**, **Europe(Seconf highest)**, **Africa**, **Latin America and Caribbean** and lastly **Oceania(Lowest Immigration)**.

**4. Comparitive Study of Immigration of World Powers:**

In present day situation, some world power nation includes India, China, USA and UK. To better understand the immigration trend of these four countries and efficiently compare them I created a subplot in which I depict the line plots for each country. It is an easy way by **add_subplot()** method of **Matplotlib** package. In this method, I divide my plotting area into 4 symmetrical regions and then each region is used to plot each country graph.

**5. Bubble Graph:**

Generally use to predict and show if there exsits any hidden association or relationship between numerical variables. Generally it represents data using three variable. For the project, I created two bubble chart. The first one to compare India and Pakistan. The second one is to compare India and China. In both cases, the third variable is the Number of Immigrants. As the size of the circle increases, the number of Immigrants also increases.

**6. Regression Plot:**

A very effective way to understand the trend or relationship between two continuous variable. We can create a regression plot using **Matplotlib** and **Seaborn**. The main difference lies in coding. Using **Matplotlib**, to obtain regression plot, we require much lines of code compare to **Seaborn**. In **Seaborn**, we can do this using just one line. Here, I created a Regression plot for Total number of Immigrations that happens in Denmark, Norway and Sweden with years. Observe that we get a negative relationship. This means with years, the number of Immigrations decreases. 

























