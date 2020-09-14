## Combining Predictions for Accurate Recommender Systems

### Resumen

In this paper they use top of the art collaborative filtering recommender algorithms and they show that lineally combining them yields better accuracy results. They try to implement a method that outperforms linear blending. They use the Netflix prize dataset to test their findings.

Then they give a general idea of the most commonly used algorithms such as knn (user-user and item-item), SVD, AFM, RBM, etc.

When training different CF models they do it in a residual way, this means that the first model is trained on raw data then each subsequent model is trained on the errors of the previous models. They then list all algorithms used and a description on how they were implemented.

When blending the predictions they used a supervised machine learning method that optimizes the RMSE on test set. They use a probe dataset that they divide in p train and p test due to the huge numbers of samples to train and test this blending algorithm.

They then mention different blending algorithms and how they implemented them as well as giving a general overview of this blending algorithms.

Finally, they list their results and findings showing tables of each algorithm and the results obtained varying different hyperparameters.

### crítica

I think it is a good idea to give an overview of the most commonly used algorithms and also list references to a more detailed explanation of them. Also it is a very good idea to show a table that summarizes each algorithms showing RMSE, training time, prediction time and memory complexity to get a better understanding of the pros and cons of each algorithm.

It is also a good idea to show a table of the different CF algorithms used and a description no how they were implemented for future replication of the paper.

They mention different things they tried even if they were not successful which is a good thing for future readers of the paper either to test them out themselves or to not lose time doing so.

They give a link to the source code and dataset used which again makes it a lot easier to replicate results and improve on them.

In conclusion I think this is a well written paper that shows experimental results on the Netflix dataset, it shows in a clear way how combining predictions is a clear advantage in recommender systems and they propose several ways this could be achieved with diverse results, the only thing that they could improve is at the end listing things that can improve with further experimentation.
