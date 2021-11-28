# -CMPE255--ANN-algorithms-

- Approximate Nearest Neighbour Search
- Local Sensivity Hashing Using FAISS
- Exhaustive Search using FAISS
- Product Quantization using FAISS
- Trees And Graphs using Annoy
- HNSW using NSMLIB



Dynamic score calculation of MF algorithm
Matrix Factorization (MF) algorithms are becoming more popular these days. In MF, the recommendation score is calculated as the inner product of the generated vector of user items, but if the number of users and items is large, the data size to be retained is very large if the score is pre-calculated for all user x item combinations. It will be.

High speed vector calculation library faiss
Faiss, developed by Facebook Research, is a library that can perform such vector calculations at high speed. It can index a set of vectors (matrix) in the memory in advance and execute score calculation and sorting instantly for the vector given as input.

faiss has the following characteristics:

GPU and multithreaded support for index operations
Dimensionality reduction: vectors with large dimensions can be reduced to smaller dimensions using PCA
Reduction of spatial complexity by dimensional compression
Quantisation: FAISS emphasises on product quantisation for compressing and storing vectors of large dimensions
Batch processing i.e searching for multiple queries at a time
Exhaustive Search
IndexFlatL2 measures the L2 (or Euclidean) distance between all given points between our query vector, and the vectors loaded into the index. It’s simple, very accurate, but not too fast.

Local Sensitivity Hashing
An algorithmic technique that hashes similar input items into the same "buckets" with high probability.(The number of buckets is much smaller than the universe of possible input items.) Since similar items end up in the same buckets, this technique can be used for data clustering and nearest neighbor search.

Trees and Graphs
- Tree-based algorithms are one of the most common strategies when it comes to ANN. They construct forests (collection of trees) as their data structure by splitting the dataset into subsets.One of the most prominent solutions is Annoy.

Hierarchical NSW
Hierarchical NSW incrementally builds a multi-layer structure consisting from hierarchical set of proximity graphs (layers) for nested subsets of the stored elements. The maximum layer in which an element is present is selected randomly with an exponentially decaying probability distribution. This allows producing graphs similar to the previously studied Navigable Small World (NSW) structures while additionally having the links separated by their characteristic distance scales. Starting search from the upper layer together with utilizing the scale separation boosts the performance compared to NSW and allows a logarithmic complexity scaling.

Product Quantization
Product quantization is a great way to compress your large data set vectors to enable faster search results. However, this also affects the accuracy of the results returned. Hence the trade-off between accuracy and memory constraints(or speed) should be critically analyzed while choosing any index in FAISS.
