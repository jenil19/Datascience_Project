# Datascience-Project

This project compares 3 subsampling algorithms: Uniform Subsampling,Lightweight-coreset,ProTras on KDD protein Homology dataset.

Uniform subsampling is a “naive” strategy of uniformly subsampling the data points.ProTras is a farthest-Traversal first based algorithm, and lightweight coreset is based on a mixture of uniform sampling and importance based sampling.

We evaluated mentioned algorithms for subsample size m =100,200,500,1000 and applied k-means++ with number of centers=50 to calculate quantization error.Since K-means++ generates first seed randomly, we run k-means++ with 50 different seeds and take average of the results to get better estimate.we then evaluate k-means++ on full dataset to get actual quantization.we measure relative error between actual quantization error and  quantization error obtained by evaluating algorithms to compare results.we also compared time taken by algorithms in the project.results are given below


![alt text](https://github.com/jenil19/Sampling-algorithm-evaluation/blob/master/comp.png?raw=true)

![alt text](https://github.com/jenil19/Evaluation-of-sampling-algorithms/blob/master/time.png?raw=true)
