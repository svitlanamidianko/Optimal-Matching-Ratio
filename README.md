Resulting Article on topic (Towards Data Science): https://medium.com/@svitlana_78975/matching-koalas-on-fire-134ad3d2822
# Optimal-Matching-Ratio

As of now, it seems most data scientists use M=1 as a default and a starting point for matching, under the assumption that it usually provides the best balance on covariates.  However, this may not always be the case (e.g. if we seek to match for an observation of age 20.0 and consider the potential matches 17.9 and 22.0, M=1 would match the observation with 22.0, while M=2 would weight 17.9 and 22.0 to return a closer match of 19.95).  We will seek to explore scenarios where one-to-multiple matching provides better balance (than one-to-one matching)—and, by nature, a larger sample size—by coming up with our own very small toy data set(s). 

Specifically, we hope to address the question: what is the optimal matching ratio for a dataset?  This is a function of both (a) maximizing balance on covariates and (b) maximizing sample size i.e. using the highest number of control units (because it is the most representative of the population).  

Does the MatchBalance function validate and reward effectively (i.e. produces a higher minimum p-value for) increased balance thanks to multiple matches?  Or does it discredit this better balance because of the weights on the matches?  Based on our experimentation, we aim to address implications and consider potential algorithmic implementation to address the case scenarios we explored and generally find the optimal value for M to achieve maximum balance.

The final report will be presented as a blog post (which we hope to actually publish), including explanations and accompanying code example(s).  We will inform our analysis with a literature review on the subject.
