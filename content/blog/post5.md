---
layout: post
title: "IMDB Viewership Analysis"
date: 2021-12-05T15:26:38+01:00
description: ""
featured_image: "/images/group.jpg"
draft: false
---
As mentioned in the previous posts, The Office dataset was expanded IMDB Episode Ratings which will be used all throughout this post.

To help the reader understand the analysed data, a simple statistical analysis with the transcript dataframe will be performed.

First, we take a glance at the number of episodes per season which will come in handy later on when performing the sentiment analysis and computeing the word-clods for every season.

![image info](/images/nr_episodes.png)

The first season was the shortest with only 6 expisodes. After it, the seasons tend to have between 22 and 26 episodes, except the 4th season with only 14 episodes. The longest seasons on the other hand, were season 5 and 6 with 26 episodes each.

### Season Viewership
In this part, one will look at the viewership of each season. This concept refers to the average size of the show's audience during the entire season and is calculated by computing the mean of the viewership for the season's episodes.

![image info](/images/viewership.png)

The average viewership has a consistent growth until season 5. After which, there is a steady decline in views. The lowest viewership is recorded from season 7 to 9 which can be explained by Michael leaving the show. 

### Top 10 highest rated episodes
Next, the top 10 highest ranked episodes are obtained using the IMDBRating and TotalVotes columns from the IMDB data.

![image info](/images/10ratedep.png)

It can be observed that the highest rated episodes, both rated at 9.8, are the Finale episode and the Goodbye, Michael in season 7 when the character leaves the show. 

![image info](/images/goodbye_michael.gif)

### Top 10 most viewed episodes
Previously we looked at the viewership of each season, now, using the same column one can identify the 10 most viewed episodes of the entire show.

![image info](/images/10mostviewed.png)

From the graph, one can see similarities between the most viewed and the top rated episodes. Stress Relief is the most viewed episode of all seasons, and at the same time being the 3rd best rated episode. Moreover, Christmas Party and Niagara: Part 1, are both in the top 10 most viewed and top 10 best rated episodes. 

### Influence of the Guest stars on the views for each season
One can see a relation between the season's ratings and the guest stars that appear in the season. Furthermore, the guest's influence on the seasons popularity can be investigated by contrasting the number of guest stars with the season's views.

![image info](/images/boxplot2.png)

Episodes with one guest star have a higher median rating than those with 0 guest stars. Hovewer, as the number of guests increases, the views do not necessarily increase. The average viewership with 4 guest in an episode is less than those with one guest star.  Hence, ithe guest star influences the ratings but do not necessarily influence the views. 



