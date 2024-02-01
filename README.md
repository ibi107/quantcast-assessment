# Quantcast Intern Assessment 2024

## Requirements

All the requirements are listed in `requirements.txt`, you can install them with `pip install -r requirements.txt`.
## Reflection

### What does the numerical data alone tell you?
The vector embeddings are uninterpretable by themselves. However, we can extract meaning from them by comparing different embeddings with eachother, in context of the text description provided, one embedding vector next to another embedding vector would share a similar description.

### How well did your chosen algorithm(s) perform?
K-Means allows you to separate datapoints into several segments (or clusters), which are characterised by their midpoints (or centroids). To evaluate the performance of my K-Means algorithm, I tried to confirm whether datapoints in a cluster are similar through their contents. I found that 3/4 clusters contained data which was relevant to that cluster only, and one seemed to contain an amalgamation of data - this could be because I had picked an insufficient value of $k$ (the number of clusters).

### When considering the supplementary data as well, what do you conclude?
By processing the supplementary data within each cluster, it is apparent that each entry in the dataset can be categorised. My methods used vector embeddings to cluster together similar data, but NLP can also be done on the supplementary data to label them.

### Given more time, what would you do next?
I see potential in taking this dataset forward with NLP. I could manually label a subset of the dataset into categories of the type of web page e.g. technology, food, politics, gaming, etc. and train a supervised machine learning model to classify embeddings into categories.