Data Preparation

Normalize the Data:

The dataset is normalized using StandardScaler() from scikit-learn to ensure all features have the same scale.

A new DataFrame is created with the scaled data, maintaining coin_id as the index.

Preview the Data:

The first five rows of the scaled DataFrame should display the normalized values.

Finding the Optimal k Using the Elbow Method

Generate a list of k-values ranging from 1 to 11.

Compute the inertia for each k-value using a for loop.

Store the inertia values in a list.

Plot an Elbow Curve to visualize the optimal k-value.

Identify the best k-value from the plot and document the selection.

Clustering Cryptocurrencies with K-Means

Train the K-Means Model:

Initialize the model using the best k-value.

Fit the model on the scaled data.

Predict cluster labels for each cryptocurrency.

Visualization:

Create a scatter plot using hvPlot.

Set x-axis as price_change_percentage_24h and y-axis as price_change_percentage_7d.

Color the points based on cluster labels.

Add coin_id as a hover feature.

Principal Component Analysis (PCA)

Reduce the dataset’s dimensionality to three principal components.

Retrieve the explained variance for each principal component.

Compute the total explained variance and analyze the retained information.

Create a new PCA-transformed DataFrame, keeping coin_id as the index.

Finding the Optimal k Using PCA Data

Repeat the Elbow Method using the PCA-transformed data.

Compare the best k-value obtained with the original dataset.

Answer: Does reducing features impact the clustering?

Clustering Cryptocurrencies Using PCA Data

Train the K-Means Model:

Use the best k-value found for PCA data.

Fit the model on the PCA-transformed dataset.

Predict clusters and add them to the DataFrame.

Visualization:

Create a scatter plot using hvPlot.

Set x-axis as PC1 and y-axis as PC2.

Color points based on cluster labels.

Include coin_id as a hover feature.

Key Insights & Conclusion

The optimal k-value might differ between the original and PCA-transformed data.

Using PCA reduces computational complexity while still retaining essential variance.

Clustering helps identify cryptocurrency market trends and potential investment strategies.

Technologies Used

Python Libraries: Pandas, scikit-learn, hvPlot, Matplotlib

Machine Learning Algorithms: K-Means Clustering, PCA


