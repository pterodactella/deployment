---
layout: post
title: "Analysis: The Office (US) - Complete Dialogue/Transcript"
date: 2021-12-04T00:26:38+01:00
description: ""
featured_image: "/images/group.jpg"
draft: false
---

### Character summary of lines spoken and episodes acted

We start our analysis on the transcript dataset by looking at the line distribution between characters through seasons and the number of episodes where each character acted. We again look at the 25 main characters identified fom the Dunderpedia Wiki. 

Let's now see how many lines the main characters have and in how this varies from season to season:

{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/15-line_count_main_characters.json" height="450px" >}}
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



* **Michael Scott**, the main character and Regional Manager of the Scranton branch is the character with the most lines, and highest **contribution of 22.43%**, even though he left The Office in season 7, and hence did not participate in the last two seasons. At the same time, he participates in only 73% of the episodes, quite less in comparison to **Dwigth Schrute**, assistant (to the) regional manager, which appeared in 98.4% of the episodes, but **contributes 14.09%**, **8.35% less than Michael** and has acted in 49 more episodes than Michael!

* Looking at their contribution percentage, we can see that **Michael, Dwight, Jim** (salesman), **Pam** (receptionist) and **Andy** (salesman and regional manager in season 8)** are the top contributors. However, the other 20 supporting characters starting from **Kevin until Pete** contibute much less than the 5 main characters, ranging from **3.21% from Kevin to 0.44% from Pete**. 

Now, we will analyse the line count by season for each of the main characters, and see who is the main character after Michael left. 


{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/16-line_distribution_seasons.json" height="450px" >}}

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



* We can see that **Michael** is the main character in all the 7 seasons where he participates. The second place is shared by **Dwigth and Jim** through the first 8 seasons. In season 8, **Andy** gets promoted to regional manager, to replace Michael, and hence, he is the character with the most lines in that season. However, in season 9, it is **Dwight** who gets promoted to regional manager. Hence, he is the dominant character with the most lines in that season. We can therefore see a pattern, the regional manager of the Scranton branch is always the character with the most lines.


* This is related to the analysis done with the IMDB ratings. Season 8, after Michael left, is rated as the worst season. This can also be influenced by the fact that Michael's replacement was Andy, who is known not to be liked by the audience. After season 8, Andy was replaced in the role of regional manager by Dwigth, and the ratings went up slightly. Can it be that the writers noticed that Andy was not liked by the audience? We will try to answer this question in the next analyses.


### Share of dialogue throughout the series
Next, we will look into the average number of lines for each main character said in each episode per season.


{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/17-characters_line_distribution_seasons.json" height="450px" >}}
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
\
\
\
\

* **Michael, Dwigth, Jim and Pam** are the ones with the highest contributions for all the seasons. However, After Michael left in season 7, **Dwight, Jim, Pam and Andy** contribute more. In fact, the dialog contibution is more spread and less focused on one single character (Michael), and other characters such as **Kevin, Angela, Oscar or Erin** have more lines in the last two seasons. On the contrary, Jan losses protagonism after season 5 when she losses the position as a manager. 


* Besides, **Darryl** experiences an increase in his dialogue after he moves from the warehouse to the main office in season 7. Then, other primary characters such as **Angela, Kevin, Oscar, Toby, Phyllis, Kelly, Meredith and Stanley** have a consistent growth from season 5. 


### Top speaker influence in the episode rating

We saw, on average, Michael is the top speaker for the 7 seasons where he participates. Now, we want to further investigate if there is a relation between the top speaker in every episode of every season, and that episode IMDb rating. 


{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/18-ratings_distribution_top_speakers.json" height="450px" >}}
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



For all episodes in the 9 seasons, 7 main speakers were identified. 

As we previously suspected, when Michael is the top speaker in an episode, that episode tends to obtain higher ratings. 

However, when **Andy** speaks, the episode ratings are lower. Hence, this explains the low ratings of season 7. However, in season 8, **Andy** was replaced as Regional Manager by **Dwigth**, who also tends to obtain low raitings, an average of 7.8 in comparison to 7.7 from **Andy**. Hence, this also explains why the ratings of season 9 were low. 

A smarter choice would have been to replace **Andy** with **Jim**, which has almost the same success rate when it comes to high episode ratings as **Michael**.

**Nelly** is also the main speaker in some episodes, and although there is not enough data to draw conclusions, the episode were she is the top speaker, obtains a relatively low rating, 6.5, in comparison to the other top speakers.

### Top speaker influence in the episode Viewership 
Let's repeat the previous analysis, but this time let's analyse the influence of the top speaker in episode views.

{{< load-plotly >}}
{{< plotly json="/kaggle_imdb/19-viewership_distribution_top_speakers.json" height="450px" >}}
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

* Once again, **Michael** and **Jim** have a positive influence in the views when they are the top speakers of the episodes. However, when **Pam** is the top speaker, the views are the lowest. This might be because generally she does not make many jokes and she is more calm, so people could see her as boring. 

* On the other hand, **Dwight** has a very specific sense of humor. He is very sarcastic, and not many viewers might understand and/or like it. 

Next we are going to analyse the most iconic jokes and characteristics of each character. Follow **[this post](./post11.md)** for some fun insights.