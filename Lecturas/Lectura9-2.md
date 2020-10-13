### Carousel Personalization in Music Streaming Apps with Contextual Bandits

## Resumen
In this paper the authors propose a to model the carousel used in music streaming apps as a multi-armed bandit with multiple plays learning problem.

Multi armed bandits with multiple players involve K entities called arms and a forecaster whos objective is to choose each round the arms that maximizes the reward. To do this the forecaster must explore all arms and over time decide which give the better results.

The problem they face is that running N (one for each user) require a long time to train and converge and it's not suitable. They tackle this problem by having a cluster of users with similar test this reduces the bandits as they only need one per cluster. The second approach they propose is that each user has a D dimensional attribute vector and bandits need to learn the optimal weights of this D dimensional array.

A second problem they have to adress is the fact that there is no certain way of knowing which card the users saw so they can't reward it with a 0 is it is not clicked. They solve this by inspiring in the cascade model.

Their experiments consists of 862 playlists that 12 have to be picked for the carousel and 3 are shown at a time. They first simulate their model on an offline experiment that runs on a simulated environment and with data they released for the public. Later they validate their findings with an A/B test ran on Deezer app.

Finally they show and explain their results. In summary semi-personalized outperform fully personalized recommenders. They explain how delayed batch feedback may have caused some issues with some of the polices. Then, they show how cascade models outperform non-cascade and how identifying this phenomena can be very helpful.
## Crítica

I like the fact that they release open data and an open-source environment to simulate similar carousel personalization problems. This creates transparency and lets the readers not only see the authors' results but also test them by themselves.

I like the fact that they tested a large set of policies and show clearly in a graph which works better, they also explain it in a very clear manner some of the phenomena that occurs in the graph and why this might happen.

They show how some of their choices affect the results like how delay batch feedback may have affected some models more than others, or how cascade outperform non-cascade. This makes their work a lot more convincing.

Finally, they lay the ground for a lot of future work proposing new ideas that could be studied and creating a platform to aid on this.
