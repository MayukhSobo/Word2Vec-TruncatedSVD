# Word2Vec-TruncatedSVD
Here I am using Amazon Food review Dataset to construct a word2vec like model for its top 2000 and 5000 words. This is using TFIDF
implementation of the word vector to figure out top 2000 or 5000 words and then calculate the cooccurance matrix for all the
top words in the neighbourhood of ± 5 words. Then use that co-occurance matrix and decompose it using TruncatedSVD to calculate
the matrix into Singular values and decomposed matrix and used the Knee method to figure out the right number of components that
maximize the variance and minimize the components and then use these as word vectors. This turned out to be real good because
when using these word vectors with cosine similarity, I came up with contextually similar words pretty easily. This was although
not an exact implementation of word2vec which used Neural Network to create contextual word embedding but it was still pretty 
good enough to use for any word2vec model that holds the contextual semantics of any words.
