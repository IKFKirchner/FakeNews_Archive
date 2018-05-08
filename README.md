# The persistene of false narratives

## Why did I collect this data?


On Monday, April 23rd, 10 pedestrians were attacked and killed by the driver of a rental van in Toronto, Canada. In the first hours of confusion and panic, twitter was the main media platform where pictures of the incident, eye witness reports, and reports on the aftermath as well as the following arrest of the driver accrued to provide a first overview over the situation. However, the hunger for new information amidst the initial disorientation lend itself as a breeding ground for speculation, false allegations and racial biases that reinforced the prejudice of terrorist attacks being predominantly committed by Muslims. Accordingly, early tweets confidently declared the driver to be Muslim and thereby fed into a popular narrative discriminating Muslims and labeling Islam as a particularly violent religion. 


Quickly, an unstoppable dynamic set off that wove the initial factual reports into a larger political discourse on the refugee crisis (see below) and Trudeau’s presidency. ![picture](https://github.com/IKFKirchner/datastory/blob/master/MITH%20Tweet%206.png) Unsurprisingly, Alt-right figures such as Gavin McInnes and Paul Joseph Watson (pic5) also seized the opportunity to further provoke with racist comments. This toxic debate was legitimized by journalists that provided the seemingly reliable information that the driver was indeed Middle Eastern (pic3). Although this information was soon repudiated as the driver turned out to be a young misogynist Christian of Armenian origins, the narrative of a Middle Eastern driver and ‘yet another’ Islamic terrorist attack lingered on for hours and even days. 


In order to show the evolution of this toxic dynamic and the predominance of popular tweets over actually accurate tweets, I have collected all tweets in response to the attack in Toronto. 



## How did I collect this data?


First, I had to identify the main hashtags that were used in tweeting about the attack. After skimming the vast data on twitter and using the google search, I singled out #toronto and #yongeandfinch (street names of where the attack happened). Although #toronto includes numerous tweets that are not concerned with the attack at all, ignoring this hashtag would have meant a great loss of data. Instead, I chose to accept the ‘noise’ and factor it into my analysis. 


I searched ‘#toronto OR #yongeandfinch since:2018-04-23’ on TWARC but got no reaction from cloud shell and could not download any data. I repeated my search and checked my command multiple times, eventually giving up because cloud shell would not react and had seemingly crashed every time. Trouble-shooting with Purdom quickly revealed the problem: My impatience has misled me to believe nothing was happening when, in fact, the search was still ongoing each time and had simply not come to an end yet. However, the data that my search would harvest, is so big, that it took too long, and we forced a premature end to the search. When I repeated the search last Saturday (May 5th) in order to complete the search, I had to find out that Twitter did not allow me to search prior to Wednesday, April 25th and the most important chunk of my data was lost. Unaware of that restriction (I was convinced that we could go back up to 14 days), I was still left with a lot of data. 


Also, I searched google for screenshots of tweets that could illustrate my point and easily found some examples from April 23rd that I included here. 


Here is the link to my [data](https://github.com/IKFKirchner/datastory/blob/master/data/tweets.csv)



## What can the data tell us?


The predominant language in which the tweets were written is English, which is hardly surprising given that the attack took place in Toronto. ![chart](https://github.com/IKFKirchner/datastory/blob/master/chart.png)



A more interesting analysis could trace the most commonly used words as the debate on Twitter unfolds. For this, I would divide the data of the first day for every half hour to show the quickly changing dynamic. For the following days, I would divide by 2 hours. For each set, I would then create a word cloud on ‘Voyant Tools’ using a ‘stop word list’ that would exclude common yet irrelevant words. This kind of analysis can be best described as narrating change over time, although I hoped to focus on the persistence of the narrative rather than the on the changes once the first false report on a Middle Eastern driver was released. 


A sentiment analysis may not prove as fruitful since the overall sentiment is very likely to be negative. Some of the tweets are of course of an apologetic nature and defend Muslims instead of labeling them as terrorists. However, apologetic tweets answer to an already dominant narrative and the fact that Islam and Muslims are mentioned in this context at all, already reveals the overall association of Islam with attacks of such nature.


There are also limits to both analyses: Often, the sentiment or the actual message is not actually spelled out but only hinted at. The following tweet does not mention any of the key words (Islam(ic), Islamist, Muslim, Middle East(ern), Arab(ic), refugee etc.), but rather uses emojis to point at Muslims. Furthermore, sarcasm is often used in such tweets in order to echo and simultaneously delegitimize political slogans (“refugees welcome” + hateful emoji). This is hard to differentiate computationally. However, just the mentioning of the key word ‘refugee’ already illustrates that the false narrative is still carrying on.


In fact, this persistence of false narratives is advocated by Twitter’s design: By ranking according to popularity, Twitter grants legitimacy to false information even after it has been repudiated and potentially even favors it over correcting reports that have not gained the same popularity yet. Earlier tweets announcing a Middle Eastern driver were therefore displayed disproportionally often, although they had long been falsified. 


Without a doubt, at least some users eventually chose to delete their tweets after they had been confronted with more accurate information. However, my data set may contain and preserve tweets that the original authors no longer endorse and may want to delete. I have harvested this data without consent and can analyze and present it without announcing it to the respective author. Especially since a tweet contains far more data than merely the actual message itself and sometimes even reveals the exact location from there a user might be tweeting, being able to access and publish this kind of data is very problematic from an ethical perspective. I will therefore choose to delete my files as soon as this exercise has been graded, although I will have lost control over the distribution of my data as well as soon as I have once published it. The fact that I was able to easily find tweets of April 23rd on Google although Twitter had already restricted my access, demonstrates this loss of control very well.










