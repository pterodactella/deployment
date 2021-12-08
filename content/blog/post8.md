---
layout: post
title: "Communities"
date: 2021-12-02T13:26:38+01:00
description: ""
featured_image: "/images/group.jpg"
draft: false
---
 Based on the network obtained using the Dunderpedia character's pages, we found communities by branch and compute their associated TF-IDF. Using the *Louvian* method, we managed to identify 9 communities with the modularity of the Louvain based partition equal to 0.341.

 To further examine the communities, we will plot the distribution of the community sizes. Each community is identified with the TOP 3 characters from each community (based on their degree in the network). 


 {{< load-plotly >}}
{{< plotly json="/01-communities.json" height="450px" >}}
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
Next, we look at the communities, and we create TF-IDF based rankings of words in each community. To calculate TF-IDF we can reuse the functions defined in the previous part. The only difference right now is the way we compute the *tf* for every word. Previously *tf* represented the number of occurences of a word in a document. This time this number is also divided by the total number of words in the respective document. In other words, *tf* this time is normalized.
The idea behind computing the *tf-idf* for every word is having a set of words across all the dialogs belonging to the community. Then, one can loop through the unique words, check their number of occurrences in each file, and increment it if necessary. At the end, by maintaining the unique set of tokens per communities, we are guaranteed to have the correct frequency number for each word, in other words - its number of occurences in each file for every character in the community.

 {{< load-plotly >}}
{{< plotly json="/02-LabMT-characters.json" height="450px" >}}
