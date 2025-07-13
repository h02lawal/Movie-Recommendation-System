I built two movie recommendation systems using Sklearn TfidfVectorizer, ColumnTransformer and Cosine Similarity. 

In the first recommendation system, the TfidfVectorizer created a vector for each overview, it assigned higher weights to words that were unique within each overview. It then used the cosine similarity matrix to compare each overview. After comparison scores between 0 and 1 were used to show similarity between each pair. A score close to 1 indicates similarity and a score close to 0 indicates no similarity.

I improved the second recommendation system by using two features, overview and genres. Rather than using TfidfVectorizer i used a ColumnTransformer which can create a single vector for multiple features such as overview and genres, i then used Cosine Similarity to group each overview and genres pair with their most similar pair.
