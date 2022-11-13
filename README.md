# Koala-Sightings-and-Tweets
This analysis is part of my personal assessment item for IAB303 Data analytics for Business Insights at QUT.
Using the QDAVI analysis cycle (Question analysis - Data - Analysis - Visualising - Insights), I was able to gain insights on Koala sightings across Brisbane. 
The client (unit tutors) also tasked us to determine the feasibility of promoting a koala tour with social media influencers on Twitter. Through the twitter tweets analysis on the hashtag #koala, I was also be to identify potential competitors based on their handle name.

##Dataset
- Koala sightings around Brisbane, QLD was retrieved from [Atlas of Living Australia](https://biocache.ala.org.au/occurrences/61c78472-0613-491d-a0ea-6c0528d7bf7f)
- Twitter tweets dataset retrieved using the Twitter API (limited to 100 tweets per instance)

##Libraries
- Folium: this library was utilisedin to easily visualisze data on an interactive leaflet map with markers indicating positions on spots of interests

##Conclusions
**Sightings analysis**
- Based on the visualization of koala occurences from 2020 to the present above, it is clear that koalas can be found reliably around Brisbane to support a koala spotting tour. Areas that have a high rate of koala occurences that prove to be reliable locations for koala tours include:
  - Toohey Area
    - Toohey Forest-Mayne Estate
    - Ring Road - especially dense occurence of koalas, most suitable location
    - Toohey Forest Conservation Park
    - Toohey Forest (including sections on both sides of the South East Busway)
    - Wellers Hill
  - Whites Hill Reserve
    - Whites Hill
    - Octantis Street Park
- Toohey Area is recommended over Whites Hill Reserve since the Toohey Area has a much higher rate of reported occurences.
  - Toohey has both a higher occurence rate and more condensed than Whites Hill
    - Whites Hill occurences are not a lot but its not too few, the problem is that they are spread out, making it inefficient to operate tours
    - Whereas Toohey Area occurences are much higher and focused in specific spots, making tour operations efficient and possible
  - Proving the area to be a reliable location for koala tours
- Low occurence rate areas such as Tones Road Park and Belmont Bushland Reserve have very few reported human observations of koalas, making them unreliable to support a tour in those areas.
- Since Cleveland & Redland Bay are also considered part of the Brisbane Metropolitan area, just 22km South-East to Brisbane, the business can also consider the option of expanding tour operations here
  - Specifically:
  - Wellington Point
  - GJ Walter Park
  - Nandeebie Park
  - Henry Ziegenfusz Park 
- In addition, since all these occurences are from 2020-present, the occurence are as up-to-date as possible, making them reliable sources of information to support tour locations

**Twitter Question**
- Since Twitter API is limited to retrieving the most recent 100 tweets and only tweets from the past 7 days. The insight will be generalized to provide insight and reasons to support the reason why the 3 users with the highest follower count should be selected for advertisement and how they were found.
- It is recommended for the 3 Twitter accounts that have been analysed, identified and visualized above to be potential promoters for the business. With a higher amount of of followers, promoters can influence more people and reach a wider customer base, allowing the tour to reach more audiences.
- The 3 potential promoters were found based on the condition that:
- Twitter accounts were filtered to have a minimum of 3000 followers
- To be considered influential on social media, sources have reported the minimum follower count to be 3000
- The filtered data on tweets are then sorted based on Follower count in descending order, duplicates are then removed to find the 3 most followed accounts that tweeted on #koala
- 3 most followed accounts have been selected as the number three is a comprehensive number to select the 3 most followed influencers that enables the business to identify a variety of different promoters and select from them
With the analysis, the business is also able to identify potential competitors in the market based on the Twitter accounts ID name and their account description if they are a zoo/wild life tour business based on their Twitter ID and user description in the output above in Analysis

**Limitations**
- Limitations of the Twitter Analysis:
  - Twitter API is limited to pulling a maximum of 100 tweets per extraction
  - 100 tweets is not a substantial number of data to support justifcations and recommendations
  - Due to the limited tweet extraction, it doesnt give a full understanding of the use of the #koala hashtag 
  - Tweets are only from the most recent 7 days
  - Therefore, tweets from more than 7 days before the execution of this code is unable to be retrieved
  - More potential promoters/competitors might not have made a tweet in the most recent 7 days, hence, they could not be identified in some analysis depending on the time of code execution
  - There are alot of Retweets in the data and there are many data where they are retweets of 1 particular tweet
  - However, RTs are still kept in the analysis since RTs are ways that users can quickly share a tweet that they like and additionally, if they want to, add comments to it. This shows that user has interest in #koala.

##Analysis Notebook
- It is suggested to view the notebook using [THIS LINK](https://nbviewer.org/github/marcusNGD/Koala-Sightings-and-Tweets/blob/main/Marcus_Koala_Dataset.ipynb) as GitHub only displays a preview of the notebook and is unable to load the mapping component.
