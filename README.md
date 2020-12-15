EDA

Analyzing audience and Sales data of Korean Movie
=================================================
Various variables such as number of audience and total sales were studied in the project. Our goal was to identify variables that affect the success of a movie.

Prerequisites:
* Jupyter Notebook
* Python3
* Anaconda

Getting Started
---------------
##### Packages to install
* matplotlib.pyplot
* seaborn
* warnings
* font_manager (matplotlib) - for Korean font
* pandas

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
- But instead found that 'total sales' and 'total audience' increase and decrease in the same movement while number of screens and movie released do not.

Built with
----------
* 김예지
  * Data gathering through API. Data cleansing process. Data visualizing on the overall movie data. (process 1 and 2 of Data Visualization)
  * Github : https://github.com/yeji0701
* 방희란
  * 
  * Github : https://github.com/Heeran-cloud
 
Acknowledgements
----------------
- [KOBIS](http://www.kobis.or.kr/kobis/business/main/main.do)
- [Naver movie](https://movie.naver.com/)
