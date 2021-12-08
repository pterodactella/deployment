---
layout: post
title: "IMDB Viewership and Rating Analysis"
date: 2021-12-05T15:26:38+01:00
description: ""
featured_image: "/images/group.jpg"
draft: false
---
As mentioned in the previous posts, The Office dataset was expanded IMDB Episode Ratings which will be used all throughout this post.

To help the reader understand the analysed data, a simple statistical analysis with the transcript dataframe will be performed.

First, we take a glance at the number of episodes per season which will come in handy later on when performing the sentiment analysis and computeing the word-clods for every season.


{{< load-plotly >}}
{{< plotly json="/01-episodes_per_season.json" height="450px" >}}
\
\
\
\
\
\
\
\
\
\
\
\


The first season was the shortest with only 6 expisodes. After it, the seasons tend to have between 22 and 26 episodes, except the 4th season with only 14 episodes. The longest seasons on the other hand, were season 5 and 6 with 26 episodes each.

### Season Viewership
In this part, one will look at the viewership of each season. This concept refers to the average size of the show's audience during the entire season and is calculated by computing the mean of the viewership for the season's episodes.


{{< load-plotly >}}
{{< plotly json="/02-viewership_seasons.json" height="450px" >}}
\
\
\
\
\
\
\
\
\
\
\


The average viewership has a consistent growth until season 5. After which, there is a steady decline in views. The lowest viewership is recorded from season 7 to 9 which can be explained by Michael leaving the show. 

### Top 10 highest rated episodes
Now we look at the rating for all episodes.
{{< load-plotly >}}
{{< plotly json="/06-imdb_ratings_votes_episodes.json" height="450px" >}}



Next, the top 10 highest ranked episodes are obtained using the IMDBRating and TotalVotes columns from the IMDB data.


{{< load-plotly >}}
{{< plotly json="/03-top_10_rated_episodes.json" height="450px" >}}


It can be observed that the highest rated episodes, both rated at 9.8, are the Finale episode and the Goodbye, Michael in season 7 when the character leaves the show. 

![image info](/images/goodbye_michael.gif)


### Top 10 most viewed episodes
Previously we looked at the viewership of each season, now, using the same column one can identify the 10 most viewed episodes of the entire show.


{{< load-plotly >}}
{{< plotly json="/04-most_10_viewed_episodes.json" height="450px" >}}

From the graph, one can see similarities between the most viewed and the top rated episodes. Stress Relief is the most viewed episode of all seasons, and at the same time being the 3rd best rated episode. Moreover, Christmas Party and Niagara: Part 1, are both in the top 10 most viewed and top 10 best rated episodes. 

### Influence of the Guest stars on the views for each season
One can see a relation between the season's ratings and the guest stars that appear in the season. Furthermore, the guest's influence on the seasons popularity can be investigated by contrasting the number of guest stars with the season's views.


{{< load-plotly >}}
{{< plotly json="/09-viewership_distribution_guest_stars.json" height="450px" >}}

Episodes with one guest star have a higher median rating than those with 0 guest stars. Hovewer, as the number of guests increases, the views do not necessarily increase. The average viewership with 4 guest in an episode is less than those with one guest star.  Hence, ithe guest star influences the ratings but do not necessarily influence the views.



### Season Rating 
The analysis continues with identifying how the ratings changed from season to season. Which will be used later on when looking at the character sentiments and their transcripts. 



{{< load-plotly >}}
{{< plotly json="/05-rating_seasons.json" height="450px" >}}

Looking at the graph, an exponantial rating growth fro season 1 to season 5 can be observed. Season 5 and 6 had a lower rating which was overcame by season 7. Succeeded by a high decrease in ratings after Michael's withdraw. The bottom rating is scored in season 8 making it the lowest rated season of the series. 

### Correlation between guest stars and season rating

Occasionally, guest stars make an appearance in the show, which makes us wander if there is a relation between the number of guest stars that appear in a season and the overall season rating.

Using the guest stars distribution, the following plot is computed. 

{{< load-plotly >}}
{{< plotly json="/07-guest_stars_distribution.json" height="450px" >}}

We can see that the number of Guest stars starts very low in the first season, but drastically grows in Season 2 to 20.7%. However, the number descreases again in seasons 3 and 4. Then it grows constantly during season 5 to 8 from 10.3% and a maximum of 17.2% in season 7. In the last season, the number of guest starts grows again to be the same as in season 2. 

Based on these statistics, we will examine if the number of guest starts has an effect on the raiting of the seasons and the top rated episodes using the number if the guest stars from all 9 season and each season's rating. 

{{< load-plotly >}}
{{< plotly json="/08-ratings_distribution_guest_stars.json" height="450px" >}}

Episodes with a greater number of Guest Stars have a higher raiting. As it can be seen from the above box plot, the median IMDb raiting is 9.15 when there were 4 guess stars, but only 8.2 when no guest stars appeared in the episode. This could explain why there was an increase in the number of stars in season 9. The producers could have thought that including more guest stars could increase the ratings of the season after the low ratings of season 8. 

### Writers influence on the episode ratings
Throughout the 9 seasons, episodes have been written by different people including actors. In order to look into the influence of the writer on the episode's rating, first one must look at the different writers and number of episodes written by them.

{{< load-plotly >}}
{{< plotly json="/10-writers_episodes.json" height="450px" >}}

The three writers who have written the most episodes along the nine seasons are in fact 3 of the main characters of the show.

The three writers who have written the most episodes along the nine seasons are in fact 3 of the main characters of The Office. 
Kelly has written 20 episodes, Ryan 15 and Toby 13. 

![image info](/images/kelly_smart1.gif)

Next, we can look at the IMDb rating for the episodes written by these characters .


{{< load-plotly >}}
{{< plotly json="/11-writers_average_episode_ratings.json" height="450px" >}}

The episodes written by Greg Daniels, an american screenwriter are the top rated episodes. However, in second place are located the episodes written by Paul Lieberstein, the actor Toby in the series. This shows that he is not only a good actor but also a talented writers as his episodes have an average rating of 9.3/10.

The episodes written by Ryan and Kelly are rated with 8.33 and 8.31, respectively. One point difference from Toby's episodes. Hence, Kelly (Mindy Kailing) and Toby (Paul Lieberstein) are the top two writers of the number of episodes they have written.

### Director influence on the episode ratings

Similarly to the above analysis, the episodes have been directed by different people, also includint actors themselves.

The first graph below, displays the directors and the number of episodes they directed. The second graph shows the average rating for the episodes directed for each of the directors.



{{< load-plotly >}}
{{< plotly json="/12-directors_episodes.json" height="450px" >}}


{{< load-plotly >}}
{{< plotly json="/13-directors_average_episode_ratings.json" height="450px" >}}
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\


Randall Einhorn and Paul Feig have directed the most number of episodes. At the same time, looking at the top 10 rated episodes we can see that Paul has directed 5 out of the top most rated episodes: Goodbye Michael, Goodbye Toby, Niagara:Part 1 and 2 and Dinner party. However, Randall has not directed any of the top 10 rated episodes.

On the other hand, Steve Carell, who plays as Michael, has the highest Average Rating for all his directed episodes. Although he has only directed 3 episodes.

Once again, a few actors of the cast have also been involved in directing episodes. Let's look at their raitings individually: 

{{< load-plotly >}}
{{< plotly json="/14-episodes_rating_directed_by_cast.json" height="450px" >}}

Steve Carell, Michael, has the highest average rating for the 3 episodes he has directed, followed by Mindy Kaling, Kelly, who has directed 2 episodes. 

Out of the 6 actors who directed episodes, the worst performing ones were the ones directed by John Krasinski, Jim, who directed 3 episodes. 

Paul Lieberstein and B.J.Novak are the ones who have been involved the most in the directing and writing of episodes. They have directed 7 and 5 episodes, respectively. And they have written 15 and 13 episodes, respectively. We can conclude however, that Paul Lieberstein is better at writing episodes, than at directing them.

