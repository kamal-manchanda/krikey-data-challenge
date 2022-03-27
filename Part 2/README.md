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

~40% of the videos have less than 88% avg completion/video

Correlation of watch time with completion rate:

![Alt text](../data/comp_wt.png?raw=true "Title")

Users with higher completion rate have a higher average watch time

Hypothesis: Higher completion rate results in higher engagement/watch time

My recommendation on how we can increase the completion rate:

1. Showing more relevant/personalized content to users:<br />
	i. based on user item interaction/collaborative filtering<br />
	ii. based on user's preferences like length of the video, feed type etc<br />
	
Limitations:<br />
1. Since the metric we are trying to improve here is avg video completion, we should make sure other metric like avg video length are not taking a hit, and it is important that total watch time should go up.

#### 2. Total number of videos watched could be either from For you/recent page or from Explore Page. For explore page:
```
Total number of videos watched = CTRxVideos Viewed
```
For increasing the watch time, we have to first target increasing the CTR.

My recommendation on how we can increase the CTR:

i. Experiment with features like live tiles(Hypothesis - Live tiles have better CTR)<br />
ii. Experiment with order of tiles in different sections. For example, videos that have a higher CTR can be shown ahead of other videos<br />
iii. We can either use multi-armed bandits or once we get more data from further experimentation, we can decide on the subsequent actions<br />

Limitations:<br />
1. Since the metric we are trying to improve here is CTR, we should make sure other metrics like %video completion are not taking a hit, and it is important that total watch time should go up.

Other correlations checked(EDA/visualizations in the jupyter notebook):<br />
a) Favourite feed type vs watch time<br />
b) Class/User type vs watch time<br />
c) Avg video length vs watch time<br />
d) game id vs watch time<br />
e) country vs watch time<br />
f) os/client version vs watch time<br />
g) is ar?/client version vs watch time<br />

## Next steps:

Post onboarding, a customer has two ways to use the app:
1. Games
2. Watch/Create Videos

Looking at Krikey's goal of growth and retention, my additional recommendations would be to do an analysis around these factors as well:

1. Retention/Engagement features for gamers - like Daily bonus, Quests
2. Help users to find new content. In search - show popular categories, trending etc
3. Adoption - Since the primary audience for the app is India, regional languages will help in targeting a larger audience