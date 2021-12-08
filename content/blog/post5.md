---
layout: post
title: "Analysis: IMDb "
date: 2021-12-05T15:26:38+01:00
description: ""
featured_image: "/images/group.jpg"
draft: false
---

To better understand the data we are analysising, we will do some basic statistics with the IMDB dataframe. 

First, we take a glance at the episode distribution.


{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/01-episodes_per_season.json" height="750px"  >}}

The first season was the shortest with only 6 expisodes. After it, the seasons tend to have between 22 and 26 episodes, except the 4th season with only 14 episodes. The longest seasons on the other hand, were season 5 and 6 with 26 episodes each.

### Season Viewership
In this part, we look at the viewership of each season. This concept refers to the average of the show's audience during the entire show and is calculated by computing the mean of the viewership for the season's episodes.


{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/02-viewership_seasons.json" height="450px" >}}
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


Next, the top 10 highest ranked episodes are obtained using the IMDBRating and TotalVotes columns from the IMDB data.


{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/03-top_10_rated_episodes.json" height="450px" >}}
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


It can be observed that the highest rated episodes, both rated at 9.8, are 'Finale' and 'Goodbye, Michael' in season 7 when Michael leaves the show. 

![image info](/images/goodbye_michael.gif) ![image info](/images/finale.gif) 




### Top 10 most viewed episodes
Previously we looked at the viewership of each season, now, we analyse the 10 most viewed episodes of the entire show.


{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/04-most_10_viewed_episodes.json" height="450px" >}}
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


From the graph, one can see similarities between the most viewed and the top rated episodes. Stress Relief is the most viewed episode of all seasons, and at the same time being the 3rd best rated episode. Moreover, Christmas Party and Niagara: Part 1, are both in the top 10 most viewed and top 10 best rated episodes. 

![image info](/images/stress_relief.gif) ![image info](/images/pam_wedding.gif) 


### Season Rating 
We want to analyse how the ratings changed from season to season. Michael left in season 7, did this have an impact in the IMDb ratings? Did the person who replaced Michael as regional manager increase or decrease the ratings? This will later be used when analizing the character sentiments, and their transcripts. 



{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/05-rating_seasons.json" height="450px" >}}
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


We can see that there is an exponential rating growth from season 1 to 5. However, seasons 5 and 6 had a lower rating. And after Michael left, the ratings highly decreased, specially in season 8. We will see if the transcripts can explain this data. However, until now, the ratings and views distributions for the 9 seasons have shown that season 8 and 9 have been the least watched and rated seasons. Is Michael departure the reason?




### IMDB Ratings and Votes for each episode for every season

The season rating analysis showed that the best rated seasons were 2, 3, 4 and 5, with a huge decrease after Michael left in the last episode of season 7. Now, we are going to perform a more detailed analysis by considering the IMDb rating for all the episodes in the Office. 

{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/06-imdb_ratings_votes_episodes.json" height="450px" >}}

\
\
\
\



The above plot offers a more clear representation of what we previously observed. The episodes until Good bye, Michael in season 7, obtain relatively high ratings. However, after Michael leaves, the episode rating is never as high as it was in previous seasons, until the last episode of season 9 'Finale', where Michael comes back.

The number of votes received is more or less the same throught all the episodes, and those episodes with high ratings obtain always high votes. However, all other episodes with rarings around or below 7, obtain around 4000-5000 votes on average.


### Guest stars in every season

Occasionally, guest stars make an appearance in the show, which makes us wander if there is a relation between the number of guest stars that appear in a season and the overall season rating.


{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/07-guest_stars_distribution.json" height="450px" >}}
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

We can see that the number of Guest stars is very low in the first season, but drastically grows in Season 2 to 20.7%. However, the number descreases again in seasons 3 and 4. Then it grows constantly during season 5 to 8 from 10.3% and a maximum of 17.2% in season 7. In the last season, the number of guest stars grows again to be the same as in season 2, 20.7%. 

Based on these statistics, we will now examine if the number of guest starts has an effect on the raiting of the seasons and the top rated episodes.

### Influence of Guest stars in season ratings

Now we are going to put everything together. First, we start by looking if the number of guest stars had an influence in the ratings for all the 9 seasons:

{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/08-ratings_distribution_guest_stars.json" height="450px" >}}
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


Episodes with a greater number of Guest Stars have higher raiting. As it can be seen from the above box plot, the median IMDb raiting is 9.15 when there were 4 guess stars, but only 8.2 when no guest stars appeared in the episode. This could explain why there was an increase in the number of stars in season 9. The producers could have thought that including more guest stars could increase the ratings of the season after the low ratings of season 8. 

However, conclusions cannot be made since the amount episodes containing guest starts is quite limited. However, there is a tendency for the ratings to go up as the number of guest stars increases. 

### Influence of the Guest stars in the season views

We could see that there seems to be a relation between the season's ratings and the guest stars that appear in the season. We further look into the guest stars influence in the seasons popularity by contrasting the number of  guest stars with the season's views.

{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/09-viewership_distribution_guest_stars.json" height="450px" >}}
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

Episodes with one guess star have a higher median rating that those with 0 guess stars. However, as the number of guess stars increases, the views do not neccessarily increse. The average viewership with 4 guess stars in an episode is less than those with one guess star. 

Hence, the guess stars influence the ratings but do not necessarily influence the views.

### Writers influence on the episode ratings
Throught the 9 seasons, episodes have been written by different people. Sometimes even by actors themselves. Let's look at the different writers aand the number of episodes they have writen.

{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/10-writers_episodes.json" height="450px" >}}
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


The three writers who have written the most episodes along the nine seasons are in fact 3 of the main characters of the show.

The three writers who have written the most episodes along the nine seasons are in fact 3 of the main characters of The Office. 
Kelly has written 20 episodes, Ryan 15 and Toby 13. 

![image info](/images/kelly_smart1.gif)
![image info](/images/ryan.gif)
![image info](/images/toby.gif)

Next, we can look into how the episodes writen by these characters are rated according to IMDb:


{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/11-writers_average_episode_ratings.json" height="450px" >}}
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


The episodes written by Greg Daniels, an american screenwriter, are the top rated episodes. However, in second place we can find the episodes writen by Paul Lieberstein, the actor Toby in the series. This shows that he is not only a good actor, but also a talented writer. His episodes are averaged rated with 9.3/10. 

The episodes written by Ryan and Kelly are rated with 8.33 and 8.31, respectively. One point difference from Toby's episodes. 

Hence, Kelly (Mindy Kaling) and Toby (Paul Liberstein) are the top two writers in terms of the number of episodes they have written.

### Director influence on the episode ratings

Similarly to the above analysis, the episodes have been directed by different people, also includint actors themselves.

Let's look at the directors and the number of episodes they directed. 

{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/12-directors_episodes.json" height="450px" >}}


We now look into the average rating for the episodes directed for each of the directors.


{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/13-directors_average_episode_ratings.json" height="450px" >}}
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

### Cast Director influence on the episode ratings

Once again, a few actors of the cast have also been involved in directing episodes. Let's look at their raitings individually: 

{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/14-episodes_rating_directed_by_cast.json" height="750px" >}}

/
/
/

Steve Carell, Michael, has the highest average rating for the 3 episodes he has directed, followed by Mindy Kaling, Kelly, who has directed 2 episodes. 

Out of the 6 actors who directed episodes, the worst performing ones were the ones directed by John Krasinski, Jim, who directed 3 episodes. 

Paul Lieberstein and B.J.Novak are the ones who have been involved the most in the directing and writing of episodes. They have directed 7 and 5 episodes, respectively. And they have written 15 and 13 episodes, respectively. We can conclude however, that Paul Lieberstein is better at writing episodes, than at directing them.
