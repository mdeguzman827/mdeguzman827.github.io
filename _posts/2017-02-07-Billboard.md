---
layout: post
title: Billboard Hot 100
--- 

The dataset we are going to explore is the Billboard's Top 100, a list of the most popular songs in America. Our purpose for this project is to analyze the data and see which factors made major hits and stayed at the top of the charts the longest. The underlying question of this is: Why do we like what we like? Are there specific genres the public prefers? Does release date matter? We will examine and attempt to answer these questions.

**Problem Statement**

What makes a song that the public will love? From genre to length of song, there are many factors that can go into what the general public enjoys. Although these rankings are numeric, the preference for songs is subjective to different individuals. Not everyone agrees that the top Billboard songs are the best. Therefore, it is important to take these rankings with a grain of salt. 

**The Data**

The data had problems due to the miscategorization of some songs. Madonna was listed as a Rock genre, along with a few others. The year these songs were relevant were only 2000, so it is likely that public preference has changed due to time. A vast majority of the songs were Rock songs as well, which could skew the results toward favoring Rock genre.

**Reading the Data**

We use pandas to read our data in. Here is a display of the data header. The data contains: year, artist, track, genre, date entered, peak date, length of song, rank, and weeks the song was on the chart.

![_config.yml]({{ site.baseurl }}/images/Screen Shot 2017-02-08 at 12.05.58 AM.png)

The graph below shows each song's rank as a function of time. There is a mysterious drop off for many songs after 19 weeks. This could be because the company forcibly takes the song off the chart if it is beloow rank 50 to open up slots for new songs.

![_config.yml]({{ site.baseurl }}/images/stringy.png)

Since we are measuring success by the length of time it is on the chart, lets get a histogram of every song's timespan that it lasted for in weeks. Below, many songs landed on the left side of the curve, suggesting this is a positive skewed graph as the mean is greater than the median. The mean was about 17 weeks and 


I chose to select specifically for successful songs (lasted longer than 30 weeks). I chose 30 weeks because the mean was about 17 weeks with a standard deviation of 9 weeks. Songs that lasted longer than 30 weeks was 1.5 standard deviations away from the mean, which is better than about 90% of the songs. I would have used 2 standard deviations, but due to limited data, I chose a lower threshold for successful songs. Here is a graph of those songs:

![_config.yml]({{ site.baseurl }}/images/songs.png)

As you can see, most of the successful songs had slower growth. In fact, it took an average of 138 days for a successful song to reach its peak. This shows that slower growth is better if you are trying to prolong the length of time the song is on the chart. It is also notable to see that songs dropped off the chart once it went below rank 50.

Now let's look at the date entered of successful songs:

![_config.yml]({{ site.baseurl }}/images/months.png)

Most of the songs that lasted longer entered in the middle of Q1/Q2 of the year. That is just before summmer. This is significant because it shows that people enjoy listening to the same song as a summer hit. We are all familiar of radios replaying the same song over and over during the summer months. Specifically, Rock songs did very well when entered during this time period. It had a succeess rate of 17.65%.

**Conclusion**

There are a few risks and assumptions I had to make while exploring the data. The data seemed to be biased towards Rock songs, while there were few Reggae or Jazz songs on the chart. It would have been interesting to see how the data would have progressed if each genre was represented equally. Also, many songs mysteriously dropped off the chart exactly after 19 weeks. This could mean the data or source was biased in the subjective ranking. It could also mean Billboard automatically drops some songs immediately after 19 weeks or when their rank drops below 50.

Although there are risks and assumptions, we can see that date entered and genre contribute to the success and length of time a song is on the Billboard Hot 100. I would recommend record labels to release Rock albums just before summer to maximize popularity.
 
