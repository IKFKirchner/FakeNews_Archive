# The persistence of false narratives: A small Twitter archive

This project was part of a larger project at the Maryland Institute for Technology in the Humanities (MITH) at the University of Maryland. It aimed at creating small Twitter archives for further analysis and for the construction of data stories.



## What will you find in this repository?





## Why did I collect this data?

On Monday, April 23, 2018, 10 pedestrians were attacked and killed by the driver of a rental van in Toronto, Canada. In the first hours of confusion and panic, twitter was the main media platform where pictures of the incident, eyewitness reports, and reports on the aftermath as well as the following arrest of the driver accrued to provide a first overview of the situation. However, the hunger for new information amidst the initial disorientation lends itself as a breeding ground for speculation, false allegations, and racial biases that reinforce the prejudice of terrorist attacks being predominantly committed by Muslims. Accordingly, early tweets confidently declared the driver to be Muslim and thereby fed into a popular narrative discriminating against Muslims and labeling Islam as a particularly violent religion. 


Quickly, an unstoppable dynamic set off that wove the initial factual reports into a larger political discourse on the refugee crisis and Trudeau’s presidency. ![picture](https://github.com/IKFKirchner/datastory/blob/master/MITH%20Tweet%206.png) Unsurprisingly, Alt-right figures such as Gavin McInnes and Paul Joseph Watson![picture](https://github.com/IKFKirchner/datastory/blob/master/MITH%20Tweet%205.png) also seized the opportunity to further provoke with racist comments. This toxic debate was legitimized by journalists who provided the seemingly reliable information that the driver was indeed Middle Eastern (Natasha Fatah works as a host for CBC News Network). ![picture](https://github.com/IKFKirchner/datastory/blob/master/MITH%20Tweet%203.png) Although this information was soon repudiated as the driver turned out to be a young misogynist Christian of Armenian origins, the narrative of a Middle Eastern driver and ‘yet another’ Islamic terrorist attack lingered on for hours and even days. 


In order to show the evolution of this toxic dynamic and the predominance of popular tweets over actually accurate tweets, I have collected all tweets in response to the attack in Toronto. 



## How did I collect this data?

This data was collected using TWARC (https://github.com/DocNow/twarc). Twarc is a command line tool and Python library for collecting and archiving Twitter JSON data via the Twitter API. It has separate commands (twarc and twarc2) for working with the older v1.1 API and the newer v2 API and Academic Access (respectively).

The archived tweets cover three days from April 23, 2018 (the day of the attack) to April 25, 2018.

I first identified the main hashtags that were used in tweeting about the attack. After skimming the vast data on Twitter and using Google search, I singled out #toronto and #yongeandfinch (street names of where the attack happened). Although #toronto includes numerous tweets that are not concerned with the attack at all, ignoring this hashtag would have meant a great loss of data. Instead, I chose to accept the ‘noise’ and factor it into my analysis. 

In addition to the TWARC search, I searched Google for screenshots of tweets.

Here is the link to my [data](https://github.com/IKFKirchner/datastory/blob/master/data/tweets.csv)



## What can the data tell us?


The predominant language in which the tweets were written is English, which is hardly surprising given that the attack took place in Toronto. ![chart](https://github.com/IKFKirchner/datastory/blob/master/chart.png)



A more interesting analysis traces the most commonly used words as the debate on Twitter unfolds. For this, I divide the data of the first day for every half hour to show the quickly changing dynamic. For the following days, I divide by 2 hours. For each set, I then create a word cloud on ‘Voyant Tools’ using a stop-word list that would exclude common yet irrelevant words. This kind of analysis can be best described as narrating change over time, although I hoped to focus on the persistence of the narrative rather than on the changes once the first false report on a Middle Eastern driver was released. 


A sentiment analysis does not prove as fruitful since the overall sentiment is very likely to be negative. Some of the tweets are of course of an apologetic nature and defend Muslims instead of labeling them as terrorists or pointing out the falsity of the allegation. However, apologetic tweets answer to an already dominant narrative and the fact that Islam and Muslims are mentioned in this context at all, already reveals the overall association of Islam with attacks of such nature. I therefore don't differentiate between accusatory and apologetic tweets, but see them both equally as evidence of the persistence of the narrative.


There are limits to these analyses: Often, the sentiment or the actual message is not actually spelled out but only hinted at. The following tweet does not mention any of the keywords (Islam(ic), Islamist, Muslim, Middle East(ern), Arab(ic), refugee, etc.), but rather uses emojis to point at Muslims. ![picture](https://github.com/IKFKirchner/datastory/blob/master/MITH%20Tweet%201.png) Furthermore, sarcasm is often used in such tweets in order to echo and simultaneously delegitimize political slogans (“refugees welcome” + hateful emoji). This is hard to differentiate computationally. However, just the mentioning of the keyword ‘refugee’ already illustrates that the false narrative is still carrying on.


In fact, this persistence of false narratives is advocated by Twitter’s design: By ranking according to popularity, Twitter grants legitimacy to false information even after it has been repudiated and potentially even favors it over correcting reports that have not gained the same popularity yet. Earlier tweets announcing a Middle Eastern driver were therefore displayed disproportionally often, although they had long been falsified. 


Without a doubt, at least some users eventually chose to delete their tweets after they had been confronted with more accurate information. However, my data set may contain and preserve tweets that the original authors no longer endorse and may want to delete. I have harvested this data without consent and can analyze and present it without announcing it to the respective author. Especially since a tweet contains far more data than merely the actual message itself and sometimes even reveals the exact location from where a user might be tweeting, being able to access and publish this kind of data is very problematic from an ethical perspective. I will therefore choose to delete my files as soon as this exercise has been graded, although I will have lost control over the distribution of my data as well as soon as I have published it. The fact that I was able to easily find tweets of April 23rd on Google although Twitter had already restricted my access, demonstrates this loss of control very well.










