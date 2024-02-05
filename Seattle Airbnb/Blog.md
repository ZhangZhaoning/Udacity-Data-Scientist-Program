![image](https://github.com/ZhangZhaoning/Udacity-Data-Scientist-Program/assets/42299684/6b783d2c-36dd-4787-9633-94c20a7843cd)

# Thoughts on 2016 Seattle Airbnb Market 

Airbnb is one of the best resources for people who are interested in tourism and would like to live in some places have its own style and not like hotels' general services, airbnb could make people feel at home and serve themselves. Many people who have not only one houses/apartment will rent it out or make it an airbnb, the price is based on the market price with some fluacuation based on neighbourhood and apartment type and scraped style. In this analysis, I would like to dive deep into Seattle Airbnb to understand the market of Aribnb there and analyze which factors influence price the most and what's the busiest season for people visiting Seattle.

Based on the data available for Seatlle Airbnb, I'm interetsted in below questions
1. Which area has most listings and which area airbnb averge price is the highest
2. What are the busiest times of the year to visit Seattle
3. What's the most popular property type and room type and how that influence the price.
4. How to leverage Machine Learning to predict Price of an Airbnb, what's the most important features.

For this project I decided to analyse the Seatle Airbnb dataset found on Kaggle: https://www.kaggle.com/code/zacksshen/kaggle-seattle-airbnb using the CRISP-DM Process of:

1. Business Understanding
2. Data Understanding
3. Prepare Data
4. Data Modeling
5. Evaluate the Results

# Data Exploration

To answer these questions we need to undserstand the data from the calendar, reviews and listings first. Below is a brief introduction of what these 3 datasets include:
1. calendar: calendar.csv stores data of airbnb unique id and whether it's available with a price 
2. reviews: reviewers comments on each house
3. listings: stores data with airbnb link and details of the house

calendar.csv stores listings price and host id in a time series format, reviews.csv stores the reviewers' comment information, while listings stores the most information on each airbnb which is interesting and will be the main data source for us to dive deep.

Now Let's take a look at what's included in these dataset in a plot format:

From the plot below we can see most of the airbnb price falls between $100 - $200

![image](https://github.com/ZhangZhaoning/Udacity-Data-Scientist-Program/assets/42299684/15b9a285-cce8-4711-8888-078bd7ab593e)


Checking missing values of the features, we can see some features such as square feet has almost 100% missing values, these features will be dropped in the following steps.
Some features has 10%-20% missing values, we will drop or fill missing values based on its business meanings.

![image](https://github.com/ZhangZhaoning/Udacity-Data-Scientist-Program/assets/42299684/c58a61ec-efa0-4e85-beb8-f0b496726c85)

We just went through the introduction we are gonna use in this analysis, we won't dive deep into all features in this case, to answer our business questions proposed at the beginning, we will leverage matplotlib and seaborn to show some interesting plots. 

### Question 1: What are the busiest times of the year to visit Seattle?
__From below line chart we can see the available uint of seattle is lowest around July which is Summer, this makes sense because summer is best time to visit Seattle. And winter time would have more available unit.__

![image](https://github.com/ZhangZhaoning/Udacity-Data-Scientist-Program/assets/42299684/3df2d71c-43ce-4c08-a5e3-9123bcb7485a)



### Question 2: What's the most popular property type and room type and how that influence the price?
__From below correlation scatterplot result, we can see there's a clear relationship between room type and price, entire home/apt has the highest price and then private room and the cheapest is shared room. And among the listings, entire apartment has the most listings.__

![image](https://github.com/ZhangZhaoning/Udacity-Data-Scientist-Program/assets/42299684/ef2a0ddb-3db2-47c4-b3bd-96de964d1a0d)

![image](https://github.com/ZhangZhaoning/Udacity-Data-Scientist-Program/assets/42299684/29109c50-2cdc-423e-8351-3dbb4ce96d29)


### Question 3: Which area has most listings and which area airbnb averge price is the highest?
__From below sorted bar plot, we can see Broadway has the most listings around 350 and the second one is Belltown. The highest averge price area is Southeast Magnolia  while the second expensive one is Postage Bay. The cheapest area is Rainier Beach__

![image](https://github.com/ZhangZhaoning/Udacity-Data-Scientist-Program/assets/42299684/8ab617cd-655f-43c6-9916-f999cbb66f89)

![image](https://github.com/ZhangZhaoning/Udacity-Data-Scientist-Program/assets/42299684/7b557c57-349c-4746-9040-c2d74daf1397)


# Conclusion

Now we have explored these business questions, there are definitely much more information and interesting topics we have not touched on in this analysis, such as reviewers coment which would use a text mining analysis, we can learn much more information based on the feedback of customers and track whether a bad review will influence the pirce of airbnb in some cases. But from a brief analysis, we can see there are three main factors influencing the price: __season, neighbourhood, room type__

Deployment
I have used Google collab to deploy my code. You may also use Jupyter Notebooks to run the code. The code libraries used and detailed code breakdown is available at GitHub and is explained in the Readme.

This is the GitHub Link: https://github.com/AkshayJaitly/Boston-AirBnb-Analysis.

What’s next:

Use predictive analytics to determine prices in the future. Determine seasonal effects on pricing. Understand more about Superhosts and what makes them special.

Feel free to follow me on GitHub.




