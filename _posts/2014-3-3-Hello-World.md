---
layout: post
title: Billboard Hot 100
--- 

The dataset we are going to explore is the Billboard's Top 100, a list of the most popular songs in America. Our purpose for this project is to analyze the data and see which factors made major hits and stayed at the top of the charts the longest. The underlying question of this is: Why do we like what we like? Are there specific genres the public prefers? Does release date matter? We will examine and attempt to answer these questions.

**Problem Statement**

What makes a song that the public will love? From genre to length of song, there are many factors that can go into what the general public enjoys. Although these rankings are numeric, the preference for songs is subjective to different individuals. Not everyone agrees that the top Billboard songs are the best. Therefore, it is important to take these rankings with a grain of salt. 

**The Data**

The data had problems due to the miscategorization of some songs. Madonna was listed as a Rock genre, along with a few others. The year these songs were relevant were only 1999 and 2000, so it is likely that public preference has changed due to time. A vast majority of the songs were Rock songs as well, which could skew the results toward favoring Rock genre.

**Reading the Data**

Here is a display of the data header. The maximum length on the chart is 76 weeks.

![_config.yml]({{ site.baseurl }}/images/Screen Shot 2017-02-08 at 12.05.58 AM.png)

I chose to select specifically for successful songs (lasted longer than 30 weeks). Here is a graph of those songs:



As you can see, most of the successful songs had slower growth. In fact, it took an average of 138 days for a successful song to reach its peak. This shows that slower growth is better if you are trying to prolong the length of time the song is on the chart. It is also notable to see that songs dropped off the chart once it went below rank 50.

Now let's look at the release date of successful songs:


Most of the songs the lasted longer were released int the middle of Q1/Q2 of the year. That is just before summmer. This is significant because it shows that people enjoy listening to the same song as it prolongs as a summer hit. Specifically, Rock songs did very well when released during this time period. It had a succeess rate of 17.65%.

**Conclusion**

We can see that release date and genre contribute to the success and length of time a song is on the Billboard Hot 100. I would recommend record labels to release Rock albums just before summer to maximize popularity.


The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.
