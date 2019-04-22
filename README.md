# Determining Probabilities of Handwriting Formations using PGMs

Developing probabilistic graphical models (PGMs) to determine probabilities of observations which are described by several variables. We will work with handwriting patterns which are described by document examiners. They can be used to determine whether a particular handwriting sample is common (high probability) or rare (low probability) and which in turn can be useful to determine whether a sample was written by a certain individual. 

Tasks
1. Evaluate pairwise correlations and independences that exist in the data. Note that we can determine whether xi and xj are independent by testing if p(xi,xj) ≈ p(xi)p(xj), where the joint probability between a pair of variables can be determined from the tables as p(xi,xj) = p(xi|xj)p(xj). 
2. Construct a Bayesian network with the fewest number of edges that maximizes the likelihood. One approach is to use the results of the ﬁrst task and start drawing links between the most correlated pairs of variables. We can construct several Bayesian networks and obtain a score for each of them. One way of scoring is to determine the likelihood the network assigns to samples generated (using ancestral sampling). Note that the dataset changes for each model. Based on your best model, describe what a high probability th looks like (in words as well as in image form). Describe some low probability th as well.
3. Convert your best Bayesian network into a Markov network using moralization. Compare inferences using Bayesian network and the Markov network, in terms of computation time and accuracy.
4. Use the ”and” image dataset to construct a Bayesian network and evaluate the goodness score (likelihood of a dataset) of several Bayesian networks.
