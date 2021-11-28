# -CMPE255--ANN-algorithms-

- Approximate Nearest Neighbour Search
- Local Sensivity Hashing 
- Exhaustive Search 
- Product Quantization 
- Trees And Graphs 
- HNSW 

## Approximate Nearest Neighbour Search
- Nearest neighbor search (NNS), as a form of proximity search, is the optimization problem of finding the point in a given set that is closest (or most similar) to a given point. Closeness is typically expressed in terms of a dissimilarity function: the less similar the objects, the larger the function values.


## Local Sensitivity Hashing
- An algorithmic technique that hashes similar input items into the same "buckets" with high probability.(The number of buckets is much smaller than the universe of possible input items.) Since similar items end up in the same buckets, this technique can be used for data clustering and nearest neighbor search.

## Exhaustive Search
- IndexFlatL2 measures the L2 (or Euclidean) distance between all given points between our query vector, and the vectors loaded into the index. It’s simple, very accurate, but not too fast.

## Product Quantization
- Product quantization (PQ) is an effective vector quantization method. A product quantizer can generate an exponentially large codebook at very low memory/time cost. The essence of PQ is to decompose the high-dimensional vector space into the Cartesian product of subspaces and then quantize these subspaces separately.

## Trees and Graphs
- Tree-based algorithms are one of the most common strategies when it comes to ANN. They construct forests (collection of trees) as their data structure by splitting the dataset into subsets.One of the most prominent solutions is Annoy.

## Hierarchical NSW
- Hierarchical Navigable Small World: In order to reduce the search time on a graph we would want our graph to have an average path. Many real-world graphs on average are highly clustered and tend to have nodes that are close to each other which are formally called small-world graph


## Dataset Used:
- Kaggel News Data Set
