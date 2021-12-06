---
layout: post
title: "Kaggle dataset: The Office (US) - Sentiment Analysis"
date: 2021-12-04T21:26:38+01:00
description: ""
featured_image: "/images/group.jpg"
draft: false
---
### **Sentiment Analysis**
Througout the show each character is exposed to a multitude of feelings, some are in pain and some of them are full of excitement. 
However, from season to season their perception of awareness is changing and one can not be sure which character is the most positive
and who does not share the same enjoyment. To see the variation on the character sentiments, we take a closer look at the transcripts
for each character, we can observe which character is the happiest and who has the lowest sentiment score during each season. 
The diagram below represents the sentiment score for every main employee from Dunder Mifflin. The first two seasons Meredith, Michael and Jim 
are rather positive, everyone being happy with the way things are. Michael being the regional manager, Jim constantly pranking Dwight and looking 
forward to a relationship with Pam and Meredith not having yet an alcohol problem. Starting with Dwight the characters tend to be more neutral and 
at the bottom of the list there is Darryl that is constantly annoyed by Michael, Angela that only cares about her cats and Stanely being the office grump.
Kelly is in a constant change of mood and when in season two Ryan appears she tends to be more happy.

![image info](/images/firsttwo.png)

Season three, four and five keeps Stanley's at the bottom of the list because he does not like to find himself in constant meetings and only loves Pretzel Days.
Moreover, we can observe Michael being constantly in top three, meaning that whenever there is a problematic situation in the office he always likes to 
take things positively and develops a multitude of characters to break the created tension in the office. From being neutral Dwight drops a few positions back
due to the fact of taking things too serious and being prancked by Jim.

![image info](/images/345.png)

Season five and six gives Toby a higher sentiment score due to the fact that he is about to leave for Costa Rica and also was invited to participate in the
Scranton Strangler court case as a jury. Because Dunder Mifflin was sold to another company, new characters start to appear like Gabe, Erin, Pete and Clark
that have a rather positive score due to the fact that they met their new colleagues and tend to get along with everyone. At the bottom of the list Meredith,
Stanley, Darryl and Angela are not pleased with the new changes. 

![image info](/images/56.PNG)

Season seven is when Michael leaves Dunder Mifflin, this being the main reason why he did not make it into top 5. On the other hand Karen has the biggest
happiness score due to the fact of being pregnant. New characters are introduced such as Robert California, whit a big sentiment score because of his role as
a CEO of Dunder Mifflin. At the bottom of the list there are the usual names always grumpy and self centered(Angela) and Nelie who has filmed in only one series
of that season but still making a bad impression from the begining. 

![image info](/images/7.PNG)

After Michael leaves Andy is appointed manager and his dream to be promoted is fulfilled, thus, receiving a high sentiment score. Nellie from being last made it into top 
ten due to the fact of being promoted to a higher position and at the characters with the lowest sentiment score being the usual grumpy faces of Angela, 
Stanley, Toby and Meredith. 
Season nine has somewhat two biast sentiment scores because both Roy and Michael appear only in one of the series, and in the middle there is Dwight. One can
say that was the most Dwight has achieved during the sitcom, thus, he and Angela have a higher sentiment score than before.

![image info](/images/89.PNG)


### **LabMT method**
 
The diagram below represents 10 happiest and saddest characters out of the main one's according to LabMT method. We can definetely state that Michael is the most positive
of them all, being the regional manager that can not affors to have a sad influence on the office. The diagram is quite accurate because Toby is the
saddest character, being constantly bullied by Michael for his lack of adventure and monotonous lifestyle. Jim and Pam are in the top 10 happiest characters
because of their relationship development throughtout the seasons, but did not make the top 5 as like in any other relation sad moments are there as well.


#### **Characters based on sentiment score:**

![image info](/images/sentiment_score.png)


#### **Histogram of all characters associated transcripts-sentiments using the LabMT method**

From the below histogram, we can see the variation on the character sentiments. It represents the number of characters that share the same sentiment score according to the LabMT method. The sentiment score does not fluctuate much which means that the characters do not have a significant change of sentiment, but rather all of them share more or less the same temperament.



![image info](/images/histogramLABMT.png)



### **Vader method**

According to the Vader method for calculating sentiment analysis based on each character transcript, Roy has the biggest sentiment score. Why would not he,
his only moment of sadness being his breack-up with Pam. After that he became a successful businessman living the dream and making everyone else envy him.
However his score is biast. due to the fact that he did not appear after the season five and appeared only once in season nine as a successful character, 
receiving an overall sentiment score higher than anyone.
Michael in the second place stays as the most consistent character according to both methods. Being the regional manager Michael had to stay positive 
in order not to bring sad thoughts into the office that will demotivate everyone else. Jim and Pam have always been good to everyone from the office, besides that
Pam was a receptionist and afterthat became the office administrator, meaning that she needed to stay positive while interacting with everyone.
Starting with dwight that has a reathe sarcastic sense of humour which is often interpreted as negative, characters like Toby, Stanley, Angela
and Jan tend to have a lower sentiment score due to the fact that they are mean to everyone else that does not like their lifestyle. Stanley and Jan were always mean to 
Michael because of his nature and lack of responsibility which denotes clearly their low score of happiness. Toby being the HR employee was always neutral
suffering from his divorce while Meredith treated her sadness with alcohol. 


#### **Characters based on sentiment score:**

![image info](/images/sentiment_score1.png)


#### **Histogram of all characters associated transcripts-sentiments using the Vader method**

As the previous histogram shows, there is no big decay between the polarity scores of the characters. Most of them are positive and only a few people have some negative thougths that can be interpreted as neutral. It means that the show is rather positive to watch and would only give you good vibes. 


![image info](/images/polarity.png)
