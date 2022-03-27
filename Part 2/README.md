# krikey-data-challenge


## Analysis details:

### Methodology:

Goal: Increase user engagement

User journey: There are two major sections

Success metric for engagement: 

```
Total watch time

Total watch time = Total number of videos watched x % video watched x average video length

Total number of videos watched could be either from For you/recent page or from Explore Page. For explore page:

Total number of videos watched = CTRxVideos Viewed
```


Bins for completion rate
```
0: 1.45%-23.3%
1: 23.3%-44.5%
2: 44.5%-66.1%
3: 66.1%-88.2%
4: 88.2%-100%
```

Distribution of number of videos and completion rate:

![Alt text](../data/cr_nr.png?raw=true "Title")

Correlation with completion rate:

![Alt text](../data/comp_wt.png?raw=true "Title")

Users with higher completion rate have a higher average watch time

Hypothesis: Higher completion rate results in higher engagement/watch time

How can we increase Engagement?

1. Showing the relevant content to users => increasing CTR
2. More personalized content => better completion rate


## Product recommendations:

Experiment around watch time suggestions for creators
1. Min and max limit would restrict users from creating new videos
2. Start with UI changes like showing "Recommended video length", Trimming videos
3. Once we experiment and get more data, we can improve this with personalized video length recommendations at user level

## Next steps:

Post onboarding, a customer has two ways to use the app:
1. Games
2. Watch/Create Videos

Since primary goal is growth and retention:

1. Retention/Engagement features for gamers - like Daily bonus, Quests
2. Help users to find new content. In search - show popular categories, trending etc
3. Adoption - Since the primary audience for the app is India, regional languages will help in targeting a larger audience