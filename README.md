# Outlier-Detection-and-correction
-Outlier Detection and Correction Process

Initial approach for outlier detection and correction

 Standard Deviation

The aim of standard deviation for outlier detection is the fact that it checks, if any of the points lies below 3 standard
deviations, away from the mean, if it does, these points are treated as the outlier.

 Zscore

Zscore aims to detect outliers by means of a score which this method computes, known as the Zscore.
Generally Zscore, which is taken above 3 are then treated as an outlier.

 Clustering

Another approach was to use clustering where we had grouped together a set of points
and have tried to find the points which were non-grouped or anomaly points and marked them
as outliers, but we didn’t have a good success compared to Zscore and std deviation for outlier
detection.

What proves an outlier as an outlier?

 Validation of Outliers

The validation to see the confidence of the outliers detected was done by means of
machine learning algorithm named Isolation Forest. The algorithm had the capability to assign
anomaly score to the points/demand and classify them as outliers or not. We had an accuracy of
94% detection for which the algorithm validates it to be an outlier.

Outlier Correction Approach-

 Outlier Correction- Median approach

The correction approach primarily used was a median based approach, which corrected
the outliers by taking median of the values, present in the demand.

 Outlier Correction- Capping Based Approach

The standard deviation serves as the main concept in the capping-based approach, we
are trying to assign caps based on the 99.99th percentile value. We basically flag the points i.e.,
demand which has a value greater than the cap limit and took difference of those demand
with the cap limit, which served as our outlier corrected demand. Below fig shows the capped
based values in our data.
