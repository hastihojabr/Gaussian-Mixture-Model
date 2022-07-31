# Gaussian-Mixture-Model
Gaussian mixture models is a famous probabilistic model which can be used for clustering. Its hidden parameters can be determined by expectation-maximization algorithm. I have implement this method on Iris Data-set and Online Retail Data-set and evaluated it using internal and external evaluation methods. 

## Algorithm 

The Expectation Maximization (EM) algorithm is an iterative method that produces maximum-likelihood (ML) estimates of parameters when there is a many-to-one mapping from an underlying distribution to the distribution governing the observation.

1. Initialize π_k, ∑_k, μ_k.
2. Evaluate responsibilities r_nk for every data point. (E step)
3. Re estimate parameters using the new rnk from E-step. (M step)
4. Repeat the last two process untill the parameter estimate has converged.

## Visualization

We visualize clusters in two dimension using Ellipses. We know that covari- ance matrix can be diagonalized. We can diagonlized cov using numpy library and command numpy.linalg.svd.

## Evaluation

In a clustering problem we have to understand how well the data is grouped into different clusters by the algorithm and how many clusters we need.

1. Bayesian information criterion
2. Silhouette score
3. Confusion matrix

# Applications

## Gaussian-Mixture-Model 1D

![em1d](https://user-images.githubusercontent.com/89476798/176494784-0e3f1c86-5358-4644-805b-4ca758c6c065.png)
![download (22)](https://user-images.githubusercontent.com/89476798/176498151-92d8d788-0974-4f31-8154-308b4d45f252.png)
![download (16)](https://user-images.githubusercontent.com/89476798/176494954-6074afbf-5ac6-44a6-bdfc-8990a41fb00f.png)


## Gaussian-Mixture-Model 2D

![emnd](https://user-images.githubusercontent.com/89476798/176494898-f506767d-6ab0-48da-bcdd-355410ae8900.png)
![download (21)](https://user-images.githubusercontent.com/89476798/176494999-01d8df1f-d459-4fc8-bf24-965abe970f07.png)

## The Iris Data set

The Iris Data set is a multivariate data set introduced by the British statistician and biologist Ronald Fisher.
We ignore the target col- umn and cluster data features using GMM. Then we can compare GMM’s prediction and the actual target and do an external evaluation of our model.

![download (13)](https://user-images.githubusercontent.com/89476798/176498332-93518086-89ca-4d9f-9f7c-2db90a53067a.png)

## The Online Retail Data set

Using RFM segmentation technique. where

Recency (R) value is the number of days a customer takes between two purchases. 
Frequency (F) is defined as the number of purchases a customer makes in a specific period. 
Monetary (M) is defined as the amount of money spent by the customer during a certain period.

![em1](https://user-images.githubusercontent.com/89476798/176498354-e3ff4488-c442-4014-8928-7d2d0bdec5b0.png)
![em3](https://user-images.githubusercontent.com/89476798/176498377-a89b2a11-3e2c-4029-93d2-36a9480c0ac1.png)
![em2](https://user-images.githubusercontent.com/89476798/176498389-9d1c224c-ae12-4802-865b-74414736f4e2.png)
