### Multi-armed recommender system bandit ensembles


## Resumen
In this paper the authors propose a new way to produce ensembles. Rather than algorithms being tested on a single non-interactive run that doesn't account for the performance changes as runtime conditions evolve, they propose a cyclic process that consider recommendation algorithms as arms and ensembles as bandits that selects an arm at each step to produce the next round of recommendations.

Previous work on ensembles run recommendations only once and the few works that seek to improve ensembles dynamically don't scale very well. They propose to adapt a multi bandit approach for building recommender system ensembles. They consider the context as the target user to whom a recommendation is delivered, the arms are the recommendation algorithms that are combined in the ensemble. The reward is 1 if the user is pleased with the recommendation 0 otherwise. Finally, arms are updated after each individual recommendation or after a batch. They use  ε-greedy and Thompson sampling to test their results.

They use the movie lense dataset and binarize the ratings (1-3 are mapped as 0 and 4-5 mapped as 1). They use knn, matrix factorization and most popular algorithm for the ensemble.

Their results show that their approach is significantly better than the algorithms alone and better than a non-bandit ensemble.

## Crítica

They could've tested their results with more than 3 algorithms to show in a more robust way their approach and scalability. Although they mention that their approach require less computational cost they don't show it in a clear way through testing.

It is good how their method always keeps the 3 algorithms as options, this way algorithms that have a very strong cold start could get the chance to be chosen as they improve their recommendations.

They show in a clear manner how non dynamic ensembles can fall in some unwanted behavior as it suffers from feedback loops and overfitting.
