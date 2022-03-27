# krikey-data-challenge


## Analysis details:

### Methodology:

Goal that I have taken: To increase user engagement

User journey: There are two primary ways as to how a user can engage with the app - videos and games. For this analysis, I have focused on engagement through videos based on the data that has been provided.

Success metric that I have considered for engagement: 

```
Total watch time
Total watch time = Number of users x Number of videos watched/user x % video watched x  avg video length
```

Based on the data, I am going after 2 factors from the above equation - 

1. % completion/video
2. Avg videos watched/user


#### 1. For % completion/video, below is my analysis 

Bins for completion rate
```
0: 1.45%-23.3%
1: 23.3%-44.5%
2: 44.5%-66.1%
3: 66.1%-88.2%
4: 88.2%-100%
```

Potential impact:

Distribution of number of videos and completion rate:

![Alt text](../data/cr_nr.png?raw=true "Title")

~40% of the videos have less than 85% completion/video

Correlation of watch time with completion rate:

![Alt text](../data/comp_wt.png?raw=true "Title")

Users with higher completion rate have a higher average watch time

Hypothesis: Higher completion rate results in higher engagement/watch time

My recommendation on how we can increase the completion rate:

1. Showing more relevant/personalized content to users:
	i. based on user item interaction/collaborative filtering<br />
	ii. based on user's preferences like length of the video, feed type etc<br />

#### 2. Total number of videos watched could be either from For you/recent page or from Explore Page. For explore page:
```
Total number of videos watched = CTRxVideos Viewed
```
For increasing the watch time, we have to first target increasing the CTR.

My recommendation on how we can increase the CTR:

i. Experiment with features like live tiles(Hypothesis - Live tiles have better CTR)<br />
ii. Experiment with order of tiles in different sections. For example, videos that have a higher CTR can be shown ahead of other videos<br />
iii. We can either use multi-armed bandits or once we get more data from further experimentation, we can decide on the subsequent actions<br />

## Next steps:

Post onboarding, a customer has two ways to use the app:
1. Games
2. Watch/Create Videos

Since primary goal is growth and retention:

1. Retention/Engagement features for gamers - like Daily bonus, Quests
2. Help users to find new content. In search - show popular categories, trending etc
3. Adoption - Since the primary audience for the app is India, regional languages will help in targeting a larger audience