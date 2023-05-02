Shannon entropy is a measure of the amount of uncertainty or randomness in a system. It is often used in information theory to quantify the amount of information in a message or data set.

In the context of feature engineering, Shannon entropy can be used to measure the amount of information carried by a categorical feature. Specifically, it can be used to quantify the "surprise" or unpredictability of a feature's values in a dataset.

To compute Shannon entropy on a frequency table, we first calculate the probability of each category occurring in the dataset. We then use these probabilities to calculate the entropy as follows:

�

(

�

)

=

−

∑

�

=

1

�

�

�

log

⁡

2

�

�

H(X)=− 

i=1

∑

n



 p 

i



 log 

2



 p 

i



 

where $X$ is the categorical feature, $n$ is the number of categories, $p_i$ is the probability of category $i$ occurring in the dataset, and $\log_2$ is the base-2 logarithm.

Intuitively, the entropy is higher when the probabilities of each category are more evenly distributed, indicating a greater amount of uncertainty or unpredictability. Conversely, the entropy is lower when one category dominates the dataset, indicating a lower amount of uncertainty.

Shannon entropy can be a useful feature engineering technique for identifying categorical features that are more informative or discriminating than others. It can also be used as a basis for feature selection or dimensionality reduction by identifying features with low entropy as less informative or redundant.
