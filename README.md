# Social Computing


## Outline

- Hate Speech Detection
- Clustering
- Centrality Measures
- Twitch Streamers' Friends Network

## Hate Speech Detection

- Tweets: `RACIST`, `SEXIST`, `NEITHER`
- Data Preprocessing: 
    - `One Hot Encoding` for labels
    - `Universal Sentence Encoder` to get text embeddings
- Fully Connected Neural Network

## Clustering

- `Louvain` clustering
- `K-Means` clustering
- `Gaussian Mixture Model` clustering

![kmeans vs. gmm](/ex03/kmeans_vs_gmm.png)
<center>Two Gaussian Distributions and one Normal Distribution</center>



## Centrality Measures

Implementation of `Betweenness Centrality` and `PageRank` centrality measures is performed on a `Krackhardt Kite Graph`.

- `Kite centrality`
- `Betweenness centrality`
- `Epsilon Betweenness centrality`
- `PageRank` centrality measure
- Personalized `PageRank` centrality

## Twitch Streamers' Friends Network

A graph of twitch friends network is constructed and analyzed.

- Sparse Vector Representation: convert dense vector to sparse vector
- Data Preprocessing
    - filter streamers
    - merge nodes with edges

### Graph

- use `networkX` to construct graph from preprocessed data frame
- visualize graph using `Spring Layout` which positions nodes using `Fruchterman-Reingold force-directed algorithm`

![spring layout](/ex01/spring_layout.png)
<center>Spring Layout</center>

- visualize graph using `Kamada Kawai Layout` which positions nodes using `Kamada-Kawai path-length cost-function`

![spring layout](/ex01/kamada_kawai_layout.png)
<center>Kamada Kawai Layout</center>