EDA

Analyzing audience and Sales data of Korean Movie
=================================================
Various variables such as number of audience and total sales were studied in the project. Our goal was to identify variables that affect the success of a movie.

Getting Started
---------------
##### Packages to install
- With the use of Python 3 in Jupyter Notebook, Anaconda
```
pip install pandas
pip install seaborn
pip install matplotlib
pip install warnings
```

##### Dataset
- (536rowsx11columns)
  * genre
  * release date (month,year, season)
  * total screen number
  * total audience
  * total sales
  * point
  * rate
  * actors

Data Exploration:
-----------------
I. Data Cleansing
- Korean movies from 2013~2020 were used.
- Eliminated movies rated 'Adult'.
- 'Total audience' was converted to thousands.
- Actors with the same name were removed from the list.

II. Data Visualization
1. ![image](https://user-images.githubusercontent.com/28764376/102176288-774e0700-3ee4-11eb-9fb0-22c1bc966e07.png)
- Expected that the number of movies released would have decreased in 2020 because of the pandemic.
- Even if year 2020 did not end and more movies may be released, still the number compared to last year has a big difference.



2. ![image](https://user-images.githubusercontent.com/28764376/102176407-a6647880-3ee4-11eb-837a-7162fed19af0.png)
- Expected that, more movies released in a year would mean more number of screens and more audience.
- But instead found that sales and audience increase and decrease in the same movement while number of screens and movie released do not.



<img src="https://user-images.githubusercontent.com/72846750/102710809-53c9f880-42f8-11eb-9141-d6bb6a02cfc6.PNG" width="600" height="400"/>
3. 
- Visualization of sales, audience, number of screens, and point for each top 10 movies to see the movement of the variables in a closer view
- In the closer view, like '7번 방의 선물' more audience does not mean more sales. On the other hand, a similar movement of increase and decrease is observed between the sales and number of screens.



4. ![image](https://user-images.githubusercontent.com/72846750/102452122-258cb480-407d-11eb-9195-3fbdc482ee71.png)
- Sorted by Top 10 Actors who have starred in the most movies during the period mentined above. Total credit count on Top 10 actors is 183.
- Top 10 Actors have appeared on 34.14% of all the movies during the period.
- Top 10 Actors performed remarkably in the Genre of Drama, Crime which is counted above 30, respectively.



5. ![image](https://user-images.githubusercontent.com/72846750/102687765-c2de1900-4234-11eb-99b0-ca578fe00796.png)
- When Top 10 Actors appeared in the movie, it had better performance in the way of number of the Audience and the Screen than the other movies.
- Apparently it doesn't mean that it deserved better points than the other movies.



6. ![image](https://user-images.githubusercontent.com/72846750/102688864-23715400-423d-11eb-8bc7-d5be1849d31d.png)
- As KOBIS has announced earlier, the Movie above Audience 7,000K is so-called "Box-office bomb", which is so rare case for the most of the actors. 
  It turned out all 10 Actors made a huge success more than once during 2013-2020.

Built with
----------
* 김예지
  * Data gathering through API. Data cleansing process. Data visualizing on the overall movie data. (process 1, 2, and 3 of Data Visualization)
  * Github : https://github.com/yeji0701
* 방희란
  * Data cleansing process. Data visualizing on the overall movie data. (process 4, 5 and 6 of Data Visualization)
  * Github : https://github.com/Heeran-cloud
 
Acknowledgements
----------------
- [KOBIS](http://www.kobis.or.kr/kobis/business/main/main.do)
- [Naver movie](https://movie.naver.com/)
