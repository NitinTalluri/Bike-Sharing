Bike Sharing Dataset

The dataset has got the hourly and daily count of the rental bikes and the respective weather conditions while renting in the years 2011 and 2012 in the Capital Bikeshare system in Washington DC. It is also induced with some season information humidity levels at the point of renting the bike. This data is obtained from the Capital Bike share system data and the corresponding weather and seasonal information is obtained from the I – weather system. The main or important events in the city can be monitored or can be detected using this bike sharing data. The patterns generated in the process can be used for sensing the mobility in the city. 
Size of the dataset is (17379, 17). The numerical features include temperature, absolute temperature, windspeed, humidity and hour etc., The categorical features include holiday, weekday, month, and season.
The bike sharing rental process is highly correlated to the environmental and seasonal changes or conditions. For example, weather conditions, humidity, season, precipitation, and hour of the day shows a huge impact on the count of the bike that tare being rented. 
Explanation of features:
The main motto behind the usage of this bike sharing data is to predict the bike rental count hourly based on the weather and climatic changes of the environment.
The features in the dataset are as follows:
•	hr: hour (0 to 23)
This will show the hour in which the bike is rented.
•	Season: (1: springer, 2: summer, 3: fall, 4: winter)
The season in which the bike is rented. We consider this feature because users may prefer not to rent a bike during winter and rainy seasons.
•	Year (2011 - 2012):
The year in which the bike is rented.
•	Holiday: 
This feature is considered because users may prefer not to rent a bike during their working days.


Now the main features that showed more correlation to the target value count.
•	temp: Normalized temperature in Celsius.
•	atemp: Normalized feeling temperature in Celsius. (It gives absolute values) 
•	hum: Normalized humidity.  	
•	windspeed: Normalized wind speed.

Target Variables:
The variables that are to be predicted based on the above listed features are as follows, they are
•	casual: count of casual users.
•	registered: count of registered users.
•	cnt: count of total rental bikes including both casual and registered.
The only thing here we need to consider is the number of bikes that are getting rented every moment. Therefore, we do not use the casual and registered elements as part of target variables. Instead, we use the cnt  as the target variable. This will cover all the registered and unregistered users.


Description of the Dataset:
Basic descriptive statistics for the database.
  

The highest number of bike rentals is 977 in the summer season on a holiday and the minimum number of bike rentals is 1, the season at that point of time is springer and the weather situation at that point of time is clear. The mean of the target variable which is cnt (count) is 189.463088. The dataset has (17,379) number of rows and 17 columns of which some are categorical, and some have numeric data in the fields. One of the columns is named instant which is to keep track of the number of records used in the dataset which can be dropped. This data has got some pros and cons, The dataset does not have any missing values or fields in the dataset.
The dataset is skewed in terms of hours when the data is plotted accordingly but this variable is a dependent variable and right skewed. Here there is a necessity to make this variable uniformly distributed. And columns like temp and atemp have high correlation with the target variable and temp tends to show more linearity towards the target variable than atemp.
Columns like casual and registered are highly correlated with the cnt column. Therefore, we might drop those two columns for better and efficient model building.

Preprocessing requirement for the dataset.
The above dataset also requires some preprocessing as there are some outliers in the dataset in terms of some numerical features that might affect the model. Some of the elements in the dataset are skewed therefore we need to normalize them and prepare the train data. After this we can simply test our model efficiency using the test data.



Source of the dataset :
Hadi Fanaee-T
Laboratory of Artificial Intelligence and Decision Support (LIAAD), University of Porto
INESC Porto, Campus da FEUP
Rua Dr. Roberto Frias, 378
4200 - 465 Porto, Portugal

Original Source: http://capitalbikeshare.com/system-data
Weather Information: http://www.freemeteo.com
Holiday Schedule: http://dchr.dc.gov/page/holiday-schedule
![image](https://github.com/NitinTalluri/Bike-Sharing/assets/66375705/bc9875be-5e1c-4b40-aaaa-55c1e178f69f)
