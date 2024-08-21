In this notebook, I use word embeddings and clustering to solve the popular New York Times minigame, Connections. The three word embedding models I run are word2vec, fasttext, and GloVe. I run two forms of clustering with cosine similarity, a greedy approach that maximizes similarity in a cluster, removes those elements, maximizes similarity in the next cluster, and repeats; and kmeans constrained. To try and make the word embeddings more discriminative, I implemented the post-processing algorithm (PPA). This algorithm centers the word embeddings about the origin and uses PCA to remove the top principle components (a parameter to choose). 

Future Plans
- Different post-processing algorithms on the Word embeddings, such as PPA -> PCA -> PPA. It also reduces the memory cost of word embeddings greatly.
  
    Source: https://lld-workshop.github.io/2017/papers/LLD_2017_paper_34.pdf
- Different Clustering Techniques. Maybe use something similar to the greedy cluster similarity maximizer and kmeans constrained we did for the first two groups, then for the two harder groups, we can try a brute(ish) force approach.
- Train word embeddings on corpus more in tune with NYT connections game


![image](https://github.com/user-attachments/assets/5b9c0c0c-5150-4fc8-a657-ab4779b4dbe1)
