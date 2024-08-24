# Generating-and-Visualizing-Embeddings
Here we are creating an embeddings and then visualizing them in 2D and 3D.

Steps involved in Generating and visualizing embeddings are as follows: 
1. Import the csv file and convert it to a dataframe. The file that is used contains just one column "reviews" of food items.
2. Convert the dataframe to a list as embeddings can be created for a list.
3. Import SentenceTransforms library and use "All-MiniLM-L6-v2" model to generate the embeddings.
4. The embeddings generated would be in 384 dimensions. It is not possible for human eye to visualize anything in 384 dimensions, so we have to reduce the dimensions from 384 to 2 or 3.
5. For reducing the dimensions we will be using UMAP (Uniform Manifold Approximation and Projections) function of umap-learn library.
6. Before reducing the dimensions we will convert the list of embeddings to tensor.
7. Then finally we will plot the scatter plot for the embeddings using matplotlib and plotly library.
8. After plotting the plot, we found that data can be divided into 3 clusters.
9. We used Kmeans algorithm also to see the 3 different clusters and also saw which review is falling in which cluster.
