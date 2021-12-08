---
layout: post
title: "Dunderpedia Basic Stats"
date: 2021-12-07T18:26:38+01:00
description: "A little backgroud on what was already discovered during part A"
featured_image: "/images/group.jpg"
draft: false
---
This blog post focuses on providing the full analysis performed during the first part of the project.

We start our Dunderpedia analysis by generating The Office network, which includes all the characters in the Office extracted from the Dunderpedia. 
The nodes in the network will be all the characters, and we will place an edge between nodes **A** and **B** if the Dunderpedia wiki page of node **A** links to the Dunderpedia Wiki page of node **B**. 

### Basic Statistics
We would like to get some insights into our network. For this, we perform simple network statistics and analysis:

{{< load-plotly >}}
{{< plotly json="/dunderpedia/04-nodes.json" height="250px"  >}}

{{< load-plotly >}}
{{< plotly json="/dunderpedia/05-links.json" height="250px"  >}}

{{< load-plotly >}}
{{< plotly json="/dunderpedia/06-top_in_degrees.json" height="250px"  >}}

The top connected character in The Office for the in-degrees is **Michael Scott**, with a 108 in-degree. Michael is the main character of The Office, and Regional Manager of the Scranton branch from season 1 to 7. Hence it makes sense that a lot of characters point to him as he is the main character and has relations to most of the other chraracters. 

{{< load-plotly >}}
{{< plotly json="/dunderpedia/07-top_out_degrees.json" height="250px"  >}}

The top connected character in The Office for the out-degrees is **Andy Bernard**, with a 33 out-degree. In the series, Andy Bernard tries to please everyone, so it makes sense that he is the one pointing to the most characters.


### Top 5 connected components
{{< load-plotly >}}
{{< plotly json="/dunderpedia/01-top_in_out_degree.json" height="850px"  >}}
\
\
\
\
\
\

The most connected characters as one can see from the in-degree graph are the top 5 main characters, according to our biased opinion as viewers. However, a verification will be done during this analysis. During the series almost everything evolves around them, is it a prank on Dwight from Jim, is it a relationship problem or shared happiness between Jim and Pam, or Andy who tries to be friends with everyone, and least but not last, Michael Scott, that keeps the group together and likes to pretend as a father to all of them.

Regarding the top connected characters for the out-degree, Michael is the regional manager and has connections not only with his office, but other branches as well as with the corporate. So it makes sense that he is the person that everyone links to and also him, being the one that links to other people. As well as Andy who's desire is to become the next branch manager. All the main characters are repeated besides Jim, who is not there for the job but for Pam. He does not like to gossip much or try to please everyone, his concerns are only about Pam.

#### The in- and out-degree distributions
We look further in the in and out degrees by computing the bin distributions:

{{< load-plotly >}}
{{< plotly json="/dunderpedia/02-degree_distributions.json" height="450px" >}}
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\

- The first thing that we can observe is that maximum out-degree is more than 3 times smaller than maximum in-degree, which could have also be seen in the previous question, when we examined the top nodes based on in- and out-degree, Michael and Andy. 

- In the in-degree plots it can be seen that there majority of nodes, nearly 100, have a degree of 0, and the degree ranges until 108. Hence, the distribution shows that a large number of characters point to a small number of characters. While in the out-degree plots, the degree distribution changes slower than the in-degree, and the degrees are more concentrated between 0 and 10, in comparison to the in-degre.

- Because of the nature of the network. In this network, the link is defined between two characters, **A** and **B**, if there exists a hyperlink in character's **A** page that link to **B**'s page. Popular characters will therefore be linked by a lot of other characters, which can accounts for highers in-degrees. Therefore, for less popular characters, will have links pointing to other characters, but very little links pointing to them, which can cause the large amout in-degrees close to 0.

- The out-degree might be limited by the page length and the fact that every characters includes a low number of hyperlinks in its page.

### Comparison between the degree distribution of the undirected graph to a random network with the same number of nodes and probability of connection p.


{{< load-plotly >}}
{{< plotly json="/dunderpedia/03-degree_distributions_random_network.json" height="450px" >}}
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\
\


From the above plot it can be see that the degree distribution of the random network is similar to a normal distribution, with the higher degrees in the middle values (from 5 to 9), with the mean in 7, the mean value of the degree. On the other hand, the Undirected graph there is only one high peak on the degree 0, and the degree count starts to decrease after. 



#### Visualization of the network
Bellow you can see how the network looks:

![image description](/images/network.png)



