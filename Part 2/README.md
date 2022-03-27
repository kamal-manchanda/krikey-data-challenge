# krikey-data-challenge


## Analysis details:

### Methodology:

Goal: Increase user engagement

User journey: There are two major sections

Success metric for engagement: Total watch time

Correlation with completion rate:

![Alt text](../data/comp_wt.png?raw=true "Title")

Users with higher completion rate have a higher average watch time

Finding sweet spot for watch time/video:

Bins for watch time
```
0: 0.1-1.55
1: 1.55-2.91
2: 2.91-4.19
3: 3.91-5.55
4: 5.55-7
```

Hypothesis: Higher completion rate results in higher engagement/watch time

How can we increase completion rate?

1. Personalization - I have not explored this part in this project
2. Finding a sweet spot of video time



![Alt text](../data/watch_time.png?raw=true "Title")

Completion rate for different watch time bins:

![Alt text](../data/wt_cr.png?raw=true "Title")

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