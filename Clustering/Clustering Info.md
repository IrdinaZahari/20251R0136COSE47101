Categorical Features of Parent Dataset
| Playing Games | Game Duration | Game Time | Hamper Sleep | Headache | Mental Stress | Depression | Attention Level | Academics |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Yes
Sometimes
No | <2 hours
3-4 horus
>5 hours | Afternoon
Evening
Mid-night | Yes
Sometimes
No | Yes
Sometimes
No | Yes
Sometimes
No | Yes
Sometimes
No | Excellent
Good
Averae
Bad | Excellent
Good
Average
Bad |


Originally, our intention was to use One-Hot Encoding or Label Encoding, however found out that they are not suitable for our dataset due to the fact that:

> **Label encoding introduces arbitrary numerical order** to categories. 
If your data is nominal (no inherent order), label encoding can mislead algorithms like K-means, which will treat the numbers as if they have mathematical meaning
> 
> 
> Source： https://www.geeksforgeeks.org/machine-learning/one-hot-encoding-vs-label-encoding/
>



So we use K-Modes clustering, which is a better choice for out dataset.

This is due to the reasons below:

- **K-modes is specifically designed for categorical data** and produces clusters that are easy to interpret because each cluster center is a mode of the actual categorical values
- **K-modes avoids the pitfalls of label encoding** by not imposing any artificial relationships or order between categories, ensuring clusters are based on actual similarities in your data

Below is an example to explain the **Use Case of K-Modes Clustering**.
https://www.kaggle.com/code/ashydv/bank-customer-clustering-k-modes-clustering


### Things to know when using K-Modes

Resource links:

- https://github.com/gowshalinirajalingam/K-Modes-Clustering
- https://github.com/harika-bonthu/KModes/blob/main/kmodes.ipynb

K-modes is used for clustering categorical variables.  It defines clusters based on the number of matching categories between data points. 

There are two well known methods to conduct K-Modes clustering, details are summarized as follows:

| **Method** | **Approach** | **Pros** | **Cons** |
| --- | --- | --- | --- |
| Huang | First k objects or most frequent categories | Simple, fast | Sensitive to data order, unstable |
| Cao | Density and distribution-based selection | More stable, robust, better for real data | Slightly more computation |
