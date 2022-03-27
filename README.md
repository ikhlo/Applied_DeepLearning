# Applied DeepLearning : GraphRecSys

## Context

Our project is to build a recomender system for scientific publications based on graphs. So far, we created our dataset (with a subset of dblp : https://www.aminer.org/citation) to a bipartite graph. 
A first step was to compute the embeddings of both abstratcts and title using a pretrained model fine tuned on scientific papers. To build recommendations, we first tested a simple cosine similarity, dot product and euclidean distance between one author embedding (which is the mean of all the papers abstracts and title embeddings he wrote) and all papers which he don't interact with to find the paper with the highest score. 
Another approach we have tested is implementing GAE/VGAE model to perform link prediction and then recommend new papers to authors.

## Authors

This project have been done in collaboration by [Aurélien Renault](https://github.com/aurelien-renault), [César Leblanc](https://github.com/CesarLeblanc), [Ikhlass Yaya-Oyé](https://github.com/ikhlo) and [Victor Clermont](https://github.com/VicCler).

## References

* [Dynamic Graph Neural Networks for Sequential Recommendation](https://arxiv.org/pdf/2104.07368.pdf)
*  [Graph Neural Networks in Recommender Systems: A Survey](https://arxiv.org/pdf/2011.02260.pdf)
