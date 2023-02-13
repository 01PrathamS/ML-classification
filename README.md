# ML-classification 

Q: The Differance between transform and fit_transform? 
==> The fit(data) method is used to compute the mean and std dev for a given feature to be used for further scaling.
--->it takes the feature F and it will just compute the mean (μ) and standard deviation (σ) of feature F.

==> The transform(data) is used to perform scaling using mean and std dev calculated using the .fit() method. We have to use .transform() in front of a fit object because we transform the fit calculations.
-->We have to use .transform() in front of a fit object because we transform the fit calculations.
-->the output will we get is always in the form of sparse matrix or array.

==> The fit_transform() method does both fits and transform.
*If we use fit and transform separate when we need both then it will decrease the efficiency of the model so we use fit_transform()


***we cannot use the fit() method on the test dataset, because it will be the wrong approach as it could introduce bias to the testing dataset. So, let us try to use the transform() method directly on the test dataset.

