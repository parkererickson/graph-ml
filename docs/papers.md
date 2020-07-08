# Graph Machine Learning Papers

## [Semi-Supervised Classification with Graph Convolutional Neural Networks](https://arxiv.org/abs/1609.02907)
Kipf & Welling (2017)

**Parker's Take:** A great paper to dive head first into the world of graph machine learning with. Introduces the concept of a convolution on a graph, and produced state-of-the-art results at the time of publish. Personally, I have used a GCN to find fraud and predict IPOs of companies.

## [Graph Attention Networks](https://arxiv.org/abs/1710.10903)
Petar Veličković, Guillem Cucurull, Arantxa Casanova, Adriana Romero, Pietro Liò, Yoshua Bengio (2018)

**Parker's Take:** While I still don't quite get the math, the algorithm described in this paper certainly an interesting one. Using an attention mechanism allows the algorithm to be more efficient/parallelizable when compared to things like a GCN. The model is also able to classify entire graphs, and can generalize to an unseen graph.

## [Graph Convolutional Neural Networks for Web-Scale Recommender Systems](https://arxiv.org/abs/1806.01973)
Rex Ying, Ruining He, Kaifeng Chen, Pong Eksombatchai, William L. Hamilton, Jure Leskovec (2018)

**Parker's Take:** One of the issues with applying Kipf & Welling's GCN in the real world is that it does not scale well. This paper, written by Pinterest of all places, proposes a new framework for at-scale GCNs. They apply their algorithm to produce embeddings of each item in their 3 billion vertex graph in order for better recommendations. For graph ML at scale, this is an essential read.

## [Variational Graph Auto-Encoders](https://arxiv.org/abs/1611.07308)
Kipf & Welling (2016)

**Parker's Take:** I think that VAEs are very cool. Applying them to graphs is even cooler. Allowing you to compress a highly-dimensional/non-dimensional structure into a relatively small vector astounds me. State-of-the-art results at link prediction because of it is even cooler.

## [Modeling Relational Data with Graph Convolutional Neural Networks](https://arxiv.org/abs/1703.06103)
Michael Schlichtkrull, Thomas N. Kipf, Peter Bloem, Rianne van den Berg, Ivan Titov, Max Welling (2017)

**Parker's Take:** Another paper with Kipf & Welling involved. This time, they expand upon the GCN, describing a method that allows multiple different types of edges and vertices to be in the graph. They then use this to perform edge prediction and vertex classification. If you are using a knowledge graph, this is a must-read.

## [node2vec: Scalable Feature Learning for Networks](https://arxiv.org/abs/1607.00653)
Aditya Grover, Jure Leskovec (2016)

**Parker's Take:** Great way to create embeddings for your vertices. Think about this as word2vec, but instead of words in a sentence, you are creating "sentences" of vertices through the randomly walking through them. The parameters **p** and **q** determine how the random walks are dispersed (focusing on local neighborhood vs. far reaches of graph), don't forget to tune them. This is a really easy method to generalize to knowledge graph content and scale.