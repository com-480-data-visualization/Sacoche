# Project : Milestone 1

**Due to 21st March, 5pm**

### Dataset
The dataset we are using is from  [Kaggle](https://www.kaggle.com/datasets) website, which aggregates the data of all the finishers of the Boston Marathon from 2015 to 2017. The datas was extracted from the official marathon website.

Link to the dataset:
- [Finishers Boston Marathon 2015, 2016 & 2017](https://www.kaggle.com/datasets/rojour/boston-results)


### Problematic

Marathons are among the most grueling yet rewarding endurance races in the world, pushing athletes to their physical and mental limits. These events bring together runners of all backgrounds, from elite professionals chasing records to everyday enthusiasts fulfilling personal goals. With its rich history and global prestige, the Boston Marathon stands as one of the most iconic races, attracting thousands of qualified participants each year. Its challenging course, unpredictable New England weather, and passionate spectators make it a unique and highly anticipated event in the running community.

This project aims to explore data from the Boston Marathons held between 2015 and 2017 through a series of interactive visualizations. By analyzing key metrics such as split times (5K, 10K, Half, etc.), finishing times, demographics (age, gender, nationality), and rankings, we seek to answer several questions: How do factors like age and gender impact performance? What pacing strategies lead to the best results? Which countries and cities have the strongest representation? How accurately do projected times reflect actual race outcomes?

The goal of this project is to provide an engaging and accessible way to analyze marathon performance trends, helping runners, coaches, and enthusiasts gain deeper insights into what it takes to succeed in one of the world’s most famous races. Whether you're an aspiring Boston qualifier, a data enthusiast, or simply curious about the patterns behind marathon success, these visualizations will offer a new perspective on the race that has defined endurance running for over a century.

### Exploratory Data Analysis


The marathon dataset collects a large amount of data on participants, including their demographics, times, and performance metrics. The datasets for the years 2015, 2016, and 2017 are extensive,  each containing a large number of rows and features, offering rich material for analysis. The shapes of the datasets are as follows:

2015: (26,598 rows, 25 columns)  
2016: (26,630 rows, 24 columns)  
2017: (26,410 rows, 25 columns)

In the 2016 dataset, there is a missing column, which is labeled as 'Unnamed:'. This column appears to be extraneous and does not contain meaningful data for the analysis.
<p align="center">
  <img src="Images/participants_age_distribution.png" width="500">
</p>
The age distribution shows a variety of participants across different age ranges, with a notable portion in the 30-50 age group, but also representation from younger and older participants. This shows a diverse demographic involved in the event, and the data is reliable for understanding the range of ages.
<p align="center">
  <img src="Images/gender.png" width="45%" style="display:inline-block; margin-right:10px;">
  <img src="Images/gender_distribution.png" width="35%" style="display:inline-block;">
</p>
The gender distribution shows a slight majority of male participants (54.7% vs. 45.3% female). The boxplot of finishing times by gender reveals that women tend to have slightly shorter finishing times, with fewer extreme values compared to men. This indicates a reliable and consistent gender comparison in the dataset.

<p align="center">
  <img src="Images/finishing_times.png" width="500">
</p>
The variations in finishing times across 2015-2017 show some differences, but the overall trends remain similar. This suggests that the dataset is reliable for year-to-year comparisons, although factors like weather or event organization might influence performance.


<p align="center">
  <img src="Images/race_strategy.png" width="500">
</p>
We can see the trend in the race strategy. It is worth noting that Boston Marathon is really comptetitive as we have to qualify for it or pay expensive fees. That is why the strategy of the best runners is quite similar to the average strategy.



### Related work


In this [notebook](https://www.kaggle.com/code/drgilermo/negative-split-and-the-wall), they tried to analize the "negative split" strategy in which the runner runs the 2nd part faster than the 1st part. And the phenomenon of "The Wall" - a condition of sudden fatigue which typically hits the marathon runner after about 30Ks. 

And on [another notebook](https://www.kaggle.com/code/abhishek0032/indian-athletes-marathon-insights-triumph) they focused on Indian runners and used other datasets to see the evolution of the gender difference on multiple distances. Notably, they showed that on very long distance (up to 100km) women can match men speeds.

Our approach is original in the sense that we provide a broader analysis on different race strategies (not only the "negative split") according to level, age, gender, nationality, weather and other factors. And the goal is to provide runners this data so that they visualize what strategy works better according to their condition. And more importantly draw inspiration from other runners' strategies to know what they need to do to step up.

Our main (realistic) source of inspiration is [gapminder](https://www.gapminder.org/tools/#$model$markers$billy$encoding$selected$data$;;;;;;&chart-type=mountain&url=v2). They provide an interactive and even animated visualization of the data. It is really clear and easy to understand the trends. 