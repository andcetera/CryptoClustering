# Crypto Clustering
Using Python and Unsupervised Machine Learning algorithms to predict if cryptocurrencies are affected by 24-hour or 7-day price changes  

![cryptocurrency photo](Images/cryptocurrencies-rising.jpg)
- - -
## Project Structure

- **Project Deliverable:** Juptyer Notebook containing project code and analysis can be found [here](Crypto_Clustering.ipynb)  
- Original dataset can be found in the [Resources](Resources/crypto_market_data.csv) folder.  
- Images used in this README can be found in the [Images](Images/) folder.

- - -

## Instructions
### Prepare the Data

- Create a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

    - The first five rows of the scaled DataFrame should appear as follows:

![The first five rows of the scaled DataFrame](Images/scaled_DataFrame.png)

### Find the Best Value for k Using the Original Scaled DataFrame

- Use the elbow method to find the best value for `k`.
- Plot a line chart with all the inertia values computed with the different values of `k` to visually identify the optimal value for `k`.
- Answer the following question in your notebook: What is the best value for `k`?
### Cluster Cryptocurrencies with K-means Using the Original Scaled Data

- Cluster the cryptocurrencies for the best value for `k` on the original scaled data.
- Predict the clusters to group the cryptocurrencies using the original scaled DataFrame.
- Create a scatter plot using hvPlot
### Optimize Clusters with Principal Component Analysis

- Using the original scaled DataFrame, perform a PCA and reduce the features to three principal components.

- Retrieve the explained variance to determine how much information can be attributed to each principal component and then answer the following question in your notebook:

    - What is the total explained variance of the three principal components?
- Create a new DataFrame with the PCA data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

    - The first five rows of the PCA DataFrame should appear as follows:

![The first five rows of the PCA DataFrame](Images/PCA_DataFrame.png)
### Find the Best Value for k Using the PCA Data

- Use the elbow method on the PCA data to find the best value for `k`
- Plot a line chart with all the inertia values computed with the different values of `k` to visually identify the optimal value for `k`.
- Answer the following question in your notebook:
    - What is the best value for `k` when using the PCA data?
    - Does it differ from the best k value found using the original data?
### Cluster Cryptocurrencies with K-means Using the PCA Data

- Cluster the cryptocurrencies for the best value for `k` on the PCA data

- Predict the clusters to group the cryptocurrencies using the PCA data.

- Create a scatter plot using hvPlot

- Answer the following question:
    - What is the impact of using fewer features to cluster the data using K-Means?

- - -
## References
Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.