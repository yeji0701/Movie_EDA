EDA

Analyzing audience and Sales data of Korean Movie
=================================================
Does horror movie rank high on summer seasons? Does the movie starring a strong ticket power actor rank higher than those do not? With these curiosities in mind, we decided to look into some data on movie and study on successful. Our goal was to explore, study, and identify variables, such as number of audience and total sales, that affect the success of a movie. 

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



3. <img src="https://user-images.githubusercontent.com/72846750/102710809-53c9f880-42f8-11eb-9141-d6bb6a02cfc6.PNG" width="600" height="400"/> 
- Visualization of sales, audience, number of screens, and point for each top 10 movies to see the movement of the variables in a closer view
- In the closer view, like '7번 방의 선물' more audience does not mean more sales. On the other hand, a similar movement of increase and decrease is observed between the sales and number of screens.



4. ![image](https://user-images.githubusercontent.com/28764376/107944110-fe952500-6fd0-11eb-844d-43c897f10499.png)
- The most number of movies according to genre are '드라마', '코미디', '범죄'. On the other hand, the highest sales according to genre ranks '드라마', '범죄', '액션', number of audience ranks '드라마', '액션', '범죄'.
- Like visualization no.2, this shows that number of screens or number of movies do not relate deeply with sales and number of audience.


5. ![image](https://user-images.githubusercontent.com/72846750/102452122-258cb480-407d-11eb-9195-3fbdc482ee71.png)
- Sorted by Top 10 Actors who have starred in the most movies during the period mentined above. Total credit count on Top 10 actors is 183.
- Top 10 Actors have appeared on 34.14% of all the movies during the period.
- Top 10 Actors performed remarkably in the Genre of Drama, Crime which is counted above 30, respectively.



6. ![image](https://user-images.githubusercontent.com/72846750/102687765-c2de1900-4234-11eb-99b0-ca578fe00796.png)
- When Top 10 Actors appeared in the movie, it had better performance in the way of number of the Audience and the Screen than the other movies.
- Apparently it doesn't mean that it deserved better points than the other movies.



7. ![image](https://user-images.githubusercontent.com/72846750/102688864-23715400-423d-11eb-8bc7-d5be1849d31d.png)
- As KOBIS has announced earlier, the Movie above Audience 7,000K is so-called "Box-office bomb", which is so rare case for the most of the actors. 
  It turned out all 10 Actors made a huge success more than once during 2013-2020.


Conclusion
----------
We were able to see the overall movie industry of Korea and studied what features can affect the success of a movie. First, we were able to see, for the first time, many minor 'Adult' rated films are being released as a movie regularly. Second, number of movies or number of screens throughout the country do not greatly affect the sales and number of audience, which made us look into the actors of each movie. Third, we saw that movies starring the top10 actors (actors sorted with the most number of movies filmed) have more number of audience than movies that do not. In the end of this project, we wondered how it could have improved if data on cost was included. Also, it was too bad we were not able to properly used the season and year column, as time and period could be an important point to think of when releasing a movie.


Built with
----------
* 김예지
  * Data gathering through API.
  * Data cleansing process. Data visualizing on the overall movie data. (process 1, 2, 3, and 4 of Data Visualization)
  * Jupyter notebook uploads and conclusion of this study
  * Github : https://github.com/yeji0701
* 방희란
  * Data cleansing process. Data visualizing on the overall movie data. (process 5, 6, and 7 of Data Visualization)
  * Github : https://github.com/Heeran-cloud
 
Acknowledgements
----------------
- [KOBIS](http://www.kobis.or.kr/kobis/business/main/main.do)
- [Naver movie](https://movie.naver.com/)
