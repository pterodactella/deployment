---
layout: post
title: "Kaggle dataset: The Office (US) - Basic Statistics "
date: 2021-12-03T20:26:38+01:00
description: ""
featured_image: "/images/group.jpg"
draft: false
---
We further expand the datased by including the Complete Dialogue/Transcript. After formatting the data, once can look at how many lines the main characters have and how this varies from season to season. 

![image description](/images/lines.png)
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

Michael, the main character and Regional Manager of the Scranton branch is the character with the most lines, which can also be seen from the graph above, even though he left the show in season 7 and did not participate in the last two seasons. Now, we will dive into the line count by season for each of the main characters, and see who became the main character after Michael has left The Office.

![image description](/images/lines2.png)

For the first 7 seasons, Michael stayed the main character. The second place is shared by Dwight and Jim through the first 8 seasons. In season 8, Andy gets promoted to regional manager, to replace Michael, and hence, he is the character with most lines during season 8. However, in season 9, it is Dwight who gets promoted to regional manager, thus being the dominant character of the season. Consequently, a correlation can be seen between who is the regional manager od the Scranton brach and the character with most lines.

This is related to the analysis done with the IMDB ratings. Season8, after Michael left, is rated as the worst season. This can also be influenced by the fact that Michael's replacement was Andy, who is known not to be liked by the audience. After season 8, Andy was replaced in the role of regional manager by Dwigth, and the ratings went up slightly. Can it be that the writers noticed that Andy was not liked by the audience? 


### **Share of dialogue throughout the series**
Next, we will peek into the average number of lines for each main character said each episode per season.

![image description](/images/shared_dialogue.png)

Michael, Dwigth, Jim and Pam are the ones with the highest contributions for all the seasons. However, After Michael left in season 7, Dwight, Jim, Pam and Andy contribute more. In fact, the dialog contibution is more spread and less focused on one single character (Michael), and other characters such as Kevin, Angela, Oscar or Erin have more lines in the last two seasons. On the contrary, Jan losses protagonism after season 5 when she losses the position as a manager. 

Darryl experiences an increase in his dialogue after he moves from the warehouse to the main office. Then, other primary characters such as Angela, Kevin, Oscar, Toby, Phyllis, Kelly, Meredith and Stanley have a consistent growth from season 5 due to the fact that the tv show is not as self centered to the one character. 

### **Top speaker influence on the episode rating**

It was seen that on average, Michael is the top speaker for the first 7 seasons. However, it is time to investigate whether a relation between the top speaker in every episode of every season and the IMDb rating exists.


![image description](/images/boxplot3.png)



For all episodes in the show, 7 main speakers were identified. 

As we previously suspected, when Michael is the top speaker in an episode, that episode tends to obtain higher ratings. 

However, when Andy speaks, the episode ratings are lower. Hence, this explains the low ratings of season 7. However, in season 8, Andy was replaced as Regional Manager by Dwigth, who also tends to obtain low raitings, an average of 7.8 in comparison to 7.7 from Andy. Hence, this also explains why the ratings of season 9 were low. 

A smarter choice would have been to replace Andry with Jim, which has almost the same success rate when it comes to high episode ratings as Michael.

### **Top speaker influence on the episode Viewership** 
Let's repeat the previous analysis, but this time let's analyse the influence of the top speaker in episode views.


{{< load-plotly >}}
{{< plotly json="/viewership_distribution_top_speakers.json" height="450px" >}}

Once again, Michael and Jim have a positive influence in the views when they are the top speakers of the episodes. However, when Pam is the top speaker, the views are the lowest. This might be because generally she does not make many jokes and she is more calm, so people could see her as boring. 

On the other hand, Dwight has a very specific sense of humor. He is very sarcastic, thus viewers might understand and/or like it. 


### **How many times the characters say their favorite lines?**

#### **That's what shes said**

![Alt Text](/images/michael.gif)


First, let's look into the number of 'That's what she said jokes' made throughout all 9 seasons.

![image description](/images/joke1.png)

The number of "That's what she said" jokes starts in season 2 and grows until season 4 after which the joke is not said as often. In season 7 when Michael leaves, no one says it. Then, in season 9, it is said again Once by Michael and once by Creed. The person who says the joke the most is Michael, who repeated the joke 23 times.

#### **Dunder Mifflin, this is Pam**
As the receptionist, for the first 4 seaons, whenever Pam was answering the phone, she was said: 'Dunder Mifflin, this is Pam'. Let's look into how many times she actually said it:
![Alt Text](/images/pam.gif)

The number of times Pam responded this way is 18.

#### **Number of times Angela talks about her Cats**

![Alt Text](/images/angela.gif)

The number of times Angela talks about her cats is 37.


#### **Number of times Andy calls Jim Tuna**

![Alt Text](/images/andy_tuna.gif)

The number of times Andy calls Jim Tuna is 54.


#### **Number of times Kelly calls or talks about Ryan**

![Alt Text](/images/kelly.gif)

Kelly calls or talks about Ryan 12 times.


#### **Number of Times Dwight says Assistant Regional Manager **

![Alt Text](/images/dwight.gif)

Dwight says Assistant Regional Manager is 20 times.

