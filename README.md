# Social Computing

Implementation of `Betweenness Centrality` and `PageRank` centrality measures is performed on a `Krackhardt Kite Graph`. Additionally, a graph of twitch friends network is constructed and analyzed.

## Outline

- Centrality Measures
- Twitch Streamers' Friends Network

## Centrality Measures

- `Kite centrality` measure
- `Betweenness centrality` measure
- `Betweenness centrality` measure with `epsilon`
- `PageRank` centrality measure
- Personalized `PageRank` centrality measure

## Twitch Streamers' Friends Network

### Sparse Vector Representation

- convert dense vector to sparse vector

### Data

#### musae_DE_target.csv

- each vertex represents a Twitch channel and contains multiple
informations about the channel

#### musae_DE_edges.csv

- edges between the channels/streamers representing their friendship connection
- Represented by `from` & `to` nodes, but are undirected as Twitch‘s friendship system is undirected

#### TwitchIDList.csv

- streamer‘s names for the used IDs of the dataset

### Data Preprocessing

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

## A Comparison of Centrality Measures
