## Deep Learning based Recommender System: A Survey and New Perspectives

### Resumen
In this paper authors review how deep learning can be applied to the area of recommendation systems. To do this they implement a survey which aims to provide a comprehensive summery on the research that is being made using deep learning for recommender systems, as well as identify open problems that are currently limiting deep learning.

Then, they summarize some of the key concepts used and lightly explain how some of the neural networks architectures work. They also explain why deep learning and neural networks might be useful in the area, as this type of networks are good to exploit inherited structures if they are present.

The first model they address is MLP, they use this architecture for collaborative filtering to model the 2 way interaction between users and items. They also use it as deep factorization machines this type of models are able to model the high-order feature interactions via deep neural network and low order interactions with factorization machine. They also propose a variation which models the explicit and implicit feature interactions.

Feature representation is another form in which they use MLP for recommendation. Wide & deep learning can solve both regression and classification problems. The wide component helps with memorization and the deep component catches the generalization.    

Recommendation with Deep Structured Semantic Model are widely used in information retrieval area and is supremely suitable for top-n recommendation. DSSM projects different entities into a common low-dimensional space, and computes their similarities with cosine function

Autoencoder based Collaborative Filtering can be found in 2 ways item-based AutoRec (I-AutoRec) and user-based AutoRec (U-AutoRec). In general, ) I-AutoRec performs better than U-AutoRec, which may be due to the higher variance of user partially observed vectors. CFN is an extension of AutoRec which makes it both more robust and also incorporates side information such as user profile.

Convolution Neural Networks are powerful in processing unstructured multimedia data with convolution and pool operations. Most of the CNNs based recommendation models utilize CNNs for feature extraction. CNNs can be used for feature representation learning from multiple sources such as image, text, audio, video, etc. CNN can also be used for text extraction, the main use is text review, extract item features for text information. CNNs are also used to extract features form video. Graph CNN for recommendation have showed promising results in very large scale web recommenders such as pinterest.  
### Crítica

The idea of making a survey on the research made on deep learning for recommender system is a very useful idea. They not only summarize the state of the art but list the challenges that are open to be solved to further improve this area. It is of tremendous value that this type of papers are done periodically as they motivate new people to get into the area in an easier way.

They do a good job summarizing key concepts and the basics of deep learning architectures as well as providing a reference for further reading. They also present strong arguments on why you should use deep learning for recommender systems. They also do a good job showing the primary arguments against DL and countering them.

They do a fine job summarizing the research and topics in easy to understand tables. This eases the job of the reader to link their preferences to the research this paper addresses.

When presenting the different uses of the architectures the authors do a very good job summarizing how it works, as well as showing references to variation on the models and the challenges this variation tackles.

They could've done a better job arguing why some architectures are better than others at a certain task, instead they present the various uses people have given this models not showing results or comparisons.
