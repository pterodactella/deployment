---
layout: post
title: "Kaggle dataset: The Office (US) - Sentiment Analysis"
date: 2021-11-30T21:26:38+01:00
description: ""
featured_image: "/images/group.jpg"
draft: false
---
## Sentiment Analysis

Througout the show each character is exposed to a multitude of feelings, some are in pain and some of them are full of excitement. 
However, from season to season their perception of awareness is changing and one can not be sure which character is the most positive
and who does not share the same enjoyment. To see the variation on the character sentiments, we take a closer look at the transcripts
for each character, we can observe which character is the happiest and who has the lowest sentiment score during each season. 

We calculate the characters sentiments using both the LabMT and Vader methods. Let's analyse the results yield by both methods:

### LabMT method
 

#### Histogram of all characters associated transcripts-sentiments using the LabMT method

From the above histogram, we cannot see much variation on the character sentiments. We can further use the calculated sentiments to get the happiest and saddest characters based on their transcripts during the 9 seasons. We focus on the main characters observing their happiest score and saddest score. 


{{< load-plotly >}}
{{< plotly json="/sentiments/01-labMT_sentiments.json" height="750px" >}}

#### Characters based on sentiment score:
The diagram below represents the happiest and the saddest characters out of the main one's according to LabMT method. We can state that **Karen** is the most positive
of them all, being the regional manager to the Stamford branch she can not afford to have a sad influence on the office. However, it is a bit biased, because of her consistency in the show. She is not as consistent as **Dwight**, appearing every episode, thus, one cas say that the score is a bit biased. The diagram is quite accurate with the saddest characters because **Toby**, **Meredith** and **Erin** are the
saddest characters. **Toby** being constantly bullied by **Michael** for his lack of adventure and monotonous lifestyle. **Erin** going through two break-ups and being parentless, has her own motives not to receive a high sentiment score. **Jim** and **Pam** are in the middle because of their relationship development throughtout the seasons, but did not make the top 5 as like in any other relation sad moments are there as well.

{{< load-plotly >}}
{{< plotly json="/sentiments/02-LabMT-characters.json" height="750px" >}}




### Vader method


#### Histogram of all characters associated transcripts-sentiments using the Vader method

As the previous histogram shows, there is no big decay between the polarity scores of the characters. Most of them are positive and only a few people have some negative thougths that can be interpreted as neutral. It means that the show is rather positive to watch and would only give you good vibes. 

{{< load-plotly >}}
{{< plotly json="/sentiments/03-vader_sentiments.json" height="450px" >}}
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

From the above plot we can see that all the characters are either neutral or positive, but not negative. We can now classify the sentiments based on the polarity to see a more clear distribution.

{{< load-plotly >}}
{{< plotly json="/sentiments/04-sentiment_distribution_vader.json" height="450px" >}}

#### Characters based on sentiment score:


{{< load-plotly >}}
{{< plotly json="/sentiments/05-Vader-characters.json" height="450px" >}}
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

According to the Vader method for calculating sentiment analysis based on each character transcript, **Clark** has the biggest sentiment score. Why would not he,
his only moment of sadness being the fact that he was not promoted to junior salesman as fast as he wanted. After that he became a successful salesman living the dream and making a bright future at Dunder Mifflin.
However his score is biased due to the fact that he did not appear until season five and one can say his presence was not consistent, thus, receiving an overall sentiment score higher than anyone.
**Michael** in the second place stays as the most consistent character according to both methods. Being the regional manager **Michael** had to stay positive 
in order not to bring sad thoughts into the office that will demotivate everyone else. **Jim** and **Pam** have always been good to everyone from the office, besides that
**Pam** was a receptionist and afterthat became the office administrator, meaning that she needed to stay positive while interacting with everyone.
Starting with dwight that has a reathe sarcastic sense of humour which is often interpreted as negative, characters like **Toby**, **Stanley**, **Angela**
and Jan tend to have a lower sentiment score due to the fact that they are mean to everyone else that does not like their lifestyle. **Stanley** and **Jan** were always mean to 
**Michael** because of his nature and lack of responsibility which denotes clearly their low score of happiness. **Toby** being the HR employee was always neutral
suffering from his divorce while **Meredith** treated her sadness with alcohol. 



### Character polarity distribution

The diagram below represents the sentiment score for every main employee from Dunder Mifflin. The first two seasons **Meredith**, **Michael** and **Jim** 
are rather positive, everyone being happy with the way things are. **Michael** being the regional manager, **Jim** constantly pranking **Dwight** and looking 
forward to a relationship with **Pam** and **Meredith** not having yet an alcohol problem. Starting with **Dwight** the characters tend to be more neutral and 
at the bottom of the list there is **Darryl** that is constantly annoyed by **Michael**, **Angela** that only cares about her cats and **Stanley** being the office grump.
**Kelly** is in a constant change of mood and when in season two **Ryan** appears she tends to be more happy.


{{< load-plotly >}}
{{< plotly json="/sentiments/06-characters_polarities_seasons.json" height="450px" >}}
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
\




Season three, four and five keeps **Stanley**'s at the bottom of the list because he does not like to find himself in constant meetings and only loves Pretzel Days.
Moreover, we can observe **Michael** being constantly in top three, meaning that whenever there is a problematic situation in the office he always likes to 
take things positively and develops a multitude of characters to break the created tension in the office. From being neutral **Dwight** drops a few positions back
due to the fact of taking things too serious and being prancked by **Jim**.


Season five and six gives **Toby** a higher sentiment score due to the fact that he is about to leave for Costa Rica and also was invited to participate in the
Scranton Strangler court case as a jury. Because Dunder Mifflin was sold to another company, new characters start to appear like **Gabe**, **Erin**, **Pete** and **Clark**
that have a rather positive score due to the fact that they met their new colleagues and tend to get along with everyone. At the bottom of the list **Meredith**,
**Stanley**, **Darryl** and **Angela** are not pleased with the new changes. 


Season seven is when **Michael** leaves Dunder Mifflin, this being the main reason why he did not make it into top 5. On the other hand Karen has the biggest
happiness score due to the fact of being pregnant. New characters are introduced such as **Robert California**, whit a big sentiment score because of his role as
a CEO of Dunder Mifflin. At the bottom of the list there are the usual names always grumpy and self centered(**Angela**) and Nelie who has filmed in only one series
of that season but still making a bad impression from the begining. 



After **Michael** leaves **Andy** is appointed manager and his dream to be promoted is fulfilled, thus, receiving a high sentiment score. **Nellie** from being last made it into top 
ten due to the fact of being promoted to a higher position and at the characters with the lowest sentiment score being the usual grumpy faces of **Angela**, 
**Stanley**, **Toby** and **Meredith**. 
Season nine has somewhat two biast sentiment scores because both **Roy** and **Michael** appear only in one of the series, and in the middle there is **Dwight**. One can
say that was the most **Dwight** has achieved during the sitcom, thus, he and **Angela** have a higher sentiment score than before.

